# Comparing `tmp/idcn-1.0.1.tar.gz` & `tmp/idcn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idcn-1.0.1.tar", last modified: Mon May 27 16:11:05 2024, max compression
+gzip compressed data, was "idcn-1.1.0.tar", last modified: Sun Jun  2 13:26:59 2024, max compression
```

## Comparing `idcn-1.0.1.tar` & `idcn-1.1.0.tar`

### file list

```diff
@@ -1,1120 +1,1120 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.546756 idcn-1.0.1/
--rw-rw-rw-   0        0        0     1085 2024-05-21 16:37:45.000000 idcn-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2591 2024-05-27 16:11:05.546756 idcn-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1424 2024-05-27 14:52:50.000000 idcn-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.892152 idcn-1.0.1/idcn/
--rw-rw-rw-   0        0        0      254 2024-05-27 14:52:30.000000 idcn-1.0.1/idcn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.888463 idcn-1.0.1/idcn/releases/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.884440 idcn-1.0.1/idcn/releases/3.10/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.940924 idcn-1.0.1/idcn/releases/3.10/idlelib/
--rw-rw-rw-   0        0        0     2152 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/CREDITS.txt
--rw-rw-rw-   0        0        0    56360 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/ChangeLog
--rw-rw-rw-   0        0        0    10312 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/HISTORY.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.948922 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/
--rw-rw-rw-   0        0        0      443 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/README.txt
--rw-rw-rw-   0        0        0      120 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/folder.gif
--rw-rw-rw-   0        0        0    57746 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle.ico
--rw-rw-rw-   0        0        0      634 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_16.gif
--rw-rw-rw-   0        0        0     1031 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    39205 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     1019 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_32.gif
--rw-rw-rw-   0        0        0     2036 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     1388 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_48.gif
--rw-rw-rw-   0        0        0     3977 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_48.png
--rw-rw-rw-   0        0        0       75 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/minusnode.gif
--rw-rw-rw-   0        0        0      125 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/openfolder.gif
--rw-rw-rw-   0        0        0       78 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/plusnode.gif
--rw-rw-rw-   0        0        0      380 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/python.gif
--rw-rw-rw-   0        0        0       72 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/tk.gif
--rw-rw-rw-   0        0        0    54195 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/NEWS.txt
--rw-rw-rw-   0        0        0    27172 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/NEWS2x.txt
--rw-rw-rw-   0        0        0    11653 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/README.txt
--rw-rw-rw-   0        0        0     8478 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/TODO.txt
--rw-rw-rw-   0        0        0      396 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/__main__.py
--rw-rw-rw-   0        0        0     9354 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/autocomplete.py
--rw-rw-rw-   0        0        0    21097 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/autocomplete_w.py
--rw-rw-rw-   0        0        0     3216 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/autoexpand.py
--rw-rw-rw-   0        0        0     8588 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/browser.py
--rw-rw-rw-   0        0        0     7265 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/calltip.py
--rw-rw-rw-   0        0        0     7158 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/calltip_w.py
--rw-rw-rw-   0        0        0    11429 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/codecontext.py
--rw-rw-rw-   0        0        0    14773 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/colorizer.py
--rw-rw-rw-   0        0        0     2266 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/config-extensions.def
--rw-rw-rw-   0        0        0     2868 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/config-highlight.def
--rw-rw-rw-   0        0        0    10906 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/config-keys.def
--rw-rw-rw-   0        0        0     3167 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/config-main.def
--rw-rw-rw-   0        0        0    38201 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/config.py
--rw-rw-rw-   0        0        0    14978 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/config_key.py
--rw-rw-rw-   0        0        0   105758 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/configdialog.py
--rw-rw-rw-   0        0        0    19186 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/debugger.py
--rw-rw-rw-   0        0        0    12170 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/debugger_r.py
--rw-rw-rw-   0        0        0     4055 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/debugobj.py
--rw-rw-rw-   0        0        0     1082 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/debugobj_r.py
--rw-rw-rw-   0        0        0     1043 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/delegator.py
--rw-rw-rw-   0        0        0     1991 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/dynoption.py
--rw-rw-rw-   0        0        0    69049 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/editor.py
--rw-rw-rw-   0        0        0     3631 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/extend.txt
--rw-rw-rw-   0        0        0     3875 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/filelist.py
--rw-rw-rw-   0        0        0    15825 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/format.py
--rw-rw-rw-   0        0        0     7465 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/grep.py
--rw-rw-rw-   0        0        0    79125 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/help.html
--rw-rw-rw-   0        0        0    11863 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/help.py
--rw-rw-rw-   0        0        0     9123 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/help_about.py
--rw-rw-rw-   0        0        0     4064 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/history.py
--rw-rw-rw-   0        0        0    12889 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/hyperparser.py
--rwxrwxrwx   0        0        0      173 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle.bat
--rw-rw-rw-   0        0        0      454 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle.py
--rw-rw-rw-   0        0        0      570 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle.pyw
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.990929 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/
--rw-rw-rw-   0        0        0     8729 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/README.txt
--rw-rw-rw-   0        0        0      712 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/example_noext
--rw-rw-rw-   0        0        0       87 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/example_stub.pyi
--rw-rw-rw-   0        0        0    15199 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/htest.py
--rw-rw-rw-   0        0        0     1943 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/mock_idle.py
--rw-rw-rw-   0        0        0    11693 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/mock_tk.py
--rw-rw-rw-   0        0        0      642 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/template.py
--rw-rw-rw-   0        0        0    11093 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_autocomplete.py
--rw-rw-rw-   0        0        0      720 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_autocomplete_w.py
--rw-rw-rw-   0        0        0     4638 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_autoexpand.py
--rw-rw-rw-   0        0        0     8420 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_browser.py
--rw-rw-rw-   0        0        0    13194 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_calltip.py
--rw-rw-rw-   0        0        0      686 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_calltip_w.py
--rw-rw-rw-   0        0        0    16082 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_codecontext.py
--rw-rw-rw-   0        0        0    22882 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_colorizer.py
--rw-rw-rw-   0        0        0    32046 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_config.py
--rw-rw-rw-   0        0        0    11462 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_config_key.py
--rw-rw-rw-   0        0        0    55344 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_configdialog.py
--rw-rw-rw-   0        0        0      571 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugger.py
--rw-rw-rw-   0        0        0      965 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugger_r.py
--rw-rw-rw-   0        0        0     1561 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugobj.py
--rw-rw-rw-   0        0        0      545 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugobj_r.py
--rw-rw-rw-   0        0        0     1567 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_delegator.py
--rw-rw-rw-   0        0        0     2564 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_editmenu.py
--rw-rw-rw-   0        0        0     7220 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_editor.py
--rw-rw-rw-   0        0        0      795 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_filelist.py
--rw-rw-rw-   0        0        0    23610 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_format.py
--rw-rw-rw-   0        0        0     5072 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_grep.py
--rw-rw-rw-   0        0        0      849 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_help.py
--rw-rw-rw-   0        0        0     5919 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_help_about.py
--rw-rw-rw-   0        0        0     5517 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_history.py
--rw-rw-rw-   0        0        0     9082 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_hyperparser.py
--rw-rw-rw-   0        0        0     2194 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_iomenu.py
--rw-rw-rw-   0        0        0     3444 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_macosx.py
--rw-rw-rw-   0        0        0     1638 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_mainmenu.py
--rw-rw-rw-   0        0        0     1317 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_multicall.py
--rw-rw-rw-   0        0        0     5422 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_outwin.py
--rw-rw-rw-   0        0        0     3544 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_parenmatch.py
--rw-rw-rw-   0        0        0     2422 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_pathbrowser.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_percolator.py
--rw-rw-rw-   0        0        0    19365 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_pyparse.py
--rw-rw-rw-   0        0        0     4965 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_pyshell.py
--rw-rw-rw-   0        0        0    15454 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_query.py
--rw-rw-rw-   0        0        0     4176 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_redirector.py
--rw-rw-rw-   0        0        0     8299 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_replace.py
--rw-rw-rw-   0        0        0      805 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_rpc.py
--rw-rw-rw-   0        0        0    15687 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_run.py
--rw-rw-rw-   0        0        0      777 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_runscript.py
--rw-rw-rw-   0        0        0      496 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_scrolledlist.py
--rw-rw-rw-   0        0        0     2459 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_search.py
--rw-rw-rw-   0        0        0     5691 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_searchbase.py
--rw-rw-rw-   0        0        0    11588 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_searchengine.py
--rw-rw-rw-   0        0        0    26573 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_sidebar.py
--rw-rw-rw-   0        0        0    19680 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_squeezer.py
--rw-rw-rw-   0        0        0     1206 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_stackviewer.py
--rw-rw-rw-   0        0        0     1133 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_statusbar.py
--rw-rw-rw-   0        0        0     6970 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_text.py
--rw-rw-rw-   0        0        0     7364 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_textview.py
--rw-rw-rw-   0        0        0     5385 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_tooltip.py
--rw-rw-rw-   0        0        0     1752 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_tree.py
--rw-rw-rw-   0        0        0     4228 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_undo.py
--rw-rw-rw-   0        0        0      308 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_util.py
--rw-rw-rw-   0        0        0     2740 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_warning.py
--rw-rw-rw-   0        0        0     1075 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_window.py
--rw-rw-rw-   0        0        0      999 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_zoomheight.py
--rw-rw-rw-   0        0        0     4455 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_zzdummy.py
--rw-rw-rw-   0        0        0     2333 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/tkinter_testing_utils.py
--rw-rw-rw-   0        0        0    16102 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/iomenu.py
--rw-rw-rw-   0        0        0    10129 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/macosx.py
--rw-rw-rw-   0        0        0     4118 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/mainmenu.py
--rw-rw-rw-   0        0        0    18648 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/multicall.py
--rw-rw-rw-   0        0        0     5657 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/outwin.py
--rw-rw-rw-   0        0        0     7204 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/parenmatch.py
--rw-rw-rw-   0        0        0     3198 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/pathbrowser.py
--rw-rw-rw-   0        0        0     3546 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/percolator.py
--rw-rw-rw-   0        0        0    19864 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/pyparse.py
--rw-rw-rw-   0        0        0    63008 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/pyshell.py
--rw-rw-rw-   0        0        0    15146 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/query.py
--rw-rw-rw-   0        0        0     6875 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/redirector.py
--rw-rw-rw-   0        0        0     9985 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/replace.py
--rw-rw-rw-   0        0        0    21075 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/rpc.py
--rw-rw-rw-   0        0        0    21418 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/run.py
--rw-rw-rw-   0        0        0     8278 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/runscript.py
--rw-rw-rw-   0        0        0     4464 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/scrolledlist.py
--rw-rw-rw-   0        0        0     5572 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/search.py
--rw-rw-rw-   0        0        0     7859 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/searchbase.py
--rw-rw-rw-   0        0        0     7359 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/searchengine.py
--rw-rw-rw-   0        0        0    20360 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/sidebar.py
--rw-rw-rw-   0        0        0    12845 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/squeezer.py
--rw-rw-rw-   0        0        0     4454 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/stackviewer.py
--rw-rw-rw-   0        0        0     1472 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/statusbar.py
--rw-rw-rw-   0        0        0     6817 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/textview.py
--rw-rw-rw-   0        0        0     6557 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/tooltip.py
--rw-rw-rw-   0        0        0    16443 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/tree.py
--rw-rw-rw-   0        0        0    11046 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/undo.py
--rw-rw-rw-   0        0        0      701 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/util.py
--rw-rw-rw-   0        0        0     2616 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/window.py
--rw-rw-rw-   0        0        0     4179 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/zoomheight.py
--rw-rw-rw-   0        0        0     2005 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/idlelib/zzdummy.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.005803 idcn-1.0.1/idcn/releases/3.10/turtledemo/
--rw-rw-rw-   0        0        0      316 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/__init__.py
--rw-rw-rw-   0        0        0    14830 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/__main__.py
--rw-rw-rw-   0        0        0      160 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/turtle.cfg
--rw-rw-rw-   0        0        0     3405 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/分形曲线.py
--rw-rw-rw-   0        0        0     1117 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/双画布.py
--rw-rw-rw-   0        0        0     1068 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/和平旗.py
--rw-rw-rw-   0        0        0     4172 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/字节设计.py
--rw-rw-rw-   0        0        0     3386 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/平铺图案.py
--rw-rw-rw-   0        0        0     6520 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/拿火柴.py
--rw-rw-rw-   0        0        0     5018 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/排序动画.py
--rw-rw-rw-   0        0        0     3124 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/时钟.py
--rw-rw-rw-   0        0        0     1999 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/极简汉诺塔.py
--rw-rw-rw-   0        0        0     2412 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/林登麦伊尔.py
--rw-rw-rw-   0        0        0     1338 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/树.py
--rw-rw-rw-   0        0        0     3020 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/森林.py
--rw-rw-rw-   0        0        0      949 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/混乱.py
--rw-rw-rw-   0        0        0     1204 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/画图.py
--rw-rw-rw-   0        0        0     1306 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/花形.py
--rw-rw-rw-   0        0        0     2741 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/行星系统.py
--rw-rw-rw-   0        0        0     1706 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/跳舞.py
--rw-rw-rw-   0        0        0      793 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/阴阳.py
--rw-rw-rw-   0        0        0     1356 2024-05-27 14:55:08.000000 idcn-1.0.1/idcn/releases/3.10/turtledemo/颜色混合器.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.885438 idcn-1.0.1/idcn/releases/3.11/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.052324 idcn-1.0.1/idcn/releases/3.11/idlelib/
--rw-rw-rw-   0        0        0     2152 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/CREDITS.txt
--rw-rw-rw-   0        0        0    56360 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/ChangeLog
--rw-rw-rw-   0        0        0    10312 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/HISTORY.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.061318 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/
--rw-rw-rw-   0        0        0      443 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/README.txt
--rw-rw-rw-   0        0        0      120 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/folder.gif
--rw-rw-rw-   0        0        0    57746 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle.ico
--rw-rw-rw-   0        0        0      634 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_16.gif
--rw-rw-rw-   0        0        0     1031 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    39205 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     1019 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_32.gif
--rw-rw-rw-   0        0        0     2036 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     1388 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_48.gif
--rw-rw-rw-   0        0        0     3977 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_48.png
--rw-rw-rw-   0        0        0       75 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/minusnode.gif
--rw-rw-rw-   0        0        0      125 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/openfolder.gif
--rw-rw-rw-   0        0        0       78 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/plusnode.gif
--rw-rw-rw-   0        0        0      380 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/python.gif
--rw-rw-rw-   0        0        0       72 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/tk.gif
--rw-rw-rw-   0        0        0    27172 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/NEWS2x.txt
--rw-rw-rw-   0        0        0    55422 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/News3.txt
--rw-rw-rw-   0        0        0    11653 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/README.txt
--rw-rw-rw-   0        0        0     8478 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/TODO.txt
--rw-rw-rw-   0        0        0      396 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/__main__.py
--rw-rw-rw-   0        0        0     9354 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/autocomplete.py
--rw-rw-rw-   0        0        0    20863 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/autocomplete_w.py
--rw-rw-rw-   0        0        0     3216 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/autoexpand.py
--rw-rw-rw-   0        0        0     8590 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/browser.py
--rw-rw-rw-   0        0        0     7265 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/calltip.py
--rw-rw-rw-   0        0        0     7083 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/calltip_w.py
--rw-rw-rw-   0        0        0    11429 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/codecontext.py
--rw-rw-rw-   0        0        0    14783 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/colorizer.py
--rw-rw-rw-   0        0        0     2266 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/config-extensions.def
--rw-rw-rw-   0        0        0     2868 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/config-highlight.def
--rw-rw-rw-   0        0        0    10906 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/config-keys.def
--rw-rw-rw-   0        0        0     3167 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/config-main.def
--rw-rw-rw-   0        0        0    38414 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/config.py
--rw-rw-rw-   0        0        0    14978 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/config_key.py
--rw-rw-rw-   0        0        0   105344 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/configdialog.py
--rw-rw-rw-   0        0        0    21073 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/debugger.py
--rw-rw-rw-   0        0        0    12118 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/debugger_r.py
--rw-rw-rw-   0        0        0     4177 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/debugobj.py
--rw-rw-rw-   0        0        0     1082 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/debugobj_r.py
--rw-rw-rw-   0        0        0     1044 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/delegator.py
--rw-rw-rw-   0        0        0     1993 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/dynoption.py
--rw-rw-rw-   0        0        0    72225 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/editor.py
--rw-rw-rw-   0        0        0     3631 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/extend.txt
--rw-rw-rw-   0        0        0     3870 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/filelist.py
--rw-rw-rw-   0        0        0    15825 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/format.py
--rw-rw-rw-   0        0        0     7512 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/grep.py
--rw-rw-rw-   0        0        0    78525 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/help.html
--rw-rw-rw-   0        0        0    11911 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/help.py
--rw-rw-rw-   0        0        0     8929 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/help_about.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/history.py
--rw-rw-rw-   0        0        0    12889 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/hyperparser.py
--rwxrwxrwx   0        0        0      173 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle.bat
--rw-rw-rw-   0        0        0      454 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle.py
--rw-rw-rw-   0        0        0      570 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle.pyw
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.102808 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/
--rw-rw-rw-   0        0        0     8880 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/README.txt
--rw-rw-rw-   0        0        0     1250 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/example_noext
--rw-rw-rw-   0        0        0      154 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/example_stub.pyi
--rw-rw-rw-   0        0        0    15313 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/htest.py
--rw-rw-rw-   0        0        0     1943 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/mock_idle.py
--rw-rw-rw-   0        0        0    11693 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/mock_tk.py
--rw-rw-rw-   0        0        0      642 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/template.py
--rw-rw-rw-   0        0        0    11093 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_autocomplete.py
--rw-rw-rw-   0        0        0      720 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_autocomplete_w.py
--rw-rw-rw-   0        0        0     4638 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_autoexpand.py
--rw-rw-rw-   0        0        0     8420 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_browser.py
--rw-rw-rw-   0        0        0    13658 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_calltip.py
--rw-rw-rw-   0        0        0      686 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_calltip_w.py
--rw-rw-rw-   0        0        0    16082 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_codecontext.py
--rw-rw-rw-   0        0        0    22882 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_colorizer.py
--rw-rw-rw-   0        0        0    32091 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_config.py
--rw-rw-rw-   0        0        0    11462 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_config_key.py
--rw-rw-rw-   0        0        0    55389 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_configdialog.py
--rw-rw-rw-   0        0        0     9727 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugger.py
--rw-rw-rw-   0        0        0      965 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugger_r.py
--rw-rw-rw-   0        0        0     1611 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugobj.py
--rw-rw-rw-   0        0        0      545 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugobj_r.py
--rw-rw-rw-   0        0        0     1567 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_delegator.py
--rw-rw-rw-   0        0        0     2564 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_editmenu.py
--rw-rw-rw-   0        0        0     8151 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_editor.py
--rw-rw-rw-   0        0        0      795 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_filelist.py
--rw-rw-rw-   0        0        0    23610 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_format.py
--rw-rw-rw-   0        0        0     5072 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_grep.py
--rw-rw-rw-   0        0        0      863 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_help.py
--rw-rw-rw-   0        0        0     5904 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_help_about.py
--rw-rw-rw-   0        0        0     5517 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_history.py
--rw-rw-rw-   0        0        0     9082 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_hyperparser.py
--rw-rw-rw-   0        0        0     2457 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_iomenu.py
--rw-rw-rw-   0        0        0     3444 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_macosx.py
--rw-rw-rw-   0        0        0     1638 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_mainmenu.py
--rw-rw-rw-   0        0        0     1317 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_multicall.py
--rw-rw-rw-   0        0        0     5417 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_outwin.py
--rw-rw-rw-   0        0        0     3544 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_parenmatch.py
--rw-rw-rw-   0        0        0     2422 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_pathbrowser.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_percolator.py
--rw-rw-rw-   0        0        0    19365 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_pyparse.py
--rw-rw-rw-   0        0        0     4965 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_pyshell.py
--rw-rw-rw-   0        0        0    15454 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_query.py
--rw-rw-rw-   0        0        0     4176 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_redirector.py
--rw-rw-rw-   0        0        0     8299 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_replace.py
--rw-rw-rw-   0        0        0      805 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_rpc.py
--rw-rw-rw-   0        0        0    15687 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_run.py
--rw-rw-rw-   0        0        0      777 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_runscript.py
--rw-rw-rw-   0        0        0      496 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_scrolledlist.py
--rw-rw-rw-   0        0        0     2459 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_search.py
--rw-rw-rw-   0        0        0     5691 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_searchbase.py
--rw-rw-rw-   0        0        0    11588 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_searchengine.py
--rw-rw-rw-   0        0        0    26854 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_sidebar.py
--rw-rw-rw-   0        0        0    19656 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_squeezer.py
--rw-rw-rw-   0        0        0      991 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_stackviewer.py
--rw-rw-rw-   0        0        0     1133 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_statusbar.py
--rw-rw-rw-   0        0        0     6970 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_text.py
--rw-rw-rw-   0        0        0     7364 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_textview.py
--rw-rw-rw-   0        0        0     5385 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_tooltip.py
--rw-rw-rw-   0        0        0     1752 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_tree.py
--rw-rw-rw-   0        0        0     4228 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_undo.py
--rw-rw-rw-   0        0        0      308 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_util.py
--rw-rw-rw-   0        0        0     2740 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_warning.py
--rw-rw-rw-   0        0        0     1075 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_window.py
--rw-rw-rw-   0        0        0      999 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_zoomheight.py
--rw-rw-rw-   0        0        0     4455 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_zzdummy.py
--rw-rw-rw-   0        0        0     2333 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/tkinter_testing_utils.py
--rw-rw-rw-   0        0        0    16289 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/iomenu.py
--rw-rw-rw-   0        0        0     9380 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/macosx.py
--rw-rw-rw-   0        0        0     4118 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/mainmenu.py
--rw-rw-rw-   0        0        0    18652 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/multicall.py
--rw-rw-rw-   0        0        0     5663 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/outwin.py
--rw-rw-rw-   0        0        0     7204 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/parenmatch.py
--rw-rw-rw-   0        0        0     3098 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/pathbrowser.py
--rw-rw-rw-   0        0        0     3568 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/percolator.py
--rw-rw-rw-   0        0        0    19864 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/pyparse.py
--rw-rw-rw-   0        0        0    62574 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/pyshell.py
--rw-rw-rw-   0        0        0    15138 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/query.py
--rw-rw-rw-   0        0        0     6777 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/redirector.py
--rw-rw-rw-   0        0        0     9827 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/replace.py
--rw-rw-rw-   0        0        0    21071 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/rpc.py
--rw-rw-rw-   0        0        0    21352 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/run.py
--rw-rw-rw-   0        0        0     8278 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/runscript.py
--rw-rw-rw-   0        0        0     4477 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/scrolledlist.py
--rw-rw-rw-   0        0        0     5573 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/search.py
--rw-rw-rw-   0        0        0     7859 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/searchbase.py
--rw-rw-rw-   0        0        0     7409 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/searchengine.py
--rw-rw-rw-   0        0        0    20341 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/sidebar.py
--rw-rw-rw-   0        0        0    12845 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/squeezer.py
--rw-rw-rw-   0        0        0     4016 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/stackviewer.py
--rw-rw-rw-   0        0        0     1474 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/statusbar.py
--rw-rw-rw-   0        0        0     6812 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/textview.py
--rw-rw-rw-   0        0        0     6471 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/tooltip.py
--rw-rw-rw-   0        0        0    16556 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/tree.py
--rw-rw-rw-   0        0        0    11016 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/undo.py
--rw-rw-rw-   0        0        0      731 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/util.py
--rw-rw-rw-   0        0        0     2616 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/window.py
--rw-rw-rw-   0        0        0     4179 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/zoomheight.py
--rw-rw-rw-   0        0        0     2005 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/idlelib/zzdummy.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.115778 idcn-1.0.1/idcn/releases/3.11/turtledemo/
--rw-rw-rw-   0        0        0      316 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/__init__.py
--rw-rw-rw-   0        0        0    15065 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/__main__.py
--rw-rw-rw-   0        0        0      160 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/turtle.cfg
--rw-rw-rw-   0        0        0     3405 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/分形曲线.py
--rw-rw-rw-   0        0        0     1117 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/双画布.py
--rw-rw-rw-   0        0        0     1068 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/和平旗.py
--rw-rw-rw-   0        0        0     4172 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/字节设计.py
--rw-rw-rw-   0        0        0     3386 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/平铺图案.py
--rw-rw-rw-   0        0        0     6520 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/拿火柴.py
--rw-rw-rw-   0        0        0     5018 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/排序动画.py
--rw-rw-rw-   0        0        0     3124 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/时钟.py
--rw-rw-rw-   0        0        0     1999 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/极简汉诺塔.py
--rw-rw-rw-   0        0        0     2412 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/林登麦伊尔.py
--rw-rw-rw-   0        0        0     1338 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/树.py
--rw-rw-rw-   0        0        0     3020 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/森林.py
--rw-rw-rw-   0        0        0      949 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/混乱.py
--rw-rw-rw-   0        0        0     1204 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/画图.py
--rw-rw-rw-   0        0        0     1306 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/花形.py
--rw-rw-rw-   0        0        0     2741 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/行星系统.py
--rw-rw-rw-   0        0        0     1706 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/跳舞.py
--rw-rw-rw-   0        0        0      793 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/阴阳.py
--rw-rw-rw-   0        0        0     1356 2024-05-27 14:55:07.000000 idcn-1.0.1/idcn/releases/3.11/turtledemo/颜色混合器.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.886440 idcn-1.0.1/idcn/releases/3.12/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.160336 idcn-1.0.1/idcn/releases/3.12/idlelib/
--rw-rw-rw-   0        0        0     2152 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/CREDITS.txt
--rw-rw-rw-   0        0        0    56360 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/ChangeLog
--rw-rw-rw-   0        0        0    10312 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/HISTORY.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.169738 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/
--rw-rw-rw-   0        0        0      443 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/README.txt
--rw-rw-rw-   0        0        0      120 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/folder.gif
--rw-rw-rw-   0        0        0    57746 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle.ico
--rw-rw-rw-   0        0        0      634 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_16.gif
--rw-rw-rw-   0        0        0     1031 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    39205 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     1019 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_32.gif
--rw-rw-rw-   0        0        0     2036 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     1388 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_48.gif
--rw-rw-rw-   0        0        0     3977 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_48.png
--rw-rw-rw-   0        0        0       75 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/minusnode.gif
--rw-rw-rw-   0        0        0      125 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/openfolder.gif
--rw-rw-rw-   0        0        0       78 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/plusnode.gif
--rw-rw-rw-   0        0        0      380 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/python.gif
--rw-rw-rw-   0        0        0       72 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/tk.gif
--rw-rw-rw-   0        0        0    27172 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/NEWS2x.txt
--rw-rw-rw-   0        0        0    55577 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/News3.txt
--rw-rw-rw-   0        0        0    11653 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/README.txt
--rw-rw-rw-   0        0        0     8478 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/TODO.txt
--rw-rw-rw-   0        0        0      396 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/__main__.py
--rw-rw-rw-   0        0        0     9354 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/autocomplete.py
--rw-rw-rw-   0        0        0    20863 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/autocomplete_w.py
--rw-rw-rw-   0        0        0     3216 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/autoexpand.py
--rw-rw-rw-   0        0        0     8590 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/browser.py
--rw-rw-rw-   0        0        0     7265 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/calltip.py
--rw-rw-rw-   0        0        0     7083 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/calltip_w.py
--rw-rw-rw-   0        0        0    11429 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/codecontext.py
--rw-rw-rw-   0        0        0    14783 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/colorizer.py
--rw-rw-rw-   0        0        0     2266 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/config-extensions.def
--rw-rw-rw-   0        0        0     2868 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/config-highlight.def
--rw-rw-rw-   0        0        0    10906 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/config-keys.def
--rw-rw-rw-   0        0        0     3167 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/config-main.def
--rw-rw-rw-   0        0        0    38429 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/config.py
--rw-rw-rw-   0        0        0    14978 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/config_key.py
--rw-rw-rw-   0        0        0   105344 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/configdialog.py
--rw-rw-rw-   0        0        0    21073 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/debugger.py
--rw-rw-rw-   0        0        0    12118 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/debugger_r.py
--rw-rw-rw-   0        0        0     4177 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/debugobj.py
--rw-rw-rw-   0        0        0     1082 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/debugobj_r.py
--rw-rw-rw-   0        0        0     1044 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/delegator.py
--rw-rw-rw-   0        0        0     1993 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/dynoption.py
--rw-rw-rw-   0        0        0    72225 2024-05-27 14:55:06.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/editor.py
--rw-rw-rw-   0        0        0     3631 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/extend.txt
--rw-rw-rw-   0        0        0     3870 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/filelist.py
--rw-rw-rw-   0        0        0    15825 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/format.py
--rw-rw-rw-   0        0        0     7512 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/grep.py
--rw-rw-rw-   0        0        0    78525 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/help.html
--rw-rw-rw-   0        0        0    11980 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/help.py
--rw-rw-rw-   0        0        0     8929 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/help_about.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/history.py
--rw-rw-rw-   0        0        0    12889 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/hyperparser.py
--rwxrwxrwx   0        0        0      173 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle.bat
--rw-rw-rw-   0        0        0      454 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle.py
--rw-rw-rw-   0        0        0      570 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle.pyw
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.212194 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/
--rw-rw-rw-   0        0        0     8880 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/README.txt
--rw-rw-rw-   0        0        0     1250 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/example_noext
--rw-rw-rw-   0        0        0      154 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/example_stub.pyi
--rw-rw-rw-   0        0        0    15313 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/htest.py
--rw-rw-rw-   0        0        0     1943 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/mock_idle.py
--rw-rw-rw-   0        0        0    11693 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/mock_tk.py
--rw-rw-rw-   0        0        0      642 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/template.py
--rw-rw-rw-   0        0        0    11093 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_autocomplete.py
--rw-rw-rw-   0        0        0      720 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_autocomplete_w.py
--rw-rw-rw-   0        0        0     4638 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_autoexpand.py
--rw-rw-rw-   0        0        0     8420 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_browser.py
--rw-rw-rw-   0        0        0    13658 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_calltip.py
--rw-rw-rw-   0        0        0      686 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_calltip_w.py
--rw-rw-rw-   0        0        0    16082 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_codecontext.py
--rw-rw-rw-   0        0        0    22882 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_colorizer.py
--rw-rw-rw-   0        0        0    32091 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_config.py
--rw-rw-rw-   0        0        0    11462 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_config_key.py
--rw-rw-rw-   0        0        0    55389 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_configdialog.py
--rw-rw-rw-   0        0        0     9727 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugger.py
--rw-rw-rw-   0        0        0      965 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugger_r.py
--rw-rw-rw-   0        0        0     1611 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugobj.py
--rw-rw-rw-   0        0        0      545 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugobj_r.py
--rw-rw-rw-   0        0        0     1567 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_delegator.py
--rw-rw-rw-   0        0        0     2564 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_editmenu.py
--rw-rw-rw-   0        0        0     8151 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_editor.py
--rw-rw-rw-   0        0        0      795 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_filelist.py
--rw-rw-rw-   0        0        0    23610 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_format.py
--rw-rw-rw-   0        0        0     5072 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_grep.py
--rw-rw-rw-   0        0        0      863 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_help.py
--rw-rw-rw-   0        0        0     5904 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_help_about.py
--rw-rw-rw-   0        0        0     5517 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_history.py
--rw-rw-rw-   0        0        0     9082 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_hyperparser.py
--rw-rw-rw-   0        0        0     2457 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_iomenu.py
--rw-rw-rw-   0        0        0     3444 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_macosx.py
--rw-rw-rw-   0        0        0     1638 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_mainmenu.py
--rw-rw-rw-   0        0        0     1317 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_multicall.py
--rw-rw-rw-   0        0        0     5417 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_outwin.py
--rw-rw-rw-   0        0        0     3544 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_parenmatch.py
--rw-rw-rw-   0        0        0     2422 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_pathbrowser.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_percolator.py
--rw-rw-rw-   0        0        0    19365 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_pyparse.py
--rw-rw-rw-   0        0        0     4965 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_pyshell.py
--rw-rw-rw-   0        0        0    15454 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_query.py
--rw-rw-rw-   0        0        0     4176 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_redirector.py
--rw-rw-rw-   0        0        0     8299 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_replace.py
--rw-rw-rw-   0        0        0      805 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_rpc.py
--rw-rw-rw-   0        0        0    15756 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_run.py
--rw-rw-rw-   0        0        0      777 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_runscript.py
--rw-rw-rw-   0        0        0      496 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_scrolledlist.py
--rw-rw-rw-   0        0        0     2459 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_search.py
--rw-rw-rw-   0        0        0     5691 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_searchbase.py
--rw-rw-rw-   0        0        0    11588 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_searchengine.py
--rw-rw-rw-   0        0        0    26854 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_sidebar.py
--rw-rw-rw-   0        0        0    19656 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_squeezer.py
--rw-rw-rw-   0        0        0      991 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_stackviewer.py
--rw-rw-rw-   0        0        0     1133 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_statusbar.py
--rw-rw-rw-   0        0        0     6970 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_text.py
--rw-rw-rw-   0        0        0     7364 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_textview.py
--rw-rw-rw-   0        0        0     5385 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_tooltip.py
--rw-rw-rw-   0        0        0     1752 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_tree.py
--rw-rw-rw-   0        0        0     4228 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_undo.py
--rw-rw-rw-   0        0        0      308 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_util.py
--rw-rw-rw-   0        0        0     2740 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_warning.py
--rw-rw-rw-   0        0        0     1075 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_window.py
--rw-rw-rw-   0        0        0      999 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_zoomheight.py
--rw-rw-rw-   0        0        0     4455 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_zzdummy.py
--rw-rw-rw-   0        0        0     2333 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/tkinter_testing_utils.py
--rw-rw-rw-   0        0        0    16289 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/iomenu.py
--rw-rw-rw-   0        0        0     9269 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/macosx.py
--rw-rw-rw-   0        0        0     4118 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/mainmenu.py
--rw-rw-rw-   0        0        0    18652 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/multicall.py
--rw-rw-rw-   0        0        0     5663 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/outwin.py
--rw-rw-rw-   0        0        0     7204 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/parenmatch.py
--rw-rw-rw-   0        0        0     3098 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/pathbrowser.py
--rw-rw-rw-   0        0        0     3568 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/percolator.py
--rw-rw-rw-   0        0        0    19864 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/pyparse.py
--rw-rw-rw-   0        0        0    62241 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/pyshell.py
--rw-rw-rw-   0        0        0    15138 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/query.py
--rw-rw-rw-   0        0        0     6777 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/redirector.py
--rw-rw-rw-   0        0        0     9827 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/replace.py
--rw-rw-rw-   0        0        0    21071 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/rpc.py
--rw-rw-rw-   0        0        0    21375 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/run.py
--rw-rw-rw-   0        0        0     8278 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/runscript.py
--rw-rw-rw-   0        0        0     4477 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/scrolledlist.py
--rw-rw-rw-   0        0        0     5573 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/search.py
--rw-rw-rw-   0        0        0     7859 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/searchbase.py
--rw-rw-rw-   0        0        0     7409 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/searchengine.py
--rw-rw-rw-   0        0        0    20341 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/sidebar.py
--rw-rw-rw-   0        0        0    12845 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/squeezer.py
--rw-rw-rw-   0        0        0     4016 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/stackviewer.py
--rw-rw-rw-   0        0        0     1474 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/statusbar.py
--rw-rw-rw-   0        0        0     6812 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/textview.py
--rw-rw-rw-   0        0        0     6471 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/tooltip.py
--rw-rw-rw-   0        0        0    16556 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/tree.py
--rw-rw-rw-   0        0        0    11016 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/undo.py
--rw-rw-rw-   0        0        0     1312 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/util.py
--rw-rw-rw-   0        0        0     2616 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/window.py
--rw-rw-rw-   0        0        0     4179 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/zoomheight.py
--rw-rw-rw-   0        0        0     2005 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/idlelib/zzdummy.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.224985 idcn-1.0.1/idcn/releases/3.12/turtledemo/
--rw-rw-rw-   0        0        0      316 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/__init__.py
--rw-rw-rw-   0        0        0    15155 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/__main__.py
--rw-rw-rw-   0        0        0      160 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/turtle.cfg
--rw-rw-rw-   0        0        0     3405 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/分形曲线.py
--rw-rw-rw-   0        0        0     1117 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/双画布.py
--rw-rw-rw-   0        0        0     1068 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/和平旗.py
--rw-rw-rw-   0        0        0     4172 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/字节设计.py
--rw-rw-rw-   0        0        0     3386 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/平铺图案.py
--rw-rw-rw-   0        0        0     6520 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/拿火柴.py
--rw-rw-rw-   0        0        0     5018 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/排序动画.py
--rw-rw-rw-   0        0        0     3124 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/时钟.py
--rw-rw-rw-   0        0        0     1999 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/极简汉诺塔.py
--rw-rw-rw-   0        0        0     2412 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/林登麦伊尔.py
--rw-rw-rw-   0        0        0     1338 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/树.py
--rw-rw-rw-   0        0        0     3020 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/森林.py
--rw-rw-rw-   0        0        0      949 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/混乱.py
--rw-rw-rw-   0        0        0     1204 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/画图.py
--rw-rw-rw-   0        0        0     1306 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/花形.py
--rw-rw-rw-   0        0        0     2741 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/行星系统.py
--rw-rw-rw-   0        0        0     1706 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/跳舞.py
--rw-rw-rw-   0        0        0      793 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/阴阳.py
--rw-rw-rw-   0        0        0     1356 2024-05-27 14:55:05.000000 idcn-1.0.1/idcn/releases/3.12/turtledemo/颜色混合器.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.887440 idcn-1.0.1/idcn/releases/3.13/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.269220 idcn-1.0.1/idcn/releases/3.13/idlelib/
--rw-rw-rw-   0        0        0     2152 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/CREDITS.txt
--rw-rw-rw-   0        0        0    56360 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/ChangeLog
--rw-rw-rw-   0        0        0    10312 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/HISTORY.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.277915 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/
--rw-rw-rw-   0        0        0      443 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/README.txt
--rw-rw-rw-   0        0        0      120 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/folder.gif
--rw-rw-rw-   0        0        0    57746 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle.ico
--rw-rw-rw-   0        0        0      634 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_16.gif
--rw-rw-rw-   0        0        0     1031 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    39205 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     1019 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_32.gif
--rw-rw-rw-   0        0        0     2036 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     1388 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_48.gif
--rw-rw-rw-   0        0        0     3977 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_48.png
--rw-rw-rw-   0        0        0       75 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/minusnode.gif
--rw-rw-rw-   0        0        0      125 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/openfolder.gif
--rw-rw-rw-   0        0        0       78 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/plusnode.gif
--rw-rw-rw-   0        0        0      380 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/python.gif
--rw-rw-rw-   0        0        0       72 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/tk.gif
--rw-rw-rw-   0        0        0    27172 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/NEWS2x.txt
--rw-rw-rw-   0        0        0    55574 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/News3.txt
--rw-rw-rw-   0        0        0    11653 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/README.txt
--rw-rw-rw-   0        0        0     8478 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/TODO.txt
--rw-rw-rw-   0        0        0      396 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/__main__.py
--rw-rw-rw-   0        0        0     9354 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/autocomplete.py
--rw-rw-rw-   0        0        0    20863 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/autocomplete_w.py
--rw-rw-rw-   0        0        0     3216 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/autoexpand.py
--rw-rw-rw-   0        0        0     8590 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/browser.py
--rw-rw-rw-   0        0        0     7265 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/calltip.py
--rw-rw-rw-   0        0        0     7083 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/calltip_w.py
--rw-rw-rw-   0        0        0    11429 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/codecontext.py
--rw-rw-rw-   0        0        0    14783 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/colorizer.py
--rw-rw-rw-   0        0        0     2266 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/config-extensions.def
--rw-rw-rw-   0        0        0     2868 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/config-highlight.def
--rw-rw-rw-   0        0        0    10906 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/config-keys.def
--rw-rw-rw-   0        0        0     3167 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/config-main.def
--rw-rw-rw-   0        0        0    38429 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/config.py
--rw-rw-rw-   0        0        0    14978 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/config_key.py
--rw-rw-rw-   0        0        0   105344 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/configdialog.py
--rw-rw-rw-   0        0        0    21073 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/debugger.py
--rw-rw-rw-   0        0        0    12118 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/debugger_r.py
--rw-rw-rw-   0        0        0     4177 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/debugobj.py
--rw-rw-rw-   0        0        0     1082 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/debugobj_r.py
--rw-rw-rw-   0        0        0     1044 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/delegator.py
--rw-rw-rw-   0        0        0     1993 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/dynoption.py
--rw-rw-rw-   0        0        0    72225 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/editor.py
--rw-rw-rw-   0        0        0     3631 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/extend.txt
--rw-rw-rw-   0        0        0     3870 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/filelist.py
--rw-rw-rw-   0        0        0    15825 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/format.py
--rw-rw-rw-   0        0        0     7512 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/grep.py
--rw-rw-rw-   0        0        0    78525 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/help.html
--rw-rw-rw-   0        0        0    11980 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/help.py
--rw-rw-rw-   0        0        0     8929 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/help_about.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/history.py
--rw-rw-rw-   0        0        0    12889 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/hyperparser.py
--rwxrwxrwx   0        0        0      173 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle.bat
--rw-rw-rw-   0        0        0      454 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle.py
--rw-rw-rw-   0        0        0      570 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle.pyw
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.321178 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/
--rw-rw-rw-   0        0        0     8880 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/README.txt
--rw-rw-rw-   0        0        0     1250 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/example_noext
--rw-rw-rw-   0        0        0      154 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/example_stub.pyi
--rw-rw-rw-   0        0        0    15313 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/htest.py
--rw-rw-rw-   0        0        0     1943 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/mock_idle.py
--rw-rw-rw-   0        0        0    11693 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/mock_tk.py
--rw-rw-rw-   0        0        0      642 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/template.py
--rw-rw-rw-   0        0        0    11093 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_autocomplete.py
--rw-rw-rw-   0        0        0      720 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_autocomplete_w.py
--rw-rw-rw-   0        0        0     4638 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_autoexpand.py
--rw-rw-rw-   0        0        0     8420 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_browser.py
--rw-rw-rw-   0        0        0    13658 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_calltip.py
--rw-rw-rw-   0        0        0      686 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_calltip_w.py
--rw-rw-rw-   0        0        0    16082 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_codecontext.py
--rw-rw-rw-   0        0        0    22882 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_colorizer.py
--rw-rw-rw-   0        0        0    32091 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_config.py
--rw-rw-rw-   0        0        0    11462 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_config_key.py
--rw-rw-rw-   0        0        0    55389 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_configdialog.py
--rw-rw-rw-   0        0        0     9727 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugger.py
--rw-rw-rw-   0        0        0      965 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugger_r.py
--rw-rw-rw-   0        0        0     1611 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugobj.py
--rw-rw-rw-   0        0        0      545 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugobj_r.py
--rw-rw-rw-   0        0        0     1567 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_delegator.py
--rw-rw-rw-   0        0        0     2564 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_editmenu.py
--rw-rw-rw-   0        0        0     8151 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_editor.py
--rw-rw-rw-   0        0        0      795 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_filelist.py
--rw-rw-rw-   0        0        0    23610 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_format.py
--rw-rw-rw-   0        0        0     5072 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_grep.py
--rw-rw-rw-   0        0        0      863 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_help.py
--rw-rw-rw-   0        0        0     5904 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_help_about.py
--rw-rw-rw-   0        0        0     5517 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_history.py
--rw-rw-rw-   0        0        0     9082 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_hyperparser.py
--rw-rw-rw-   0        0        0     2457 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_iomenu.py
--rw-rw-rw-   0        0        0     3444 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_macosx.py
--rw-rw-rw-   0        0        0     1638 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_mainmenu.py
--rw-rw-rw-   0        0        0     1317 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_multicall.py
--rw-rw-rw-   0        0        0     5417 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_outwin.py
--rw-rw-rw-   0        0        0     3544 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_parenmatch.py
--rw-rw-rw-   0        0        0     2422 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_pathbrowser.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_percolator.py
--rw-rw-rw-   0        0        0    19365 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_pyparse.py
--rw-rw-rw-   0        0        0     4965 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_pyshell.py
--rw-rw-rw-   0        0        0    15454 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_query.py
--rw-rw-rw-   0        0        0     4176 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_redirector.py
--rw-rw-rw-   0        0        0     8299 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_replace.py
--rw-rw-rw-   0        0        0      805 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_rpc.py
--rw-rw-rw-   0        0        0    15851 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_run.py
--rw-rw-rw-   0        0        0      777 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_runscript.py
--rw-rw-rw-   0        0        0      496 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_scrolledlist.py
--rw-rw-rw-   0        0        0     2459 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_search.py
--rw-rw-rw-   0        0        0     5691 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_searchbase.py
--rw-rw-rw-   0        0        0    11588 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_searchengine.py
--rw-rw-rw-   0        0        0    26854 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_sidebar.py
--rw-rw-rw-   0        0        0    19656 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_squeezer.py
--rw-rw-rw-   0        0        0      991 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_stackviewer.py
--rw-rw-rw-   0        0        0     1133 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_statusbar.py
--rw-rw-rw-   0        0        0     6970 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_text.py
--rw-rw-rw-   0        0        0     7364 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_textview.py
--rw-rw-rw-   0        0        0     5385 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_tooltip.py
--rw-rw-rw-   0        0        0     1752 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_tree.py
--rw-rw-rw-   0        0        0     4228 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_undo.py
--rw-rw-rw-   0        0        0      308 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_util.py
--rw-rw-rw-   0        0        0     2740 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_warning.py
--rw-rw-rw-   0        0        0     1075 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_window.py
--rw-rw-rw-   0        0        0      999 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_zoomheight.py
--rw-rw-rw-   0        0        0     4455 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_zzdummy.py
--rw-rw-rw-   0        0        0     2333 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/tkinter_testing_utils.py
--rw-rw-rw-   0        0        0    16289 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/iomenu.py
--rw-rw-rw-   0        0        0     9269 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/macosx.py
--rw-rw-rw-   0        0        0     4118 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/mainmenu.py
--rw-rw-rw-   0        0        0    18652 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/multicall.py
--rw-rw-rw-   0        0        0     5663 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/outwin.py
--rw-rw-rw-   0        0        0     7204 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/parenmatch.py
--rw-rw-rw-   0        0        0     3098 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/pathbrowser.py
--rw-rw-rw-   0        0        0     3568 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/percolator.py
--rw-rw-rw-   0        0        0    19864 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/pyparse.py
--rw-rw-rw-   0        0        0    62241 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/pyshell.py
--rw-rw-rw-   0        0        0    15138 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/query.py
--rw-rw-rw-   0        0        0     6832 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/redirector.py
--rw-rw-rw-   0        0        0     9784 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/replace.py
--rw-rw-rw-   0        0        0    21071 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/rpc.py
--rw-rw-rw-   0        0        0    21375 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/run.py
--rw-rw-rw-   0        0        0     8278 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/runscript.py
--rw-rw-rw-   0        0        0     4477 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/scrolledlist.py
--rw-rw-rw-   0        0        0     5573 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/search.py
--rw-rw-rw-   0        0        0     7859 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/searchbase.py
--rw-rw-rw-   0        0        0     7366 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/searchengine.py
--rw-rw-rw-   0        0        0    20330 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/sidebar.py
--rw-rw-rw-   0        0        0    12845 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/squeezer.py
--rw-rw-rw-   0        0        0     4016 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/stackviewer.py
--rw-rw-rw-   0        0        0     1474 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/statusbar.py
--rw-rw-rw-   0        0        0     6812 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/textview.py
--rw-rw-rw-   0        0        0     6471 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/tooltip.py
--rw-rw-rw-   0        0        0    16556 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/tree.py
--rw-rw-rw-   0        0        0    11016 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/undo.py
--rw-rw-rw-   0        0        0     1312 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/util.py
--rw-rw-rw-   0        0        0     2616 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/window.py
--rw-rw-rw-   0        0        0     4179 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/zoomheight.py
--rw-rw-rw-   0        0        0     2005 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/idlelib/zzdummy.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.334175 idcn-1.0.1/idcn/releases/3.13/turtledemo/
--rw-rw-rw-   0        0        0      316 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/__init__.py
--rw-rw-rw-   0        0        0    15155 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/__main__.py
--rw-rw-rw-   0        0        0      160 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/turtle.cfg
--rw-rw-rw-   0        0        0     3405 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/分形曲线.py
--rw-rw-rw-   0        0        0     1117 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/双画布.py
--rw-rw-rw-   0        0        0     1068 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/和平旗.py
--rw-rw-rw-   0        0        0     4172 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/字节设计.py
--rw-rw-rw-   0        0        0     3386 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/平铺图案.py
--rw-rw-rw-   0        0        0     6520 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/拿火柴.py
--rw-rw-rw-   0        0        0     5018 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/排序动画.py
--rw-rw-rw-   0        0        0     3124 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/时钟.py
--rw-rw-rw-   0        0        0     1999 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/极简汉诺塔.py
--rw-rw-rw-   0        0        0     2412 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/林登麦伊尔.py
--rw-rw-rw-   0        0        0     1338 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/树.py
--rw-rw-rw-   0        0        0     3020 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/森林.py
--rw-rw-rw-   0        0        0      949 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/混乱.py
--rw-rw-rw-   0        0        0     1204 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/画图.py
--rw-rw-rw-   0        0        0     1306 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/花形.py
--rw-rw-rw-   0        0        0     2741 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/行星系统.py
--rw-rw-rw-   0        0        0     1706 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/跳舞.py
--rw-rw-rw-   0        0        0      793 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/阴阳.py
--rw-rw-rw-   0        0        0     1356 2024-05-27 14:55:04.000000 idcn-1.0.1/idcn/releases/3.13/turtledemo/颜色混合器.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.888463 idcn-1.0.1/idcn/releases/3.8/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.377974 idcn-1.0.1/idcn/releases/3.8/idlelib/
--rw-rw-rw-   0        0        0     1866 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/CREDITS.txt
--rw-rw-rw-   0        0        0    56360 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/ChangeLog
--rw-rw-rw-   0        0        0    10312 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/HISTORY.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.386623 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/
--rw-rw-rw-   0        0        0      443 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/README.txt
--rw-rw-rw-   0        0        0      120 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/folder.gif
--rw-rw-rw-   0        0        0    57746 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle.ico
--rw-rw-rw-   0        0        0     1034 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_16.gif
--rw-rw-rw-   0        0        0     1264 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    42839 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     1435 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_32.gif
--rw-rw-rw-   0        0        0     2542 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     1388 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_48.gif
--rw-rw-rw-   0        0        0     4710 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_48.png
--rw-rw-rw-   0        0        0       96 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/minusnode.gif
--rw-rw-rw-   0        0        0      125 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/openfolder.gif
--rw-rw-rw-   0        0        0       79 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/plusnode.gif
--rw-rw-rw-   0        0        0      585 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/python.gif
--rw-rw-rw-   0        0        0       85 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/tk.gif
--rw-rw-rw-   0        0        0    50808 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/NEWS.txt
--rw-rw-rw-   0        0        0    27172 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/NEWS2x.txt
--rw-rw-rw-   0        0        0     9599 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/README.txt
--rw-rw-rw-   0        0        0     8478 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/TODO.txt
--rw-rw-rw-   0        0        0      396 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/__main__.py
--rw-rw-rw-   0        0        0     9150 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/autocomplete.py
--rw-rw-rw-   0        0        0    20109 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/autocomplete_w.py
--rw-rw-rw-   0        0        0     3216 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/autoexpand.py
--rw-rw-rw-   0        0        0     8316 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/browser.py
--rw-rw-rw-   0        0        0     7265 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/calltip.py
--rw-rw-rw-   0        0        0     7158 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/calltip_w.py
--rw-rw-rw-   0        0        0    11429 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/codecontext.py
--rw-rw-rw-   0        0        0    13201 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/colorizer.py
--rw-rw-rw-   0        0        0     2266 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/config-extensions.def
--rw-rw-rw-   0        0        0     2868 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/config-highlight.def
--rw-rw-rw-   0        0        0    10906 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/config-keys.def
--rw-rw-rw-   0        0        0     3167 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/config-main.def
--rw-rw-rw-   0        0        0    38200 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/config.py
--rw-rw-rw-   0        0        0    14288 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/config_key.py
--rw-rw-rw-   0        0        0   105087 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/configdialog.py
--rw-rw-rw-   0        0        0    19186 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/debugger.py
--rw-rw-rw-   0        0        0    12170 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/debugger_r.py
--rw-rw-rw-   0        0        0     4055 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/debugobj.py
--rw-rw-rw-   0        0        0     1082 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/debugobj_r.py
--rw-rw-rw-   0        0        0     1043 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/delegator.py
--rw-rw-rw-   0        0        0     2017 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/dynoption.py
--rw-rw-rw-   0        0        0    68360 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/editor.py
--rw-rw-rw-   0        0        0     3631 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/extend.txt
--rw-rw-rw-   0        0        0     3875 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/filelist.py
--rw-rw-rw-   0        0        0    15825 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/format.py
--rw-rw-rw-   0        0        0     7465 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/grep.py
--rw-rw-rw-   0        0        0    68324 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/help.html
--rw-rw-rw-   0        0        0    11859 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/help.py
--rw-rw-rw-   0        0        0     8998 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/help_about.py
--rw-rw-rw-   0        0        0     4043 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/history.py
--rw-rw-rw-   0        0        0    12883 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/hyperparser.py
--rwxrwxrwx   0        0        0      173 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle.bat
--rw-rw-rw-   0        0        0      454 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle.py
--rw-rw-rw-   0        0        0      570 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle.pyw
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.426273 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/
--rw-rw-rw-   0        0        0     8729 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/README.txt
--rw-rw-rw-   0        0        0      712 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/__init__.py
--rw-rw-rw-   0        0        0    15190 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/htest.py
--rw-rw-rw-   0        0        0     1943 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/mock_idle.py
--rw-rw-rw-   0        0        0    11692 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/mock_tk.py
--rw-rw-rw-   0        0        0      642 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/template.py
--rw-rw-rw-   0        0        0    10904 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_autocomplete.py
--rw-rw-rw-   0        0        0      709 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_autocomplete_w.py
--rw-rw-rw-   0        0        0     4638 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_autoexpand.py
--rw-rw-rw-   0        0        0     7963 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_browser.py
--rw-rw-rw-   0        0        0    13193 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_calltip.py
--rw-rw-rw-   0        0        0      686 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_calltip_w.py
--rw-rw-rw-   0        0        0    16082 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_codecontext.py
--rw-rw-rw-   0        0        0    15017 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_colorizer.py
--rw-rw-rw-   0        0        0    32046 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_config.py
--rw-rw-rw-   0        0        0     9709 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_config_key.py
--rw-rw-rw-   0        0        0    54344 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_configdialog.py
--rw-rw-rw-   0        0        0      571 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugger.py
--rw-rw-rw-   0        0        0     1009 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugger_r.py
--rw-rw-rw-   0        0        0     1561 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugobj.py
--rw-rw-rw-   0        0        0      545 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugobj_r.py
--rw-rw-rw-   0        0        0     1567 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_delegator.py
--rw-rw-rw-   0        0        0     2564 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_editmenu.py
--rw-rw-rw-   0        0        0     7523 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_editor.py
--rw-rw-rw-   0        0        0      795 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_filelist.py
--rw-rw-rw-   0        0        0    23610 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_format.py
--rw-rw-rw-   0        0        0     5072 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_grep.py
--rw-rw-rw-   0        0        0      849 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_help.py
--rw-rw-rw-   0        0        0     5919 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_help_about.py
--rw-rw-rw-   0        0        0     5517 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_history.py
--rw-rw-rw-   0        0        0     9082 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_hyperparser.py
--rw-rw-rw-   0        0        0     1278 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_iomenu.py
--rw-rw-rw-   0        0        0     3309 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_macosx.py
--rw-rw-rw-   0        0        0     1638 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_mainmenu.py
--rw-rw-rw-   0        0        0     1316 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_multicall.py
--rw-rw-rw-   0        0        0     5422 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_outwin.py
--rw-rw-rw-   0        0        0     3550 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_parenmatch.py
--rw-rw-rw-   0        0        0     2422 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_pathbrowser.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_percolator.py
--rw-rw-rw-   0        0        0    19364 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_pyparse.py
--rw-rw-rw-   0        0        0     2171 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_pyshell.py
--rw-rw-rw-   0        0        0    15450 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_query.py
--rw-rw-rw-   0        0        0     4176 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_redirector.py
--rw-rw-rw-   0        0        0     8299 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_replace.py
--rw-rw-rw-   0        0        0      805 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_rpc.py
--rw-rw-rw-   0        0        0    13983 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_run.py
--rw-rw-rw-   0        0        0      777 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_runscript.py
--rw-rw-rw-   0        0        0      496 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_scrolledlist.py
--rw-rw-rw-   0        0        0     2459 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_search.py
--rw-rw-rw-   0        0        0     5691 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_searchbase.py
--rw-rw-rw-   0        0        0    11588 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_searchengine.py
--rw-rw-rw-   0        0        0    13231 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_sidebar.py
--rw-rw-rw-   0        0        0    20108 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_squeezer.py
--rw-rw-rw-   0        0        0     1206 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_stackviewer.py
--rw-rw-rw-   0        0        0     1133 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_statusbar.py
--rw-rw-rw-   0        0        0     6978 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_text.py
--rw-rw-rw-   0        0        0     7364 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_textview.py
--rw-rw-rw-   0        0        0     5385 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_tooltip.py
--rw-rw-rw-   0        0        0     1752 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_tree.py
--rw-rw-rw-   0        0        0     4228 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_undo.py
--rw-rw-rw-   0        0        0     2740 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_warning.py
--rw-rw-rw-   0        0        0     1075 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_window.py
--rw-rw-rw-   0        0        0      999 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_zoomheight.py
--rw-rw-rw-   0        0        0     4457 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_zzdummy.py
--rw-rw-rw-   0        0        0    15863 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/iomenu.py
--rw-rw-rw-   0        0        0     9641 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/macosx.py
--rw-rw-rw-   0        0        0     4109 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/mainmenu.py
--rw-rw-rw-   0        0        0    18648 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/multicall.py
--rw-rw-rw-   0        0        0     5657 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/outwin.py
--rw-rw-rw-   0        0        0     7204 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/parenmatch.py
--rw-rw-rw-   0        0        0     3198 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/pathbrowser.py
--rw-rw-rw-   0        0        0     3130 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/percolator.py
--rw-rw-rw-   0        0        0    19947 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/pyparse.py
--rw-rw-rw-   0        0        0    57468 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/pyshell.py
--rw-rw-rw-   0        0        0    15142 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/query.py
--rw-rw-rw-   0        0        0     6875 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/redirector.py
--rw-rw-rw-   0        0        0     9875 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/replace.py
--rw-rw-rw-   0        0        0    21069 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/rpc.py
--rw-rw-rw-   0        0        0    20855 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/run.py
--rw-rw-rw-   0        0        0     8278 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/runscript.py
--rw-rw-rw-   0        0        0     4464 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/scrolledlist.py
--rw-rw-rw-   0        0        0     5572 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/search.py
--rw-rw-rw-   0        0        0     7859 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/searchbase.py
--rw-rw-rw-   0        0        0     7356 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/searchengine.py
--rw-rw-rw-   0        0        0    13585 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/sidebar.py
--rw-rw-rw-   0        0        0    12836 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/squeezer.py
--rw-rw-rw-   0        0        0     4454 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/stackviewer.py
--rw-rw-rw-   0        0        0     1472 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/statusbar.py
--rw-rw-rw-   0        0        0     6817 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/textview.py
--rw-rw-rw-   0        0        0     6557 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/tooltip.py
--rw-rw-rw-   0        0        0    16443 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/tree.py
--rw-rw-rw-   0        0        0    11046 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/undo.py
--rw-rw-rw-   0        0        0     2616 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/window.py
--rw-rw-rw-   0        0        0     4179 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/zoomheight.py
--rw-rw-rw-   0        0        0     2005 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/idlelib/zzdummy.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.438713 idcn-1.0.1/idcn/releases/3.8/turtledemo/
--rw-rw-rw-   0        0        0      316 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/__init__.py
--rw-rw-rw-   0        0        0    14040 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/__main__.py
--rw-rw-rw-   0        0        0      160 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/turtle.cfg
--rw-rw-rw-   0        0        0     3405 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/分形曲线.py
--rw-rw-rw-   0        0        0     1117 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/双画布.py
--rw-rw-rw-   0        0        0     1068 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/和平旗.py
--rw-rw-rw-   0        0        0     4172 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/字节设计.py
--rw-rw-rw-   0        0        0     3386 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/平铺图案.py
--rw-rw-rw-   0        0        0     6520 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/拿火柴.py
--rw-rw-rw-   0        0        0     5018 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/排序动画.py
--rw-rw-rw-   0        0        0     3145 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/时钟.py
--rw-rw-rw-   0        0        0     1999 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/极简汉诺塔.py
--rw-rw-rw-   0        0        0     2412 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/林登麦伊尔.py
--rw-rw-rw-   0        0        0     1338 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/树.py
--rw-rw-rw-   0        0        0     3020 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/森林.py
--rw-rw-rw-   0        0        0      949 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/混乱.py
--rw-rw-rw-   0        0        0     1204 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/画图.py
--rw-rw-rw-   0        0        0     1306 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/花形.py
--rw-rw-rw-   0        0        0     2741 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/行星系统.py
--rw-rw-rw-   0        0        0     1706 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/跳舞.py
--rw-rw-rw-   0        0        0      793 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/阴阳.py
--rw-rw-rw-   0        0        0     1356 2024-05-27 14:55:11.000000 idcn-1.0.1/idcn/releases/3.8/turtledemo/颜色混合器.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:04.888463 idcn-1.0.1/idcn/releases/3.9/
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.484028 idcn-1.0.1/idcn/releases/3.9/idlelib/
--rw-rw-rw-   0        0        0     1866 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/CREDITS.txt
--rw-rw-rw-   0        0        0    56360 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/ChangeLog
--rw-rw-rw-   0        0        0    10312 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/HISTORY.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.493031 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/
--rw-rw-rw-   0        0        0      443 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/README.txt
--rw-rw-rw-   0        0        0      120 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/folder.gif
--rw-rw-rw-   0        0        0    57746 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle.ico
--rw-rw-rw-   0        0        0      634 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_16.gif
--rw-rw-rw-   0        0        0     1031 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    39205 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     1019 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_32.gif
--rw-rw-rw-   0        0        0     2036 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     1388 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_48.gif
--rw-rw-rw-   0        0        0     3977 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_48.png
--rw-rw-rw-   0        0        0       75 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/minusnode.gif
--rw-rw-rw-   0        0        0      125 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/openfolder.gif
--rw-rw-rw-   0        0        0       78 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/plusnode.gif
--rw-rw-rw-   0        0        0      380 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/python.gif
--rw-rw-rw-   0        0        0       72 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/tk.gif
--rw-rw-rw-   0        0        0    51948 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/NEWS.txt
--rw-rw-rw-   0        0        0    27172 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/NEWS2x.txt
--rw-rw-rw-   0        0        0     9680 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/README.txt
--rw-rw-rw-   0        0        0     8478 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/TODO.txt
--rw-rw-rw-   0        0        0      396 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/__init__.py
--rw-rw-rw-   0        0        0      159 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/__main__.py
--rw-rw-rw-   0        0        0     9150 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/autocomplete.py
--rw-rw-rw-   0        0        0    20981 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/autocomplete_w.py
--rw-rw-rw-   0        0        0     3216 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/autoexpand.py
--rw-rw-rw-   0        0        0     8316 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/browser.py
--rw-rw-rw-   0        0        0     7265 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/calltip.py
--rw-rw-rw-   0        0        0     7158 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/calltip_w.py
--rw-rw-rw-   0        0        0    11429 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/codecontext.py
--rw-rw-rw-   0        0        0    13201 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/colorizer.py
--rw-rw-rw-   0        0        0     2266 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/config-extensions.def
--rw-rw-rw-   0        0        0     2868 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/config-highlight.def
--rw-rw-rw-   0        0        0    10906 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/config-keys.def
--rw-rw-rw-   0        0        0     3167 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/config-main.def
--rw-rw-rw-   0        0        0    38200 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/config.py
--rw-rw-rw-   0        0        0    14288 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/config_key.py
--rw-rw-rw-   0        0        0   105765 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/configdialog.py
--rw-rw-rw-   0        0        0    19186 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/debugger.py
--rw-rw-rw-   0        0        0    12170 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/debugger_r.py
--rw-rw-rw-   0        0        0     4055 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/debugobj.py
--rw-rw-rw-   0        0        0     1082 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/debugobj_r.py
--rw-rw-rw-   0        0        0     1043 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/delegator.py
--rw-rw-rw-   0        0        0     2017 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/dynoption.py
--rw-rw-rw-   0        0        0    68397 2024-05-27 14:55:10.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/editor.py
--rw-rw-rw-   0        0        0     3631 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/extend.txt
--rw-rw-rw-   0        0        0     3875 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/filelist.py
--rw-rw-rw-   0        0        0    15825 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/format.py
--rw-rw-rw-   0        0        0     7465 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/grep.py
--rw-rw-rw-   0        0        0    68554 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/help.html
--rw-rw-rw-   0        0        0    11859 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/help.py
--rw-rw-rw-   0        0        0     9101 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/help_about.py
--rw-rw-rw-   0        0        0     4043 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/history.py
--rw-rw-rw-   0        0        0    12883 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/hyperparser.py
--rwxrwxrwx   0        0        0      173 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle.bat
--rw-rw-rw-   0        0        0      454 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle.py
--rw-rw-rw-   0        0        0      570 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle.pyw
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.533227 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/
--rw-rw-rw-   0        0        0     8729 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/README.txt
--rw-rw-rw-   0        0        0      712 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/__init__.py
--rw-rw-rw-   0        0        0       68 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/example_noext
--rw-rw-rw-   0        0        0       87 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/example_stub.pyi
--rw-rw-rw-   0        0        0    15199 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/htest.py
--rw-rw-rw-   0        0        0     1943 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/mock_idle.py
--rw-rw-rw-   0        0        0    11693 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/mock_tk.py
--rw-rw-rw-   0        0        0      642 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/template.py
--rw-rw-rw-   0        0        0    10904 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_autocomplete.py
--rw-rw-rw-   0        0        0      709 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_autocomplete_w.py
--rw-rw-rw-   0        0        0     4638 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_autoexpand.py
--rw-rw-rw-   0        0        0     7963 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_browser.py
--rw-rw-rw-   0        0        0    13194 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_calltip.py
--rw-rw-rw-   0        0        0      686 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_calltip_w.py
--rw-rw-rw-   0        0        0    16082 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_codecontext.py
--rw-rw-rw-   0        0        0    15017 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_colorizer.py
--rw-rw-rw-   0        0        0    32046 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_config.py
--rw-rw-rw-   0        0        0     9708 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_config_key.py
--rw-rw-rw-   0        0        0    55344 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_configdialog.py
--rw-rw-rw-   0        0        0      571 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugger.py
--rw-rw-rw-   0        0        0     1009 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugger_r.py
--rw-rw-rw-   0        0        0     1561 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugobj.py
--rw-rw-rw-   0        0        0      545 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugobj_r.py
--rw-rw-rw-   0        0        0     1567 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_delegator.py
--rw-rw-rw-   0        0        0     2564 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_editmenu.py
--rw-rw-rw-   0        0        0     7523 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_editor.py
--rw-rw-rw-   0        0        0      795 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_filelist.py
--rw-rw-rw-   0        0        0    23610 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_format.py
--rw-rw-rw-   0        0        0     5072 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_grep.py
--rw-rw-rw-   0        0        0      849 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_help.py
--rw-rw-rw-   0        0        0     5919 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_help_about.py
--rw-rw-rw-   0        0        0     5517 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_history.py
--rw-rw-rw-   0        0        0     9082 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_hyperparser.py
--rw-rw-rw-   0        0        0     1908 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_iomenu.py
--rw-rw-rw-   0        0        0     3444 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_macosx.py
--rw-rw-rw-   0        0        0     1638 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_mainmenu.py
--rw-rw-rw-   0        0        0     1317 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_multicall.py
--rw-rw-rw-   0        0        0     5422 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_outwin.py
--rw-rw-rw-   0        0        0     3550 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_parenmatch.py
--rw-rw-rw-   0        0        0     2422 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_pathbrowser.py
--rw-rw-rw-   0        0        0     4065 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_percolator.py
--rw-rw-rw-   0        0        0    19365 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_pyparse.py
--rw-rw-rw-   0        0        0     2171 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_pyshell.py
--rw-rw-rw-   0        0        0    15454 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_query.py
--rw-rw-rw-   0        0        0     4176 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_redirector.py
--rw-rw-rw-   0        0        0     8299 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_replace.py
--rw-rw-rw-   0        0        0      805 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_rpc.py
--rw-rw-rw-   0        0        0    13983 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_run.py
--rw-rw-rw-   0        0        0      777 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_runscript.py
--rw-rw-rw-   0        0        0      496 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_scrolledlist.py
--rw-rw-rw-   0        0        0     2459 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_search.py
--rw-rw-rw-   0        0        0     5691 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_searchbase.py
--rw-rw-rw-   0        0        0    11588 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_searchengine.py
--rw-rw-rw-   0        0        0    13231 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_sidebar.py
--rw-rw-rw-   0        0        0    20108 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_squeezer.py
--rw-rw-rw-   0        0        0     1206 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_stackviewer.py
--rw-rw-rw-   0        0        0     1133 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_statusbar.py
--rw-rw-rw-   0        0        0     6978 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_text.py
--rw-rw-rw-   0        0        0     7364 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_textview.py
--rw-rw-rw-   0        0        0     5385 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_tooltip.py
--rw-rw-rw-   0        0        0     1752 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_tree.py
--rw-rw-rw-   0        0        0     4228 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_undo.py
--rw-rw-rw-   0        0        0      308 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_util.py
--rw-rw-rw-   0        0        0     2740 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_warning.py
--rw-rw-rw-   0        0        0     1075 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_window.py
--rw-rw-rw-   0        0        0      999 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_zoomheight.py
--rw-rw-rw-   0        0        0     4457 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_zzdummy.py
--rw-rw-rw-   0        0        0    15963 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/iomenu.py
--rw-rw-rw-   0        0        0     9642 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/macosx.py
--rw-rw-rw-   0        0        0     4109 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/mainmenu.py
--rw-rw-rw-   0        0        0    18648 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/multicall.py
--rw-rw-rw-   0        0        0     5657 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/outwin.py
--rw-rw-rw-   0        0        0     7204 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/parenmatch.py
--rw-rw-rw-   0        0        0     3198 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/pathbrowser.py
--rw-rw-rw-   0        0        0     3130 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/percolator.py
--rw-rw-rw-   0        0        0    19864 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/pyparse.py
--rw-rw-rw-   0        0        0    57639 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/pyshell.py
--rw-rw-rw-   0        0        0    15146 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/query.py
--rw-rw-rw-   0        0        0     6875 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/redirector.py
--rw-rw-rw-   0        0        0     9785 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/replace.py
--rw-rw-rw-   0        0        0    21069 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/rpc.py
--rw-rw-rw-   0        0        0    20960 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/run.py
--rw-rw-rw-   0        0        0     8278 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/runscript.py
--rw-rw-rw-   0        0        0     4464 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/scrolledlist.py
--rw-rw-rw-   0        0        0     5572 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/search.py
--rw-rw-rw-   0        0        0     7859 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/searchbase.py
--rw-rw-rw-   0        0        0     7356 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/searchengine.py
--rw-rw-rw-   0        0        0    13585 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/sidebar.py
--rw-rw-rw-   0        0        0    12836 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/squeezer.py
--rw-rw-rw-   0        0        0     4454 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/stackviewer.py
--rw-rw-rw-   0        0        0     1472 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/statusbar.py
--rw-rw-rw-   0        0        0     6817 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/textview.py
--rw-rw-rw-   0        0        0     6557 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/tooltip.py
--rw-rw-rw-   0        0        0    16443 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/tree.py
--rw-rw-rw-   0        0        0    11046 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/undo.py
--rw-rw-rw-   0        0        0      721 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/util.py
--rw-rw-rw-   0        0        0     2616 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/window.py
--rw-rw-rw-   0        0        0     4179 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/zoomheight.py
--rw-rw-rw-   0        0        0     2005 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/idlelib/zzdummy.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.544737 idcn-1.0.1/idcn/releases/3.9/turtledemo/
--rw-rw-rw-   0        0        0      316 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/__init__.py
--rw-rw-rw-   0        0        0    14830 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/__main__.py
--rw-rw-rw-   0        0        0      160 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/turtle.cfg
--rw-rw-rw-   0        0        0     3405 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/分形曲线.py
--rw-rw-rw-   0        0        0     1117 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/双画布.py
--rw-rw-rw-   0        0        0     1068 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/和平旗.py
--rw-rw-rw-   0        0        0     4172 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/字节设计.py
--rw-rw-rw-   0        0        0     3386 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/平铺图案.py
--rw-rw-rw-   0        0        0     6520 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/拿火柴.py
--rw-rw-rw-   0        0        0     5018 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/排序动画.py
--rw-rw-rw-   0        0        0     3145 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/时钟.py
--rw-rw-rw-   0        0        0     1999 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/极简汉诺塔.py
--rw-rw-rw-   0        0        0     2412 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/林登麦伊尔.py
--rw-rw-rw-   0        0        0     1338 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/树.py
--rw-rw-rw-   0        0        0     3020 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/森林.py
--rw-rw-rw-   0        0        0      949 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/混乱.py
--rw-rw-rw-   0        0        0     1204 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/画图.py
--rw-rw-rw-   0        0        0     1306 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/花形.py
--rw-rw-rw-   0        0        0     2741 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/行星系统.py
--rw-rw-rw-   0        0        0     1706 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/跳舞.py
--rw-rw-rw-   0        0        0      793 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/阴阳.py
--rw-rw-rw-   0        0        0     1356 2024-05-27 14:55:09.000000 idcn-1.0.1/idcn/releases/3.9/turtledemo/颜色混合器.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:11:05.545736 idcn-1.0.1/idcn.egg-info/
--rw-rw-rw-   0        0        0     2591 2024-05-27 16:11:04.000000 idcn-1.0.1/idcn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    48672 2024-05-27 16:11:04.000000 idcn-1.0.1/idcn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 16:11:04.000000 idcn-1.0.1/idcn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-27 14:55:52.000000 idcn-1.0.1/idcn.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2024-05-27 16:11:04.000000 idcn-1.0.1/idcn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       27 2024-05-27 14:52:13.000000 idcn-1.0.1/idcn.pth
--rw-rw-rw-   0        0        0       42 2024-05-27 16:11:05.546756 idcn-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1926 2024-05-27 16:07:06.000000 idcn-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.831320 idcn-1.1.0/
+-rw-rw-rw-   0        0        0     1065 2024-06-02 13:23:01.000000 idcn-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2591 2024-06-02 13:26:59.830320 idcn-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1424 2024-06-02 13:23:01.000000 idcn-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.176323 idcn-1.1.0/idcn/
+-rw-rw-rw-   0        0        0      247 2024-06-02 13:23:01.000000 idcn-1.1.0/idcn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.172313 idcn-1.1.0/idcn/releases/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.168315 idcn-1.1.0/idcn/releases/3.10/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.222460 idcn-1.1.0/idcn/releases/3.10/idlelib/
+-rw-rw-rw-   0        0        0     2152 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/CREDITS.txt
+-rw-rw-rw-   0        0        0    56360 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/ChangeLog
+-rw-rw-rw-   0        0        0    10312 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/HISTORY.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.231460 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/
+-rw-rw-rw-   0        0        0      443 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/README.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/folder.gif
+-rw-rw-rw-   0        0        0    57746 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle.ico
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_16.gif
+-rw-rw-rw-   0        0        0     1031 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_16.png
+-rw-rw-rw-   0        0        0    39205 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_256.png
+-rw-rw-rw-   0        0        0     1019 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_32.gif
+-rw-rw-rw-   0        0        0     2036 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_32.png
+-rw-rw-rw-   0        0        0     1388 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_48.gif
+-rw-rw-rw-   0        0        0     3977 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_48.png
+-rw-rw-rw-   0        0        0       75 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/minusnode.gif
+-rw-rw-rw-   0        0        0      125 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/openfolder.gif
+-rw-rw-rw-   0        0        0       78 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/plusnode.gif
+-rw-rw-rw-   0        0        0      380 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/python.gif
+-rw-rw-rw-   0        0        0       72 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/tk.gif
+-rw-rw-rw-   0        0        0    54195 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/NEWS.txt
+-rw-rw-rw-   0        0        0    27172 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/NEWS2x.txt
+-rw-rw-rw-   0        0        0    11653 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/README.txt
+-rw-rw-rw-   0        0        0     8478 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/TODO.txt
+-rw-rw-rw-   0        0        0      396 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/__main__.py
+-rw-rw-rw-   0        0        0     9354 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/autocomplete.py
+-rw-rw-rw-   0        0        0    21097 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/autocomplete_w.py
+-rw-rw-rw-   0        0        0     3216 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/autoexpand.py
+-rw-rw-rw-   0        0        0     8588 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/browser.py
+-rw-rw-rw-   0        0        0     7265 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/calltip.py
+-rw-rw-rw-   0        0        0     7158 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/calltip_w.py
+-rw-rw-rw-   0        0        0    11429 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/codecontext.py
+-rw-rw-rw-   0        0        0    14773 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/colorizer.py
+-rw-rw-rw-   0        0        0     2266 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/config-extensions.def
+-rw-rw-rw-   0        0        0     2868 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/config-highlight.def
+-rw-rw-rw-   0        0        0    10906 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/config-keys.def
+-rw-rw-rw-   0        0        0     3167 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/config-main.def
+-rw-rw-rw-   0        0        0    38201 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/config.py
+-rw-rw-rw-   0        0        0    14978 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/config_key.py
+-rw-rw-rw-   0        0        0   105758 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/configdialog.py
+-rw-rw-rw-   0        0        0    19186 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/debugger.py
+-rw-rw-rw-   0        0        0    12170 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/debugger_r.py
+-rw-rw-rw-   0        0        0     4055 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/debugobj.py
+-rw-rw-rw-   0        0        0     1082 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/debugobj_r.py
+-rw-rw-rw-   0        0        0     1043 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/delegator.py
+-rw-rw-rw-   0        0        0     1991 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/dynoption.py
+-rw-rw-rw-   0        0        0    69049 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/editor.py
+-rw-rw-rw-   0        0        0     3631 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/extend.txt
+-rw-rw-rw-   0        0        0     3875 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/filelist.py
+-rw-rw-rw-   0        0        0    15825 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/format.py
+-rw-rw-rw-   0        0        0     7465 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/grep.py
+-rw-rw-rw-   0        0        0    79125 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/help.html
+-rw-rw-rw-   0        0        0    11863 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/help.py
+-rw-rw-rw-   0        0        0     9123 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/help_about.py
+-rw-rw-rw-   0        0        0     4064 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/history.py
+-rw-rw-rw-   0        0        0    12889 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/hyperparser.py
+-rwxrwxrwx   0        0        0      173 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle.bat
+-rw-rw-rw-   0        0        0      454 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle.py
+-rw-rw-rw-   0        0        0      570 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle.pyw
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.273569 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/
+-rw-rw-rw-   0        0        0     8729 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/README.txt
+-rw-rw-rw-   0        0        0      712 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/example_noext
+-rw-rw-rw-   0        0        0       87 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/example_stub.pyi
+-rw-rw-rw-   0        0        0    15199 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/htest.py
+-rw-rw-rw-   0        0        0     1943 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/mock_idle.py
+-rw-rw-rw-   0        0        0    11693 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/mock_tk.py
+-rw-rw-rw-   0        0        0      642 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/template.py
+-rw-rw-rw-   0        0        0    11093 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_autocomplete.py
+-rw-rw-rw-   0        0        0      720 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_autocomplete_w.py
+-rw-rw-rw-   0        0        0     4638 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_autoexpand.py
+-rw-rw-rw-   0        0        0     8420 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_browser.py
+-rw-rw-rw-   0        0        0    13194 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_calltip.py
+-rw-rw-rw-   0        0        0      686 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_calltip_w.py
+-rw-rw-rw-   0        0        0    16082 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_codecontext.py
+-rw-rw-rw-   0        0        0    22882 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_colorizer.py
+-rw-rw-rw-   0        0        0    32046 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_config.py
+-rw-rw-rw-   0        0        0    11462 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_config_key.py
+-rw-rw-rw-   0        0        0    55344 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_configdialog.py
+-rw-rw-rw-   0        0        0      571 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugger.py
+-rw-rw-rw-   0        0        0      965 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugger_r.py
+-rw-rw-rw-   0        0        0     1561 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugobj.py
+-rw-rw-rw-   0        0        0      545 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugobj_r.py
+-rw-rw-rw-   0        0        0     1567 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_delegator.py
+-rw-rw-rw-   0        0        0     2564 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_editmenu.py
+-rw-rw-rw-   0        0        0     7220 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_editor.py
+-rw-rw-rw-   0        0        0      795 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_filelist.py
+-rw-rw-rw-   0        0        0    23610 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_format.py
+-rw-rw-rw-   0        0        0     5072 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_grep.py
+-rw-rw-rw-   0        0        0      849 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_help.py
+-rw-rw-rw-   0        0        0     5919 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_help_about.py
+-rw-rw-rw-   0        0        0     5517 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_history.py
+-rw-rw-rw-   0        0        0     9082 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_hyperparser.py
+-rw-rw-rw-   0        0        0     2194 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_iomenu.py
+-rw-rw-rw-   0        0        0     3444 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_macosx.py
+-rw-rw-rw-   0        0        0     1638 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_mainmenu.py
+-rw-rw-rw-   0        0        0     1317 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_multicall.py
+-rw-rw-rw-   0        0        0     5422 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_outwin.py
+-rw-rw-rw-   0        0        0     3544 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_parenmatch.py
+-rw-rw-rw-   0        0        0     2422 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_pathbrowser.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_percolator.py
+-rw-rw-rw-   0        0        0    19365 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_pyparse.py
+-rw-rw-rw-   0        0        0     4965 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_pyshell.py
+-rw-rw-rw-   0        0        0    15454 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_query.py
+-rw-rw-rw-   0        0        0     4176 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_redirector.py
+-rw-rw-rw-   0        0        0     8299 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_replace.py
+-rw-rw-rw-   0        0        0      805 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_rpc.py
+-rw-rw-rw-   0        0        0    15687 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_run.py
+-rw-rw-rw-   0        0        0      777 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_runscript.py
+-rw-rw-rw-   0        0        0      496 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_scrolledlist.py
+-rw-rw-rw-   0        0        0     2459 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_search.py
+-rw-rw-rw-   0        0        0     5691 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_searchbase.py
+-rw-rw-rw-   0        0        0    11588 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_searchengine.py
+-rw-rw-rw-   0        0        0    26573 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_sidebar.py
+-rw-rw-rw-   0        0        0    19680 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_squeezer.py
+-rw-rw-rw-   0        0        0     1206 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_stackviewer.py
+-rw-rw-rw-   0        0        0     1133 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_statusbar.py
+-rw-rw-rw-   0        0        0     6970 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_text.py
+-rw-rw-rw-   0        0        0     7364 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_textview.py
+-rw-rw-rw-   0        0        0     5385 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_tooltip.py
+-rw-rw-rw-   0        0        0     1752 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_tree.py
+-rw-rw-rw-   0        0        0     4228 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_undo.py
+-rw-rw-rw-   0        0        0      308 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_util.py
+-rw-rw-rw-   0        0        0     2740 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_warning.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_window.py
+-rw-rw-rw-   0        0        0      999 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_zoomheight.py
+-rw-rw-rw-   0        0        0     4455 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_zzdummy.py
+-rw-rw-rw-   0        0        0     2333 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/tkinter_testing_utils.py
+-rw-rw-rw-   0        0        0    16102 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/iomenu.py
+-rw-rw-rw-   0        0        0    10129 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/macosx.py
+-rw-rw-rw-   0        0        0     4118 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/mainmenu.py
+-rw-rw-rw-   0        0        0    18648 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/multicall.py
+-rw-rw-rw-   0        0        0     5657 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/outwin.py
+-rw-rw-rw-   0        0        0     7204 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/parenmatch.py
+-rw-rw-rw-   0        0        0     3198 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/pathbrowser.py
+-rw-rw-rw-   0        0        0     3546 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/percolator.py
+-rw-rw-rw-   0        0        0    19864 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/pyparse.py
+-rw-rw-rw-   0        0        0    63008 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/pyshell.py
+-rw-rw-rw-   0        0        0    15146 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/query.py
+-rw-rw-rw-   0        0        0     6875 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/redirector.py
+-rw-rw-rw-   0        0        0     9985 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/replace.py
+-rw-rw-rw-   0        0        0    21075 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/rpc.py
+-rw-rw-rw-   0        0        0    21418 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/run.py
+-rw-rw-rw-   0        0        0     8278 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/runscript.py
+-rw-rw-rw-   0        0        0     4464 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/scrolledlist.py
+-rw-rw-rw-   0        0        0     5572 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/search.py
+-rw-rw-rw-   0        0        0     7859 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/searchbase.py
+-rw-rw-rw-   0        0        0     7359 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/searchengine.py
+-rw-rw-rw-   0        0        0    20360 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/sidebar.py
+-rw-rw-rw-   0        0        0    12845 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/squeezer.py
+-rw-rw-rw-   0        0        0     4454 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/stackviewer.py
+-rw-rw-rw-   0        0        0     1472 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/statusbar.py
+-rw-rw-rw-   0        0        0     6817 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/textview.py
+-rw-rw-rw-   0        0        0     6557 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/tooltip.py
+-rw-rw-rw-   0        0        0    16443 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/tree.py
+-rw-rw-rw-   0        0        0    11046 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/undo.py
+-rw-rw-rw-   0        0        0      701 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/util.py
+-rw-rw-rw-   0        0        0     2616 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/window.py
+-rw-rw-rw-   0        0        0     4179 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/zoomheight.py
+-rw-rw-rw-   0        0        0     2005 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/idlelib/zzdummy.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.285551 idcn-1.1.0/idcn/releases/3.10/turtledemo/
+-rw-rw-rw-   0        0        0      316 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/__init__.py
+-rw-rw-rw-   0        0        0    14830 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/__main__.py
+-rw-rw-rw-   0        0        0      160 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/turtle.cfg
+-rw-rw-rw-   0        0        0     3405 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/分形曲线.py
+-rw-rw-rw-   0        0        0     1117 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/双画布.py
+-rw-rw-rw-   0        0        0     1068 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/和平旗.py
+-rw-rw-rw-   0        0        0     4172 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/字节设计.py
+-rw-rw-rw-   0        0        0     3386 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/平铺图案.py
+-rw-rw-rw-   0        0        0     6520 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/拿火柴.py
+-rw-rw-rw-   0        0        0     5018 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/排序动画.py
+-rw-rw-rw-   0        0        0     3124 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/时钟.py
+-rw-rw-rw-   0        0        0     1999 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/极简汉诺塔.py
+-rw-rw-rw-   0        0        0     2412 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/林登麦伊尔.py
+-rw-rw-rw-   0        0        0     1338 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/树.py
+-rw-rw-rw-   0        0        0     3020 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/森林.py
+-rw-rw-rw-   0        0        0      949 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/混乱.py
+-rw-rw-rw-   0        0        0     1204 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/画图.py
+-rw-rw-rw-   0        0        0     1306 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/花形.py
+-rw-rw-rw-   0        0        0     2741 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/行星系统.py
+-rw-rw-rw-   0        0        0     1706 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/跳舞.py
+-rw-rw-rw-   0        0        0      793 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/阴阳.py
+-rw-rw-rw-   0        0        0     1356 2024-06-02 13:26:53.000000 idcn-1.1.0/idcn/releases/3.10/turtledemo/颜色混合器.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.170313 idcn-1.1.0/idcn/releases/3.11/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.328909 idcn-1.1.0/idcn/releases/3.11/idlelib/
+-rw-rw-rw-   0        0        0     2152 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/CREDITS.txt
+-rw-rw-rw-   0        0        0    56360 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/ChangeLog
+-rw-rw-rw-   0        0        0    10312 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/HISTORY.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.338302 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/
+-rw-rw-rw-   0        0        0      443 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/README.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/folder.gif
+-rw-rw-rw-   0        0        0    57746 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle.ico
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_16.gif
+-rw-rw-rw-   0        0        0     1031 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_16.png
+-rw-rw-rw-   0        0        0    39205 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_256.png
+-rw-rw-rw-   0        0        0     1019 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_32.gif
+-rw-rw-rw-   0        0        0     2036 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_32.png
+-rw-rw-rw-   0        0        0     1388 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_48.gif
+-rw-rw-rw-   0        0        0     3977 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_48.png
+-rw-rw-rw-   0        0        0       75 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/minusnode.gif
+-rw-rw-rw-   0        0        0      125 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/openfolder.gif
+-rw-rw-rw-   0        0        0       78 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/plusnode.gif
+-rw-rw-rw-   0        0        0      380 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/python.gif
+-rw-rw-rw-   0        0        0       72 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/tk.gif
+-rw-rw-rw-   0        0        0    27172 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/NEWS2x.txt
+-rw-rw-rw-   0        0        0    55422 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/News3.txt
+-rw-rw-rw-   0        0        0    11653 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/README.txt
+-rw-rw-rw-   0        0        0     8478 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/TODO.txt
+-rw-rw-rw-   0        0        0      396 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/__main__.py
+-rw-rw-rw-   0        0        0     9354 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/autocomplete.py
+-rw-rw-rw-   0        0        0    20863 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/autocomplete_w.py
+-rw-rw-rw-   0        0        0     3216 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/autoexpand.py
+-rw-rw-rw-   0        0        0     8590 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/browser.py
+-rw-rw-rw-   0        0        0     7265 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/calltip.py
+-rw-rw-rw-   0        0        0     7083 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/calltip_w.py
+-rw-rw-rw-   0        0        0    11429 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/codecontext.py
+-rw-rw-rw-   0        0        0    14783 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/colorizer.py
+-rw-rw-rw-   0        0        0     2266 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/config-extensions.def
+-rw-rw-rw-   0        0        0     2868 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/config-highlight.def
+-rw-rw-rw-   0        0        0    10906 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/config-keys.def
+-rw-rw-rw-   0        0        0     3167 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/config-main.def
+-rw-rw-rw-   0        0        0    38414 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/config.py
+-rw-rw-rw-   0        0        0    14978 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/config_key.py
+-rw-rw-rw-   0        0        0   105344 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/configdialog.py
+-rw-rw-rw-   0        0        0    21073 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/debugger.py
+-rw-rw-rw-   0        0        0    12118 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/debugger_r.py
+-rw-rw-rw-   0        0        0     4177 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/debugobj.py
+-rw-rw-rw-   0        0        0     1082 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/debugobj_r.py
+-rw-rw-rw-   0        0        0     1044 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/delegator.py
+-rw-rw-rw-   0        0        0     1993 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/dynoption.py
+-rw-rw-rw-   0        0        0    72225 2024-06-02 13:26:52.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/editor.py
+-rw-rw-rw-   0        0        0     3631 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/extend.txt
+-rw-rw-rw-   0        0        0     3870 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/filelist.py
+-rw-rw-rw-   0        0        0    15825 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/format.py
+-rw-rw-rw-   0        0        0     7512 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/grep.py
+-rw-rw-rw-   0        0        0    78525 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/help.html
+-rw-rw-rw-   0        0        0    11911 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/help.py
+-rw-rw-rw-   0        0        0     8929 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/help_about.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/history.py
+-rw-rw-rw-   0        0        0    12889 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/hyperparser.py
+-rwxrwxrwx   0        0        0      173 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle.bat
+-rw-rw-rw-   0        0        0      454 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle.py
+-rw-rw-rw-   0        0        0      570 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle.pyw
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.380458 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/
+-rw-rw-rw-   0        0        0     8880 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/README.txt
+-rw-rw-rw-   0        0        0     1250 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/example_noext
+-rw-rw-rw-   0        0        0      154 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/example_stub.pyi
+-rw-rw-rw-   0        0        0    15313 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/htest.py
+-rw-rw-rw-   0        0        0     1943 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/mock_idle.py
+-rw-rw-rw-   0        0        0    11693 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/mock_tk.py
+-rw-rw-rw-   0        0        0      642 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/template.py
+-rw-rw-rw-   0        0        0    11093 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_autocomplete.py
+-rw-rw-rw-   0        0        0      720 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_autocomplete_w.py
+-rw-rw-rw-   0        0        0     4638 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_autoexpand.py
+-rw-rw-rw-   0        0        0     8420 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_browser.py
+-rw-rw-rw-   0        0        0    13658 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_calltip.py
+-rw-rw-rw-   0        0        0      686 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_calltip_w.py
+-rw-rw-rw-   0        0        0    16082 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_codecontext.py
+-rw-rw-rw-   0        0        0    22882 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_colorizer.py
+-rw-rw-rw-   0        0        0    32091 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_config.py
+-rw-rw-rw-   0        0        0    11462 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_config_key.py
+-rw-rw-rw-   0        0        0    55389 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_configdialog.py
+-rw-rw-rw-   0        0        0     9727 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugger.py
+-rw-rw-rw-   0        0        0      965 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugger_r.py
+-rw-rw-rw-   0        0        0     1611 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugobj.py
+-rw-rw-rw-   0        0        0      545 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugobj_r.py
+-rw-rw-rw-   0        0        0     1567 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_delegator.py
+-rw-rw-rw-   0        0        0     2564 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_editmenu.py
+-rw-rw-rw-   0        0        0     8151 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_editor.py
+-rw-rw-rw-   0        0        0      795 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_filelist.py
+-rw-rw-rw-   0        0        0    23610 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_format.py
+-rw-rw-rw-   0        0        0     5072 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_grep.py
+-rw-rw-rw-   0        0        0      863 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_help.py
+-rw-rw-rw-   0        0        0     5904 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_help_about.py
+-rw-rw-rw-   0        0        0     5517 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_history.py
+-rw-rw-rw-   0        0        0     9082 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_hyperparser.py
+-rw-rw-rw-   0        0        0     2457 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_iomenu.py
+-rw-rw-rw-   0        0        0     3444 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_macosx.py
+-rw-rw-rw-   0        0        0     1638 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_mainmenu.py
+-rw-rw-rw-   0        0        0     1317 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_multicall.py
+-rw-rw-rw-   0        0        0     5417 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_outwin.py
+-rw-rw-rw-   0        0        0     3544 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_parenmatch.py
+-rw-rw-rw-   0        0        0     2422 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_pathbrowser.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_percolator.py
+-rw-rw-rw-   0        0        0    19365 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_pyparse.py
+-rw-rw-rw-   0        0        0     4965 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_pyshell.py
+-rw-rw-rw-   0        0        0    15454 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_query.py
+-rw-rw-rw-   0        0        0     4176 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_redirector.py
+-rw-rw-rw-   0        0        0     8299 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_replace.py
+-rw-rw-rw-   0        0        0      805 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_rpc.py
+-rw-rw-rw-   0        0        0    15687 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_run.py
+-rw-rw-rw-   0        0        0      777 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_runscript.py
+-rw-rw-rw-   0        0        0      496 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_scrolledlist.py
+-rw-rw-rw-   0        0        0     2459 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_search.py
+-rw-rw-rw-   0        0        0     5691 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_searchbase.py
+-rw-rw-rw-   0        0        0    11588 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_searchengine.py
+-rw-rw-rw-   0        0        0    26854 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_sidebar.py
+-rw-rw-rw-   0        0        0    19656 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_squeezer.py
+-rw-rw-rw-   0        0        0      991 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_stackviewer.py
+-rw-rw-rw-   0        0        0     1133 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_statusbar.py
+-rw-rw-rw-   0        0        0     6970 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_text.py
+-rw-rw-rw-   0        0        0     7364 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_textview.py
+-rw-rw-rw-   0        0        0     5385 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_tooltip.py
+-rw-rw-rw-   0        0        0     1752 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_tree.py
+-rw-rw-rw-   0        0        0     4228 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_undo.py
+-rw-rw-rw-   0        0        0      308 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_util.py
+-rw-rw-rw-   0        0        0     2740 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_warning.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_window.py
+-rw-rw-rw-   0        0        0      999 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_zoomheight.py
+-rw-rw-rw-   0        0        0     4455 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_zzdummy.py
+-rw-rw-rw-   0        0        0     2333 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/tkinter_testing_utils.py
+-rw-rw-rw-   0        0        0    16289 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/iomenu.py
+-rw-rw-rw-   0        0        0     9380 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/macosx.py
+-rw-rw-rw-   0        0        0     4118 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/mainmenu.py
+-rw-rw-rw-   0        0        0    18652 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/multicall.py
+-rw-rw-rw-   0        0        0     5663 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/outwin.py
+-rw-rw-rw-   0        0        0     7204 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/parenmatch.py
+-rw-rw-rw-   0        0        0     3098 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/pathbrowser.py
+-rw-rw-rw-   0        0        0     3568 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/percolator.py
+-rw-rw-rw-   0        0        0    19864 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/pyparse.py
+-rw-rw-rw-   0        0        0    62574 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/pyshell.py
+-rw-rw-rw-   0        0        0    15138 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/query.py
+-rw-rw-rw-   0        0        0     6777 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/redirector.py
+-rw-rw-rw-   0        0        0     9827 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/replace.py
+-rw-rw-rw-   0        0        0    21071 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/rpc.py
+-rw-rw-rw-   0        0        0    21352 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/run.py
+-rw-rw-rw-   0        0        0     8278 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/runscript.py
+-rw-rw-rw-   0        0        0     4477 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/scrolledlist.py
+-rw-rw-rw-   0        0        0     5573 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/search.py
+-rw-rw-rw-   0        0        0     7859 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/searchbase.py
+-rw-rw-rw-   0        0        0     7409 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/searchengine.py
+-rw-rw-rw-   0        0        0    20341 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/sidebar.py
+-rw-rw-rw-   0        0        0    12845 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/squeezer.py
+-rw-rw-rw-   0        0        0     4016 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/stackviewer.py
+-rw-rw-rw-   0        0        0     1474 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/statusbar.py
+-rw-rw-rw-   0        0        0     6812 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/textview.py
+-rw-rw-rw-   0        0        0     6471 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/tooltip.py
+-rw-rw-rw-   0        0        0    16556 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/tree.py
+-rw-rw-rw-   0        0        0    11016 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/undo.py
+-rw-rw-rw-   0        0        0      731 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/util.py
+-rw-rw-rw-   0        0        0     2616 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/window.py
+-rw-rw-rw-   0        0        0     4179 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/zoomheight.py
+-rw-rw-rw-   0        0        0     2005 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/idlelib/zzdummy.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.392480 idcn-1.1.0/idcn/releases/3.11/turtledemo/
+-rw-rw-rw-   0        0        0      316 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/__init__.py
+-rw-rw-rw-   0        0        0    15065 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/__main__.py
+-rw-rw-rw-   0        0        0      160 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/turtle.cfg
+-rw-rw-rw-   0        0        0     3405 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/分形曲线.py
+-rw-rw-rw-   0        0        0     1117 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/双画布.py
+-rw-rw-rw-   0        0        0     1068 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/和平旗.py
+-rw-rw-rw-   0        0        0     4172 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/字节设计.py
+-rw-rw-rw-   0        0        0     3386 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/平铺图案.py
+-rw-rw-rw-   0        0        0     6520 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/拿火柴.py
+-rw-rw-rw-   0        0        0     5018 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/排序动画.py
+-rw-rw-rw-   0        0        0     3124 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/时钟.py
+-rw-rw-rw-   0        0        0     1999 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/极简汉诺塔.py
+-rw-rw-rw-   0        0        0     2412 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/林登麦伊尔.py
+-rw-rw-rw-   0        0        0     1338 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/树.py
+-rw-rw-rw-   0        0        0     3020 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/森林.py
+-rw-rw-rw-   0        0        0      949 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/混乱.py
+-rw-rw-rw-   0        0        0     1204 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/画图.py
+-rw-rw-rw-   0        0        0     1306 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/花形.py
+-rw-rw-rw-   0        0        0     2741 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/行星系统.py
+-rw-rw-rw-   0        0        0     1706 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/跳舞.py
+-rw-rw-rw-   0        0        0      793 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/阴阳.py
+-rw-rw-rw-   0        0        0     1356 2024-06-02 13:26:51.000000 idcn-1.1.0/idcn/releases/3.11/turtledemo/颜色混合器.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.171315 idcn-1.1.0/idcn/releases/3.12/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.435099 idcn-1.1.0/idcn/releases/3.12/idlelib/
+-rw-rw-rw-   0        0        0     2152 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/CREDITS.txt
+-rw-rw-rw-   0        0        0    56360 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/ChangeLog
+-rw-rw-rw-   0        0        0    10312 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/HISTORY.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.444709 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/
+-rw-rw-rw-   0        0        0      443 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/README.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/folder.gif
+-rw-rw-rw-   0        0        0    57746 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle.ico
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_16.gif
+-rw-rw-rw-   0        0        0     1031 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_16.png
+-rw-rw-rw-   0        0        0    39205 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_256.png
+-rw-rw-rw-   0        0        0     1019 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_32.gif
+-rw-rw-rw-   0        0        0     2036 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_32.png
+-rw-rw-rw-   0        0        0     1388 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_48.gif
+-rw-rw-rw-   0        0        0     3977 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_48.png
+-rw-rw-rw-   0        0        0       75 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/minusnode.gif
+-rw-rw-rw-   0        0        0      125 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/openfolder.gif
+-rw-rw-rw-   0        0        0       78 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/plusnode.gif
+-rw-rw-rw-   0        0        0      380 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/python.gif
+-rw-rw-rw-   0        0        0       72 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/tk.gif
+-rw-rw-rw-   0        0        0    27172 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/NEWS2x.txt
+-rw-rw-rw-   0        0        0    55577 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/News3.txt
+-rw-rw-rw-   0        0        0    11653 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/README.txt
+-rw-rw-rw-   0        0        0     8478 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/TODO.txt
+-rw-rw-rw-   0        0        0      396 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/__main__.py
+-rw-rw-rw-   0        0        0     9354 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/autocomplete.py
+-rw-rw-rw-   0        0        0    20863 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/autocomplete_w.py
+-rw-rw-rw-   0        0        0     3216 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/autoexpand.py
+-rw-rw-rw-   0        0        0     8590 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/browser.py
+-rw-rw-rw-   0        0        0     7265 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/calltip.py
+-rw-rw-rw-   0        0        0     7083 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/calltip_w.py
+-rw-rw-rw-   0        0        0    11429 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/codecontext.py
+-rw-rw-rw-   0        0        0    14783 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/colorizer.py
+-rw-rw-rw-   0        0        0     2266 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/config-extensions.def
+-rw-rw-rw-   0        0        0     2868 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/config-highlight.def
+-rw-rw-rw-   0        0        0    10906 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/config-keys.def
+-rw-rw-rw-   0        0        0     3167 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/config-main.def
+-rw-rw-rw-   0        0        0    38429 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/config.py
+-rw-rw-rw-   0        0        0    14978 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/config_key.py
+-rw-rw-rw-   0        0        0   105344 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/configdialog.py
+-rw-rw-rw-   0        0        0    21073 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/debugger.py
+-rw-rw-rw-   0        0        0    12118 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/debugger_r.py
+-rw-rw-rw-   0        0        0     4177 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/debugobj.py
+-rw-rw-rw-   0        0        0     1082 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/debugobj_r.py
+-rw-rw-rw-   0        0        0     1044 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/delegator.py
+-rw-rw-rw-   0        0        0     1993 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/dynoption.py
+-rw-rw-rw-   0        0        0    72225 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/editor.py
+-rw-rw-rw-   0        0        0     3631 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/extend.txt
+-rw-rw-rw-   0        0        0     3870 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/filelist.py
+-rw-rw-rw-   0        0        0    15825 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/format.py
+-rw-rw-rw-   0        0        0     7512 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/grep.py
+-rw-rw-rw-   0        0        0    78525 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/help.html
+-rw-rw-rw-   0        0        0    11980 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/help.py
+-rw-rw-rw-   0        0        0     8929 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/help_about.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/history.py
+-rw-rw-rw-   0        0        0    12889 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/hyperparser.py
+-rwxrwxrwx   0        0        0      173 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle.bat
+-rw-rw-rw-   0        0        0      454 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle.py
+-rw-rw-rw-   0        0        0      570 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle.pyw
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.487266 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/
+-rw-rw-rw-   0        0        0     8880 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/README.txt
+-rw-rw-rw-   0        0        0     1250 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/example_noext
+-rw-rw-rw-   0        0        0      154 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/example_stub.pyi
+-rw-rw-rw-   0        0        0    15313 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/htest.py
+-rw-rw-rw-   0        0        0     1943 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/mock_idle.py
+-rw-rw-rw-   0        0        0    11693 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/mock_tk.py
+-rw-rw-rw-   0        0        0      642 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/template.py
+-rw-rw-rw-   0        0        0    11093 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_autocomplete.py
+-rw-rw-rw-   0        0        0      720 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_autocomplete_w.py
+-rw-rw-rw-   0        0        0     4638 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_autoexpand.py
+-rw-rw-rw-   0        0        0     8420 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_browser.py
+-rw-rw-rw-   0        0        0    13658 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_calltip.py
+-rw-rw-rw-   0        0        0      686 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_calltip_w.py
+-rw-rw-rw-   0        0        0    16082 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_codecontext.py
+-rw-rw-rw-   0        0        0    22882 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_colorizer.py
+-rw-rw-rw-   0        0        0    32091 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_config.py
+-rw-rw-rw-   0        0        0    11462 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_config_key.py
+-rw-rw-rw-   0        0        0    55389 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_configdialog.py
+-rw-rw-rw-   0        0        0     9727 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugger.py
+-rw-rw-rw-   0        0        0      965 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugger_r.py
+-rw-rw-rw-   0        0        0     1611 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugobj.py
+-rw-rw-rw-   0        0        0      545 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugobj_r.py
+-rw-rw-rw-   0        0        0     1567 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_delegator.py
+-rw-rw-rw-   0        0        0     2564 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_editmenu.py
+-rw-rw-rw-   0        0        0     8151 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_editor.py
+-rw-rw-rw-   0        0        0      795 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_filelist.py
+-rw-rw-rw-   0        0        0    23610 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_format.py
+-rw-rw-rw-   0        0        0     5072 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_grep.py
+-rw-rw-rw-   0        0        0      863 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_help.py
+-rw-rw-rw-   0        0        0     5904 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_help_about.py
+-rw-rw-rw-   0        0        0     5517 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_history.py
+-rw-rw-rw-   0        0        0     9082 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_hyperparser.py
+-rw-rw-rw-   0        0        0     2457 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_iomenu.py
+-rw-rw-rw-   0        0        0     3444 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_macosx.py
+-rw-rw-rw-   0        0        0     1638 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_mainmenu.py
+-rw-rw-rw-   0        0        0     1317 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_multicall.py
+-rw-rw-rw-   0        0        0     5417 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_outwin.py
+-rw-rw-rw-   0        0        0     3544 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_parenmatch.py
+-rw-rw-rw-   0        0        0     2422 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_pathbrowser.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_percolator.py
+-rw-rw-rw-   0        0        0    19365 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_pyparse.py
+-rw-rw-rw-   0        0        0     4965 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_pyshell.py
+-rw-rw-rw-   0        0        0    15454 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_query.py
+-rw-rw-rw-   0        0        0     4176 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_redirector.py
+-rw-rw-rw-   0        0        0     8299 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_replace.py
+-rw-rw-rw-   0        0        0      805 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_rpc.py
+-rw-rw-rw-   0        0        0    15756 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_run.py
+-rw-rw-rw-   0        0        0      777 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_runscript.py
+-rw-rw-rw-   0        0        0      496 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_scrolledlist.py
+-rw-rw-rw-   0        0        0     2459 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_search.py
+-rw-rw-rw-   0        0        0     5691 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_searchbase.py
+-rw-rw-rw-   0        0        0    11588 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_searchengine.py
+-rw-rw-rw-   0        0        0    26854 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_sidebar.py
+-rw-rw-rw-   0        0        0    19656 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_squeezer.py
+-rw-rw-rw-   0        0        0      991 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_stackviewer.py
+-rw-rw-rw-   0        0        0     1133 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_statusbar.py
+-rw-rw-rw-   0        0        0     6970 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_text.py
+-rw-rw-rw-   0        0        0     7364 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_textview.py
+-rw-rw-rw-   0        0        0     5385 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_tooltip.py
+-rw-rw-rw-   0        0        0     1752 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_tree.py
+-rw-rw-rw-   0        0        0     4228 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_undo.py
+-rw-rw-rw-   0        0        0      308 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_util.py
+-rw-rw-rw-   0        0        0     2740 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_warning.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_window.py
+-rw-rw-rw-   0        0        0      999 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_zoomheight.py
+-rw-rw-rw-   0        0        0     4455 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_zzdummy.py
+-rw-rw-rw-   0        0        0     2333 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/tkinter_testing_utils.py
+-rw-rw-rw-   0        0        0    16289 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/iomenu.py
+-rw-rw-rw-   0        0        0     9269 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/macosx.py
+-rw-rw-rw-   0        0        0     4118 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/mainmenu.py
+-rw-rw-rw-   0        0        0    18652 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/multicall.py
+-rw-rw-rw-   0        0        0     5663 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/outwin.py
+-rw-rw-rw-   0        0        0     7204 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/parenmatch.py
+-rw-rw-rw-   0        0        0     3098 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/pathbrowser.py
+-rw-rw-rw-   0        0        0     3568 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/percolator.py
+-rw-rw-rw-   0        0        0    19864 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/pyparse.py
+-rw-rw-rw-   0        0        0    62241 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/pyshell.py
+-rw-rw-rw-   0        0        0    15138 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/query.py
+-rw-rw-rw-   0        0        0     6777 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/redirector.py
+-rw-rw-rw-   0        0        0     9827 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/replace.py
+-rw-rw-rw-   0        0        0    21071 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/rpc.py
+-rw-rw-rw-   0        0        0    21375 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/run.py
+-rw-rw-rw-   0        0        0     8278 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/runscript.py
+-rw-rw-rw-   0        0        0     4477 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/scrolledlist.py
+-rw-rw-rw-   0        0        0     5573 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/search.py
+-rw-rw-rw-   0        0        0     7859 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/searchbase.py
+-rw-rw-rw-   0        0        0     7409 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/searchengine.py
+-rw-rw-rw-   0        0        0    20341 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/sidebar.py
+-rw-rw-rw-   0        0        0    12845 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/squeezer.py
+-rw-rw-rw-   0        0        0     4016 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/stackviewer.py
+-rw-rw-rw-   0        0        0     1474 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/statusbar.py
+-rw-rw-rw-   0        0        0     6812 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/textview.py
+-rw-rw-rw-   0        0        0     6471 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/tooltip.py
+-rw-rw-rw-   0        0        0    16556 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/tree.py
+-rw-rw-rw-   0        0        0    11016 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/undo.py
+-rw-rw-rw-   0        0        0     1312 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/util.py
+-rw-rw-rw-   0        0        0     2616 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/window.py
+-rw-rw-rw-   0        0        0     4179 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/zoomheight.py
+-rw-rw-rw-   0        0        0     2005 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/idlelib/zzdummy.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.501875 idcn-1.1.0/idcn/releases/3.12/turtledemo/
+-rw-rw-rw-   0        0        0      316 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/__init__.py
+-rw-rw-rw-   0        0        0    15155 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/__main__.py
+-rw-rw-rw-   0        0        0      160 2024-06-02 13:26:49.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/turtle.cfg
+-rw-rw-rw-   0        0        0     3405 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/分形曲线.py
+-rw-rw-rw-   0        0        0     1117 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/双画布.py
+-rw-rw-rw-   0        0        0     1068 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/和平旗.py
+-rw-rw-rw-   0        0        0     4172 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/字节设计.py
+-rw-rw-rw-   0        0        0     3386 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/平铺图案.py
+-rw-rw-rw-   0        0        0     6520 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/拿火柴.py
+-rw-rw-rw-   0        0        0     5018 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/排序动画.py
+-rw-rw-rw-   0        0        0     3124 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/时钟.py
+-rw-rw-rw-   0        0        0     1999 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/极简汉诺塔.py
+-rw-rw-rw-   0        0        0     2412 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/林登麦伊尔.py
+-rw-rw-rw-   0        0        0     1338 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/树.py
+-rw-rw-rw-   0        0        0     3020 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/森林.py
+-rw-rw-rw-   0        0        0      949 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/混乱.py
+-rw-rw-rw-   0        0        0     1204 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/画图.py
+-rw-rw-rw-   0        0        0     1306 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/花形.py
+-rw-rw-rw-   0        0        0     2741 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/行星系统.py
+-rw-rw-rw-   0        0        0     1706 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/跳舞.py
+-rw-rw-rw-   0        0        0      793 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/阴阳.py
+-rw-rw-rw-   0        0        0     1356 2024-06-02 13:26:50.000000 idcn-1.1.0/idcn/releases/3.12/turtledemo/颜色混合器.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.171315 idcn-1.1.0/idcn/releases/3.13/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.546533 idcn-1.1.0/idcn/releases/3.13/idlelib/
+-rw-rw-rw-   0        0        0     2152 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/CREDITS.txt
+-rw-rw-rw-   0        0        0    56360 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/ChangeLog
+-rw-rw-rw-   0        0        0    10312 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/HISTORY.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.554565 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/
+-rw-rw-rw-   0        0        0      443 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/README.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/folder.gif
+-rw-rw-rw-   0        0        0    57746 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle.ico
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_16.gif
+-rw-rw-rw-   0        0        0     1031 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_16.png
+-rw-rw-rw-   0        0        0    39205 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_256.png
+-rw-rw-rw-   0        0        0     1019 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_32.gif
+-rw-rw-rw-   0        0        0     2036 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_32.png
+-rw-rw-rw-   0        0        0     1388 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_48.gif
+-rw-rw-rw-   0        0        0     3977 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_48.png
+-rw-rw-rw-   0        0        0       75 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/minusnode.gif
+-rw-rw-rw-   0        0        0      125 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/openfolder.gif
+-rw-rw-rw-   0        0        0       78 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/plusnode.gif
+-rw-rw-rw-   0        0        0      380 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/python.gif
+-rw-rw-rw-   0        0        0       72 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/tk.gif
+-rw-rw-rw-   0        0        0    27172 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/NEWS2x.txt
+-rw-rw-rw-   0        0        0    55574 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/News3.txt
+-rw-rw-rw-   0        0        0    11653 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/README.txt
+-rw-rw-rw-   0        0        0     8478 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/TODO.txt
+-rw-rw-rw-   0        0        0      396 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/__main__.py
+-rw-rw-rw-   0        0        0     9354 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/autocomplete.py
+-rw-rw-rw-   0        0        0    20863 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/autocomplete_w.py
+-rw-rw-rw-   0        0        0     3216 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/autoexpand.py
+-rw-rw-rw-   0        0        0     8590 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/browser.py
+-rw-rw-rw-   0        0        0     7265 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/calltip.py
+-rw-rw-rw-   0        0        0     7083 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/calltip_w.py
+-rw-rw-rw-   0        0        0    11429 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/codecontext.py
+-rw-rw-rw-   0        0        0    14783 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/colorizer.py
+-rw-rw-rw-   0        0        0     2266 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/config-extensions.def
+-rw-rw-rw-   0        0        0     2868 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/config-highlight.def
+-rw-rw-rw-   0        0        0    10906 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/config-keys.def
+-rw-rw-rw-   0        0        0     3167 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/config-main.def
+-rw-rw-rw-   0        0        0    38429 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/config.py
+-rw-rw-rw-   0        0        0    14978 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/config_key.py
+-rw-rw-rw-   0        0        0   105344 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/configdialog.py
+-rw-rw-rw-   0        0        0    21073 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/debugger.py
+-rw-rw-rw-   0        0        0    12118 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/debugger_r.py
+-rw-rw-rw-   0        0        0     4177 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/debugobj.py
+-rw-rw-rw-   0        0        0     1082 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/debugobj_r.py
+-rw-rw-rw-   0        0        0     1044 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/delegator.py
+-rw-rw-rw-   0        0        0     1993 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/dynoption.py
+-rw-rw-rw-   0        0        0    72225 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/editor.py
+-rw-rw-rw-   0        0        0     3631 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/extend.txt
+-rw-rw-rw-   0        0        0     3870 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/filelist.py
+-rw-rw-rw-   0        0        0    15825 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/format.py
+-rw-rw-rw-   0        0        0     7512 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/grep.py
+-rw-rw-rw-   0        0        0    78525 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/help.html
+-rw-rw-rw-   0        0        0    11980 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/help.py
+-rw-rw-rw-   0        0        0     8929 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/help_about.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/history.py
+-rw-rw-rw-   0        0        0    12889 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/hyperparser.py
+-rwxrwxrwx   0        0        0      173 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle.bat
+-rw-rw-rw-   0        0        0      454 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle.py
+-rw-rw-rw-   0        0        0      570 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle.pyw
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.604457 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/
+-rw-rw-rw-   0        0        0     8880 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/README.txt
+-rw-rw-rw-   0        0        0     1250 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/example_noext
+-rw-rw-rw-   0        0        0      154 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/example_stub.pyi
+-rw-rw-rw-   0        0        0    15313 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/htest.py
+-rw-rw-rw-   0        0        0     1943 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/mock_idle.py
+-rw-rw-rw-   0        0        0    11693 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/mock_tk.py
+-rw-rw-rw-   0        0        0      642 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/template.py
+-rw-rw-rw-   0        0        0    11093 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_autocomplete.py
+-rw-rw-rw-   0        0        0      720 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_autocomplete_w.py
+-rw-rw-rw-   0        0        0     4638 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_autoexpand.py
+-rw-rw-rw-   0        0        0     8420 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_browser.py
+-rw-rw-rw-   0        0        0    13658 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_calltip.py
+-rw-rw-rw-   0        0        0      686 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_calltip_w.py
+-rw-rw-rw-   0        0        0    16082 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_codecontext.py
+-rw-rw-rw-   0        0        0    22882 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_colorizer.py
+-rw-rw-rw-   0        0        0    32091 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_config.py
+-rw-rw-rw-   0        0        0    11462 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_config_key.py
+-rw-rw-rw-   0        0        0    55389 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_configdialog.py
+-rw-rw-rw-   0        0        0     9727 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugger.py
+-rw-rw-rw-   0        0        0      965 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugger_r.py
+-rw-rw-rw-   0        0        0     1611 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugobj.py
+-rw-rw-rw-   0        0        0      545 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugobj_r.py
+-rw-rw-rw-   0        0        0     1567 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_delegator.py
+-rw-rw-rw-   0        0        0     2564 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_editmenu.py
+-rw-rw-rw-   0        0        0     8151 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_editor.py
+-rw-rw-rw-   0        0        0      795 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_filelist.py
+-rw-rw-rw-   0        0        0    23610 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_format.py
+-rw-rw-rw-   0        0        0     5072 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_grep.py
+-rw-rw-rw-   0        0        0      863 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_help.py
+-rw-rw-rw-   0        0        0     5904 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_help_about.py
+-rw-rw-rw-   0        0        0     5517 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_history.py
+-rw-rw-rw-   0        0        0     9082 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_hyperparser.py
+-rw-rw-rw-   0        0        0     2457 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_iomenu.py
+-rw-rw-rw-   0        0        0     3444 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_macosx.py
+-rw-rw-rw-   0        0        0     1638 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_mainmenu.py
+-rw-rw-rw-   0        0        0     1317 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_multicall.py
+-rw-rw-rw-   0        0        0     5417 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_outwin.py
+-rw-rw-rw-   0        0        0     3544 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_parenmatch.py
+-rw-rw-rw-   0        0        0     2422 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_pathbrowser.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_percolator.py
+-rw-rw-rw-   0        0        0    19365 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_pyparse.py
+-rw-rw-rw-   0        0        0     4965 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_pyshell.py
+-rw-rw-rw-   0        0        0    15454 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_query.py
+-rw-rw-rw-   0        0        0     4176 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_redirector.py
+-rw-rw-rw-   0        0        0     8299 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_replace.py
+-rw-rw-rw-   0        0        0      805 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_rpc.py
+-rw-rw-rw-   0        0        0    15851 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_run.py
+-rw-rw-rw-   0        0        0      777 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_runscript.py
+-rw-rw-rw-   0        0        0      496 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_scrolledlist.py
+-rw-rw-rw-   0        0        0     2459 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_search.py
+-rw-rw-rw-   0        0        0     5691 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_searchbase.py
+-rw-rw-rw-   0        0        0    11588 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_searchengine.py
+-rw-rw-rw-   0        0        0    26854 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_sidebar.py
+-rw-rw-rw-   0        0        0    19656 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_squeezer.py
+-rw-rw-rw-   0        0        0      991 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_stackviewer.py
+-rw-rw-rw-   0        0        0     1133 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_statusbar.py
+-rw-rw-rw-   0        0        0     6970 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_text.py
+-rw-rw-rw-   0        0        0     7364 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_textview.py
+-rw-rw-rw-   0        0        0     5385 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_tooltip.py
+-rw-rw-rw-   0        0        0     1752 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_tree.py
+-rw-rw-rw-   0        0        0     4228 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_undo.py
+-rw-rw-rw-   0        0        0      308 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_util.py
+-rw-rw-rw-   0        0        0     2740 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_warning.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_window.py
+-rw-rw-rw-   0        0        0      999 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_zoomheight.py
+-rw-rw-rw-   0        0        0     4455 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_zzdummy.py
+-rw-rw-rw-   0        0        0     2333 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/tkinter_testing_utils.py
+-rw-rw-rw-   0        0        0    16289 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/iomenu.py
+-rw-rw-rw-   0        0        0     9269 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/macosx.py
+-rw-rw-rw-   0        0        0     4118 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/mainmenu.py
+-rw-rw-rw-   0        0        0    18652 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/multicall.py
+-rw-rw-rw-   0        0        0     5663 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/outwin.py
+-rw-rw-rw-   0        0        0     7204 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/parenmatch.py
+-rw-rw-rw-   0        0        0     3098 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/pathbrowser.py
+-rw-rw-rw-   0        0        0     3568 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/percolator.py
+-rw-rw-rw-   0        0        0    19864 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/pyparse.py
+-rw-rw-rw-   0        0        0    62241 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/pyshell.py
+-rw-rw-rw-   0        0        0    15138 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/query.py
+-rw-rw-rw-   0        0        0     6832 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/redirector.py
+-rw-rw-rw-   0        0        0     9784 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/replace.py
+-rw-rw-rw-   0        0        0    21071 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/rpc.py
+-rw-rw-rw-   0        0        0    21375 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/run.py
+-rw-rw-rw-   0        0        0     8278 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/runscript.py
+-rw-rw-rw-   0        0        0     4477 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/scrolledlist.py
+-rw-rw-rw-   0        0        0     5573 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/search.py
+-rw-rw-rw-   0        0        0     7859 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/searchbase.py
+-rw-rw-rw-   0        0        0     7366 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/searchengine.py
+-rw-rw-rw-   0        0        0    20330 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/sidebar.py
+-rw-rw-rw-   0        0        0    12845 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/squeezer.py
+-rw-rw-rw-   0        0        0     4016 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/stackviewer.py
+-rw-rw-rw-   0        0        0     1474 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/statusbar.py
+-rw-rw-rw-   0        0        0     6812 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/textview.py
+-rw-rw-rw-   0        0        0     6471 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/tooltip.py
+-rw-rw-rw-   0        0        0    16556 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/tree.py
+-rw-rw-rw-   0        0        0    11016 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/undo.py
+-rw-rw-rw-   0        0        0     1312 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/util.py
+-rw-rw-rw-   0        0        0     2616 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/window.py
+-rw-rw-rw-   0        0        0     4179 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/zoomheight.py
+-rw-rw-rw-   0        0        0     2005 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/idlelib/zzdummy.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.617440 idcn-1.1.0/idcn/releases/3.13/turtledemo/
+-rw-rw-rw-   0        0        0      316 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/__init__.py
+-rw-rw-rw-   0        0        0    15155 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/__main__.py
+-rw-rw-rw-   0        0        0      160 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/turtle.cfg
+-rw-rw-rw-   0        0        0     3405 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/分形曲线.py
+-rw-rw-rw-   0        0        0     1117 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/双画布.py
+-rw-rw-rw-   0        0        0     1068 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/和平旗.py
+-rw-rw-rw-   0        0        0     4172 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/字节设计.py
+-rw-rw-rw-   0        0        0     3386 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/平铺图案.py
+-rw-rw-rw-   0        0        0     6520 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/拿火柴.py
+-rw-rw-rw-   0        0        0     5018 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/排序动画.py
+-rw-rw-rw-   0        0        0     3124 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/时钟.py
+-rw-rw-rw-   0        0        0     1999 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/极简汉诺塔.py
+-rw-rw-rw-   0        0        0     2412 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/林登麦伊尔.py
+-rw-rw-rw-   0        0        0     1338 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/树.py
+-rw-rw-rw-   0        0        0     3020 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/森林.py
+-rw-rw-rw-   0        0        0      949 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/混乱.py
+-rw-rw-rw-   0        0        0     1204 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/画图.py
+-rw-rw-rw-   0        0        0     1306 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/花形.py
+-rw-rw-rw-   0        0        0     2741 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/行星系统.py
+-rw-rw-rw-   0        0        0     1706 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/跳舞.py
+-rw-rw-rw-   0        0        0      793 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/阴阳.py
+-rw-rw-rw-   0        0        0     1356 2024-06-02 13:26:48.000000 idcn-1.1.0/idcn/releases/3.13/turtledemo/颜色混合器.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.172313 idcn-1.1.0/idcn/releases/3.8/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.661351 idcn-1.1.0/idcn/releases/3.8/idlelib/
+-rw-rw-rw-   0        0        0     1866 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/CREDITS.txt
+-rw-rw-rw-   0        0        0    56360 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/ChangeLog
+-rw-rw-rw-   0        0        0    10312 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/HISTORY.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.670361 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/
+-rw-rw-rw-   0        0        0      443 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/README.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/folder.gif
+-rw-rw-rw-   0        0        0    57746 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle.ico
+-rw-rw-rw-   0        0        0     1034 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_16.gif
+-rw-rw-rw-   0        0        0     1264 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_16.png
+-rw-rw-rw-   0        0        0    42839 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_256.png
+-rw-rw-rw-   0        0        0     1435 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_32.gif
+-rw-rw-rw-   0        0        0     2542 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_32.png
+-rw-rw-rw-   0        0        0     1388 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_48.gif
+-rw-rw-rw-   0        0        0     4710 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_48.png
+-rw-rw-rw-   0        0        0       96 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/minusnode.gif
+-rw-rw-rw-   0        0        0      125 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/openfolder.gif
+-rw-rw-rw-   0        0        0       79 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/plusnode.gif
+-rw-rw-rw-   0        0        0      585 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/python.gif
+-rw-rw-rw-   0        0        0       85 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/tk.gif
+-rw-rw-rw-   0        0        0    50808 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/NEWS.txt
+-rw-rw-rw-   0        0        0    27172 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/NEWS2x.txt
+-rw-rw-rw-   0        0        0     9599 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/README.txt
+-rw-rw-rw-   0        0        0     8478 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/TODO.txt
+-rw-rw-rw-   0        0        0      396 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/__main__.py
+-rw-rw-rw-   0        0        0     9150 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/autocomplete.py
+-rw-rw-rw-   0        0        0    20109 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/autocomplete_w.py
+-rw-rw-rw-   0        0        0     3216 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/autoexpand.py
+-rw-rw-rw-   0        0        0     8316 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/browser.py
+-rw-rw-rw-   0        0        0     7265 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/calltip.py
+-rw-rw-rw-   0        0        0     7158 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/calltip_w.py
+-rw-rw-rw-   0        0        0    11429 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/codecontext.py
+-rw-rw-rw-   0        0        0    13201 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/colorizer.py
+-rw-rw-rw-   0        0        0     2266 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/config-extensions.def
+-rw-rw-rw-   0        0        0     2868 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/config-highlight.def
+-rw-rw-rw-   0        0        0    10906 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/config-keys.def
+-rw-rw-rw-   0        0        0     3167 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/config-main.def
+-rw-rw-rw-   0        0        0    38200 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/config.py
+-rw-rw-rw-   0        0        0    14288 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/config_key.py
+-rw-rw-rw-   0        0        0   105087 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/configdialog.py
+-rw-rw-rw-   0        0        0    19186 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/debugger.py
+-rw-rw-rw-   0        0        0    12170 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/debugger_r.py
+-rw-rw-rw-   0        0        0     4055 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/debugobj.py
+-rw-rw-rw-   0        0        0     1082 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/debugobj_r.py
+-rw-rw-rw-   0        0        0     1043 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/delegator.py
+-rw-rw-rw-   0        0        0     2017 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/dynoption.py
+-rw-rw-rw-   0        0        0    68360 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/editor.py
+-rw-rw-rw-   0        0        0     3631 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/extend.txt
+-rw-rw-rw-   0        0        0     3875 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/filelist.py
+-rw-rw-rw-   0        0        0    15825 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/format.py
+-rw-rw-rw-   0        0        0     7465 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/grep.py
+-rw-rw-rw-   0        0        0    68324 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/help.html
+-rw-rw-rw-   0        0        0    11859 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/help.py
+-rw-rw-rw-   0        0        0     8998 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/help_about.py
+-rw-rw-rw-   0        0        0     4043 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/history.py
+-rw-rw-rw-   0        0        0    12883 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/hyperparser.py
+-rwxrwxrwx   0        0        0      173 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle.bat
+-rw-rw-rw-   0        0        0      454 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle.py
+-rw-rw-rw-   0        0        0      570 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle.pyw
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.709728 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/
+-rw-rw-rw-   0        0        0     8729 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/README.txt
+-rw-rw-rw-   0        0        0      712 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/__init__.py
+-rw-rw-rw-   0        0        0    15190 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/htest.py
+-rw-rw-rw-   0        0        0     1943 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/mock_idle.py
+-rw-rw-rw-   0        0        0    11692 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/mock_tk.py
+-rw-rw-rw-   0        0        0      642 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/template.py
+-rw-rw-rw-   0        0        0    10904 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_autocomplete.py
+-rw-rw-rw-   0        0        0      709 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_autocomplete_w.py
+-rw-rw-rw-   0        0        0     4638 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_autoexpand.py
+-rw-rw-rw-   0        0        0     7963 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_browser.py
+-rw-rw-rw-   0        0        0    13193 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_calltip.py
+-rw-rw-rw-   0        0        0      686 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_calltip_w.py
+-rw-rw-rw-   0        0        0    16082 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_codecontext.py
+-rw-rw-rw-   0        0        0    15017 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_colorizer.py
+-rw-rw-rw-   0        0        0    32046 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_config.py
+-rw-rw-rw-   0        0        0     9709 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_config_key.py
+-rw-rw-rw-   0        0        0    54344 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_configdialog.py
+-rw-rw-rw-   0        0        0      571 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugger.py
+-rw-rw-rw-   0        0        0     1009 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugger_r.py
+-rw-rw-rw-   0        0        0     1561 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugobj.py
+-rw-rw-rw-   0        0        0      545 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugobj_r.py
+-rw-rw-rw-   0        0        0     1567 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_delegator.py
+-rw-rw-rw-   0        0        0     2564 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_editmenu.py
+-rw-rw-rw-   0        0        0     7523 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_editor.py
+-rw-rw-rw-   0        0        0      795 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_filelist.py
+-rw-rw-rw-   0        0        0    23610 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_format.py
+-rw-rw-rw-   0        0        0     5072 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_grep.py
+-rw-rw-rw-   0        0        0      849 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_help.py
+-rw-rw-rw-   0        0        0     5919 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_help_about.py
+-rw-rw-rw-   0        0        0     5517 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_history.py
+-rw-rw-rw-   0        0        0     9082 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_hyperparser.py
+-rw-rw-rw-   0        0        0     1278 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_iomenu.py
+-rw-rw-rw-   0        0        0     3309 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_macosx.py
+-rw-rw-rw-   0        0        0     1638 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_mainmenu.py
+-rw-rw-rw-   0        0        0     1316 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_multicall.py
+-rw-rw-rw-   0        0        0     5422 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_outwin.py
+-rw-rw-rw-   0        0        0     3550 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_parenmatch.py
+-rw-rw-rw-   0        0        0     2422 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_pathbrowser.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_percolator.py
+-rw-rw-rw-   0        0        0    19364 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_pyparse.py
+-rw-rw-rw-   0        0        0     2171 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_pyshell.py
+-rw-rw-rw-   0        0        0    15450 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_query.py
+-rw-rw-rw-   0        0        0     4176 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_redirector.py
+-rw-rw-rw-   0        0        0     8299 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_replace.py
+-rw-rw-rw-   0        0        0      805 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_rpc.py
+-rw-rw-rw-   0        0        0    13983 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_run.py
+-rw-rw-rw-   0        0        0      777 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_runscript.py
+-rw-rw-rw-   0        0        0      496 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_scrolledlist.py
+-rw-rw-rw-   0        0        0     2459 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_search.py
+-rw-rw-rw-   0        0        0     5691 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_searchbase.py
+-rw-rw-rw-   0        0        0    11588 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_searchengine.py
+-rw-rw-rw-   0        0        0    13231 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_sidebar.py
+-rw-rw-rw-   0        0        0    20108 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_squeezer.py
+-rw-rw-rw-   0        0        0     1206 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_stackviewer.py
+-rw-rw-rw-   0        0        0     1133 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_statusbar.py
+-rw-rw-rw-   0        0        0     6978 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_text.py
+-rw-rw-rw-   0        0        0     7364 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_textview.py
+-rw-rw-rw-   0        0        0     5385 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_tooltip.py
+-rw-rw-rw-   0        0        0     1752 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_tree.py
+-rw-rw-rw-   0        0        0     4228 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_undo.py
+-rw-rw-rw-   0        0        0     2740 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_warning.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_window.py
+-rw-rw-rw-   0        0        0      999 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_zoomheight.py
+-rw-rw-rw-   0        0        0     4457 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_zzdummy.py
+-rw-rw-rw-   0        0        0    15863 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/iomenu.py
+-rw-rw-rw-   0        0        0     9641 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/macosx.py
+-rw-rw-rw-   0        0        0     4109 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/mainmenu.py
+-rw-rw-rw-   0        0        0    18648 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/multicall.py
+-rw-rw-rw-   0        0        0     5657 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/outwin.py
+-rw-rw-rw-   0        0        0     7204 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/parenmatch.py
+-rw-rw-rw-   0        0        0     3198 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/pathbrowser.py
+-rw-rw-rw-   0        0        0     3130 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/percolator.py
+-rw-rw-rw-   0        0        0    19947 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/pyparse.py
+-rw-rw-rw-   0        0        0    57468 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/pyshell.py
+-rw-rw-rw-   0        0        0    15142 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/query.py
+-rw-rw-rw-   0        0        0     6875 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/redirector.py
+-rw-rw-rw-   0        0        0     9875 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/replace.py
+-rw-rw-rw-   0        0        0    21069 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/rpc.py
+-rw-rw-rw-   0        0        0    20855 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/run.py
+-rw-rw-rw-   0        0        0     8278 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/runscript.py
+-rw-rw-rw-   0        0        0     4464 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/scrolledlist.py
+-rw-rw-rw-   0        0        0     5572 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/search.py
+-rw-rw-rw-   0        0        0     7859 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/searchbase.py
+-rw-rw-rw-   0        0        0     7356 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/searchengine.py
+-rw-rw-rw-   0        0        0    13585 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/sidebar.py
+-rw-rw-rw-   0        0        0    12836 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/squeezer.py
+-rw-rw-rw-   0        0        0     4454 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/stackviewer.py
+-rw-rw-rw-   0        0        0     1472 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/statusbar.py
+-rw-rw-rw-   0        0        0     6817 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/textview.py
+-rw-rw-rw-   0        0        0     6557 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/tooltip.py
+-rw-rw-rw-   0        0        0    16443 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/tree.py
+-rw-rw-rw-   0        0        0    11046 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/undo.py
+-rw-rw-rw-   0        0        0     2616 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/window.py
+-rw-rw-rw-   0        0        0     4179 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/zoomheight.py
+-rw-rw-rw-   0        0        0     2005 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/idlelib/zzdummy.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.723799 idcn-1.1.0/idcn/releases/3.8/turtledemo/
+-rw-rw-rw-   0        0        0      316 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/__init__.py
+-rw-rw-rw-   0        0        0    14040 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/__main__.py
+-rw-rw-rw-   0        0        0      160 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/turtle.cfg
+-rw-rw-rw-   0        0        0     3405 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/分形曲线.py
+-rw-rw-rw-   0        0        0     1117 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/双画布.py
+-rw-rw-rw-   0        0        0     1068 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/和平旗.py
+-rw-rw-rw-   0        0        0     4172 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/字节设计.py
+-rw-rw-rw-   0        0        0     3386 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/平铺图案.py
+-rw-rw-rw-   0        0        0     6520 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/拿火柴.py
+-rw-rw-rw-   0        0        0     5018 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/排序动画.py
+-rw-rw-rw-   0        0        0     3145 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/时钟.py
+-rw-rw-rw-   0        0        0     1999 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/极简汉诺塔.py
+-rw-rw-rw-   0        0        0     2412 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/林登麦伊尔.py
+-rw-rw-rw-   0        0        0     1338 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/树.py
+-rw-rw-rw-   0        0        0     3020 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/森林.py
+-rw-rw-rw-   0        0        0      949 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/混乱.py
+-rw-rw-rw-   0        0        0     1204 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/画图.py
+-rw-rw-rw-   0        0        0     1306 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/花形.py
+-rw-rw-rw-   0        0        0     2741 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/行星系统.py
+-rw-rw-rw-   0        0        0     1706 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/跳舞.py
+-rw-rw-rw-   0        0        0      793 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/阴阳.py
+-rw-rw-rw-   0        0        0     1356 2024-06-02 13:26:56.000000 idcn-1.1.0/idcn/releases/3.8/turtledemo/颜色混合器.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.173313 idcn-1.1.0/idcn/releases/3.9/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.768315 idcn-1.1.0/idcn/releases/3.9/idlelib/
+-rw-rw-rw-   0        0        0     1866 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/CREDITS.txt
+-rw-rw-rw-   0        0        0    56360 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/ChangeLog
+-rw-rw-rw-   0        0        0    10312 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/HISTORY.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.777916 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/
+-rw-rw-rw-   0        0        0      443 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/README.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/folder.gif
+-rw-rw-rw-   0        0        0    57746 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle.ico
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_16.gif
+-rw-rw-rw-   0        0        0     1031 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_16.png
+-rw-rw-rw-   0        0        0    39205 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_256.png
+-rw-rw-rw-   0        0        0     1019 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_32.gif
+-rw-rw-rw-   0        0        0     2036 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_32.png
+-rw-rw-rw-   0        0        0     1388 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_48.gif
+-rw-rw-rw-   0        0        0     3977 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_48.png
+-rw-rw-rw-   0        0        0       75 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/minusnode.gif
+-rw-rw-rw-   0        0        0      125 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/openfolder.gif
+-rw-rw-rw-   0        0        0       78 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/plusnode.gif
+-rw-rw-rw-   0        0        0      380 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/python.gif
+-rw-rw-rw-   0        0        0       72 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/tk.gif
+-rw-rw-rw-   0        0        0    51948 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/NEWS.txt
+-rw-rw-rw-   0        0        0    27172 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/NEWS2x.txt
+-rw-rw-rw-   0        0        0     9680 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/README.txt
+-rw-rw-rw-   0        0        0     8478 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/TODO.txt
+-rw-rw-rw-   0        0        0      396 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/__main__.py
+-rw-rw-rw-   0        0        0     9150 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/autocomplete.py
+-rw-rw-rw-   0        0        0    20981 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/autocomplete_w.py
+-rw-rw-rw-   0        0        0     3216 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/autoexpand.py
+-rw-rw-rw-   0        0        0     8316 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/browser.py
+-rw-rw-rw-   0        0        0     7265 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/calltip.py
+-rw-rw-rw-   0        0        0     7158 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/calltip_w.py
+-rw-rw-rw-   0        0        0    11429 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/codecontext.py
+-rw-rw-rw-   0        0        0    13201 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/colorizer.py
+-rw-rw-rw-   0        0        0     2266 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/config-extensions.def
+-rw-rw-rw-   0        0        0     2868 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/config-highlight.def
+-rw-rw-rw-   0        0        0    10906 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/config-keys.def
+-rw-rw-rw-   0        0        0     3167 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/config-main.def
+-rw-rw-rw-   0        0        0    38200 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/config.py
+-rw-rw-rw-   0        0        0    14288 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/config_key.py
+-rw-rw-rw-   0        0        0   105765 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/configdialog.py
+-rw-rw-rw-   0        0        0    19186 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/debugger.py
+-rw-rw-rw-   0        0        0    12170 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/debugger_r.py
+-rw-rw-rw-   0        0        0     4055 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/debugobj.py
+-rw-rw-rw-   0        0        0     1082 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/debugobj_r.py
+-rw-rw-rw-   0        0        0     1043 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/delegator.py
+-rw-rw-rw-   0        0        0     2017 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/dynoption.py
+-rw-rw-rw-   0        0        0    68397 2024-06-02 13:26:55.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/editor.py
+-rw-rw-rw-   0        0        0     3631 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/extend.txt
+-rw-rw-rw-   0        0        0     3875 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/filelist.py
+-rw-rw-rw-   0        0        0    15825 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/format.py
+-rw-rw-rw-   0        0        0     7465 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/grep.py
+-rw-rw-rw-   0        0        0    68554 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/help.html
+-rw-rw-rw-   0        0        0    11859 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/help.py
+-rw-rw-rw-   0        0        0     9101 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/help_about.py
+-rw-rw-rw-   0        0        0     4043 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/history.py
+-rw-rw-rw-   0        0        0    12883 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/hyperparser.py
+-rwxrwxrwx   0        0        0      173 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle.bat
+-rw-rw-rw-   0        0        0      454 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle.py
+-rw-rw-rw-   0        0        0      570 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle.pyw
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.816386 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/
+-rw-rw-rw-   0        0        0     8729 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/README.txt
+-rw-rw-rw-   0        0        0      712 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/example_noext
+-rw-rw-rw-   0        0        0       87 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/example_stub.pyi
+-rw-rw-rw-   0        0        0    15199 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/htest.py
+-rw-rw-rw-   0        0        0     1943 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/mock_idle.py
+-rw-rw-rw-   0        0        0    11693 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/mock_tk.py
+-rw-rw-rw-   0        0        0      642 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/template.py
+-rw-rw-rw-   0        0        0    10904 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_autocomplete.py
+-rw-rw-rw-   0        0        0      709 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_autocomplete_w.py
+-rw-rw-rw-   0        0        0     4638 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_autoexpand.py
+-rw-rw-rw-   0        0        0     7963 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_browser.py
+-rw-rw-rw-   0        0        0    13194 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_calltip.py
+-rw-rw-rw-   0        0        0      686 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_calltip_w.py
+-rw-rw-rw-   0        0        0    16082 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_codecontext.py
+-rw-rw-rw-   0        0        0    15017 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_colorizer.py
+-rw-rw-rw-   0        0        0    32046 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_config.py
+-rw-rw-rw-   0        0        0     9708 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_config_key.py
+-rw-rw-rw-   0        0        0    55344 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_configdialog.py
+-rw-rw-rw-   0        0        0      571 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugger.py
+-rw-rw-rw-   0        0        0     1009 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugger_r.py
+-rw-rw-rw-   0        0        0     1561 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugobj.py
+-rw-rw-rw-   0        0        0      545 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugobj_r.py
+-rw-rw-rw-   0        0        0     1567 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_delegator.py
+-rw-rw-rw-   0        0        0     2564 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_editmenu.py
+-rw-rw-rw-   0        0        0     7523 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_editor.py
+-rw-rw-rw-   0        0        0      795 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_filelist.py
+-rw-rw-rw-   0        0        0    23610 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_format.py
+-rw-rw-rw-   0        0        0     5072 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_grep.py
+-rw-rw-rw-   0        0        0      849 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_help.py
+-rw-rw-rw-   0        0        0     5919 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_help_about.py
+-rw-rw-rw-   0        0        0     5517 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_history.py
+-rw-rw-rw-   0        0        0     9082 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_hyperparser.py
+-rw-rw-rw-   0        0        0     1908 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_iomenu.py
+-rw-rw-rw-   0        0        0     3444 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_macosx.py
+-rw-rw-rw-   0        0        0     1638 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_mainmenu.py
+-rw-rw-rw-   0        0        0     1317 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_multicall.py
+-rw-rw-rw-   0        0        0     5422 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_outwin.py
+-rw-rw-rw-   0        0        0     3550 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_parenmatch.py
+-rw-rw-rw-   0        0        0     2422 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_pathbrowser.py
+-rw-rw-rw-   0        0        0     4065 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_percolator.py
+-rw-rw-rw-   0        0        0    19365 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_pyparse.py
+-rw-rw-rw-   0        0        0     2171 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_pyshell.py
+-rw-rw-rw-   0        0        0    15454 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_query.py
+-rw-rw-rw-   0        0        0     4176 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_redirector.py
+-rw-rw-rw-   0        0        0     8299 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_replace.py
+-rw-rw-rw-   0        0        0      805 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_rpc.py
+-rw-rw-rw-   0        0        0    13983 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_run.py
+-rw-rw-rw-   0        0        0      777 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_runscript.py
+-rw-rw-rw-   0        0        0      496 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_scrolledlist.py
+-rw-rw-rw-   0        0        0     2459 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_search.py
+-rw-rw-rw-   0        0        0     5691 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_searchbase.py
+-rw-rw-rw-   0        0        0    11588 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_searchengine.py
+-rw-rw-rw-   0        0        0    13231 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_sidebar.py
+-rw-rw-rw-   0        0        0    20108 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_squeezer.py
+-rw-rw-rw-   0        0        0     1206 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_stackviewer.py
+-rw-rw-rw-   0        0        0     1133 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_statusbar.py
+-rw-rw-rw-   0        0        0     6978 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_text.py
+-rw-rw-rw-   0        0        0     7364 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_textview.py
+-rw-rw-rw-   0        0        0     5385 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_tooltip.py
+-rw-rw-rw-   0        0        0     1752 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_tree.py
+-rw-rw-rw-   0        0        0     4228 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_undo.py
+-rw-rw-rw-   0        0        0      308 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_util.py
+-rw-rw-rw-   0        0        0     2740 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_warning.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_window.py
+-rw-rw-rw-   0        0        0      999 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_zoomheight.py
+-rw-rw-rw-   0        0        0     4457 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_zzdummy.py
+-rw-rw-rw-   0        0        0    15963 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/iomenu.py
+-rw-rw-rw-   0        0        0     9642 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/macosx.py
+-rw-rw-rw-   0        0        0     4109 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/mainmenu.py
+-rw-rw-rw-   0        0        0    18648 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/multicall.py
+-rw-rw-rw-   0        0        0     5657 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/outwin.py
+-rw-rw-rw-   0        0        0     7204 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/parenmatch.py
+-rw-rw-rw-   0        0        0     3198 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/pathbrowser.py
+-rw-rw-rw-   0        0        0     3130 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/percolator.py
+-rw-rw-rw-   0        0        0    19864 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/pyparse.py
+-rw-rw-rw-   0        0        0    57639 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/pyshell.py
+-rw-rw-rw-   0        0        0    15146 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/query.py
+-rw-rw-rw-   0        0        0     6875 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/redirector.py
+-rw-rw-rw-   0        0        0     9785 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/replace.py
+-rw-rw-rw-   0        0        0    21069 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/rpc.py
+-rw-rw-rw-   0        0        0    20960 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/run.py
+-rw-rw-rw-   0        0        0     8278 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/runscript.py
+-rw-rw-rw-   0        0        0     4464 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/scrolledlist.py
+-rw-rw-rw-   0        0        0     5572 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/search.py
+-rw-rw-rw-   0        0        0     7859 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/searchbase.py
+-rw-rw-rw-   0        0        0     7356 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/searchengine.py
+-rw-rw-rw-   0        0        0    13585 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/sidebar.py
+-rw-rw-rw-   0        0        0    12836 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/squeezer.py
+-rw-rw-rw-   0        0        0     4454 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/stackviewer.py
+-rw-rw-rw-   0        0        0     1472 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/statusbar.py
+-rw-rw-rw-   0        0        0     6817 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/textview.py
+-rw-rw-rw-   0        0        0     6557 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/tooltip.py
+-rw-rw-rw-   0        0        0    16443 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/tree.py
+-rw-rw-rw-   0        0        0    11046 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/undo.py
+-rw-rw-rw-   0        0        0      721 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/util.py
+-rw-rw-rw-   0        0        0     2616 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/window.py
+-rw-rw-rw-   0        0        0     4179 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/zoomheight.py
+-rw-rw-rw-   0        0        0     2005 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/idlelib/zzdummy.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.829316 idcn-1.1.0/idcn/releases/3.9/turtledemo/
+-rw-rw-rw-   0        0        0      316 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/__init__.py
+-rw-rw-rw-   0        0        0    14830 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/__main__.py
+-rw-rw-rw-   0        0        0      160 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/turtle.cfg
+-rw-rw-rw-   0        0        0     3405 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/分形曲线.py
+-rw-rw-rw-   0        0        0     1117 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/双画布.py
+-rw-rw-rw-   0        0        0     1068 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/和平旗.py
+-rw-rw-rw-   0        0        0     4172 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/字节设计.py
+-rw-rw-rw-   0        0        0     3386 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/平铺图案.py
+-rw-rw-rw-   0        0        0     6520 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/拿火柴.py
+-rw-rw-rw-   0        0        0     5018 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/排序动画.py
+-rw-rw-rw-   0        0        0     3145 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/时钟.py
+-rw-rw-rw-   0        0        0     1999 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/极简汉诺塔.py
+-rw-rw-rw-   0        0        0     2412 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/林登麦伊尔.py
+-rw-rw-rw-   0        0        0     1338 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/树.py
+-rw-rw-rw-   0        0        0     3020 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/森林.py
+-rw-rw-rw-   0        0        0      949 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/混乱.py
+-rw-rw-rw-   0        0        0     1204 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/画图.py
+-rw-rw-rw-   0        0        0     1306 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/花形.py
+-rw-rw-rw-   0        0        0     2741 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/行星系统.py
+-rw-rw-rw-   0        0        0     1706 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/跳舞.py
+-rw-rw-rw-   0        0        0      793 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/阴阳.py
+-rw-rw-rw-   0        0        0     1356 2024-06-02 13:26:54.000000 idcn-1.1.0/idcn/releases/3.9/turtledemo/颜色混合器.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:26:59.830320 idcn-1.1.0/idcn.egg-info/
+-rw-rw-rw-   0        0        0     2591 2024-06-02 13:26:58.000000 idcn-1.1.0/idcn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    48680 2024-06-02 13:26:59.000000 idcn-1.1.0/idcn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 13:26:58.000000 idcn-1.1.0/idcn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-02 13:26:58.000000 idcn-1.1.0/idcn.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2024-06-02 13:26:58.000000 idcn-1.1.0/idcn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2024-06-02 13:23:01.000000 idcn-1.1.0/idcn.pth
+-rw-rw-rw-   0        0        0       42 2024-06-02 13:26:59.831320 idcn-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1636 2024-06-02 13:23:01.000000 idcn-1.1.0/setup.py
```

### Comparing `idcn-1.0.1/PKG-INFO` & `idcn-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idcn
-Version: 1.0.1
+Version: 1.1.0
 Summary: IDLE Chinese Translation | IDLE 汉化包
 Home-page: https://github.com/zetaloop/IDLE-CN
 Author: zetaloop
 Author-email: zetaloop@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `idcn-1.0.1/README.md` & `idcn-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/CREDITS.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/ChangeLog` & `idcn-1.1.0/idcn/releases/3.10/idlelib/ChangeLog`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/HISTORY.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle.ico` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle.ico`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_16.gif` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_16.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_16.png` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_16.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_256.png` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_256.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_32.gif` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_32.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_32.png` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_32.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_48.gif` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_48.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/Icons/idle_48.png` & `idcn-1.1.0/idcn/releases/3.10/idlelib/Icons/idle_48.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/NEWS.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/NEWS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/NEWS2x.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/NEWS2x.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/README.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/TODO.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/TODO.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/autocomplete.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/autoexpand.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/browser.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/calltip.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/calltip_w.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/codecontext.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/colorizer.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/config-extensions.def` & `idcn-1.1.0/idcn/releases/3.10/idlelib/config-extensions.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/config-highlight.def` & `idcn-1.1.0/idcn/releases/3.10/idlelib/config-highlight.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/config-keys.def` & `idcn-1.1.0/idcn/releases/3.10/idlelib/config-keys.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/config-main.def` & `idcn-1.1.0/idcn/releases/3.10/idlelib/config-main.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/config.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/config_key.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/configdialog.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/debugger.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/debugger_r.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/debugobj.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/delegator.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/dynoption.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/dynoption.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/editor.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/extend.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/extend.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/filelist.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/format.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/grep.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/help.html` & `idcn-1.1.0/idcn/releases/3.10/idlelib/help.html`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/help.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/help_about.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/history.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/hyperparser.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle.pyw` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle.pyw`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/README.txt` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/__init__.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/__init__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/htest.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/htest.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/mock_idle.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/mock_idle.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/mock_tk.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/mock_tk.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/template.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/template.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_autocomplete.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_autoexpand.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_browser.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_calltip.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_calltip_w.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_codecontext.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_colorizer.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_config.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_config_key.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_configdialog.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugger.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugger_r.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugobj.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_delegator.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_editmenu.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_editmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_editor.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_filelist.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_format.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_grep.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_help.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_help_about.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_history.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_hyperparser.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_iomenu.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_macosx.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_mainmenu.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_multicall.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_outwin.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_parenmatch.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_percolator.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_pyparse.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_pyshell.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_query.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_redirector.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_replace.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_rpc.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_run.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_runscript.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_search.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_searchbase.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_searchengine.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_sidebar.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_squeezer.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_stackviewer.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_statusbar.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_text.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_text.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_textview.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_tooltip.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_tree.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_undo.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_warning.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_warning.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_window.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_zoomheight.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/test_zzdummy.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/test_zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/idle_test/tkinter_testing_utils.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/idle_test/tkinter_testing_utils.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/iomenu.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/macosx.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/mainmenu.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/multicall.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/outwin.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/parenmatch.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/percolator.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/pyparse.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/pyshell.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/query.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/redirector.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/replace.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/rpc.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/run.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/runscript.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/scrolledlist.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/scrolledlist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/search.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/searchbase.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/searchengine.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/sidebar.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/squeezer.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/stackviewer.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/statusbar.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/textview.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/tooltip.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/tree.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/undo.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/util.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/util.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/window.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/zoomheight.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/idlelib/zzdummy.py` & `idcn-1.1.0/idcn/releases/3.10/idlelib/zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/__main__.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/__main__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/分形曲线.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/分形曲线.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/双画布.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/双画布.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/和平旗.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/和平旗.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/字节设计.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/字节设计.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/平铺图案.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/平铺图案.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/拿火柴.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/拿火柴.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/排序动画.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/排序动画.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/时钟.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/时钟.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/极简汉诺塔.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/极简汉诺塔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/林登麦伊尔.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/林登麦伊尔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/树.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/树.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/森林.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/森林.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/混乱.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/混乱.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/画图.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/画图.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/花形.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/花形.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/行星系统.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/行星系统.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/跳舞.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/跳舞.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/阴阳.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/阴阳.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.10/turtledemo/颜色混合器.py` & `idcn-1.1.0/idcn/releases/3.10/turtledemo/颜色混合器.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/CREDITS.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/ChangeLog` & `idcn-1.1.0/idcn/releases/3.11/idlelib/ChangeLog`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/HISTORY.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle.ico` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle.ico`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_16.gif` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_16.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_16.png` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_16.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_256.png` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_256.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_32.gif` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_32.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_32.png` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_32.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_48.gif` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_48.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/Icons/idle_48.png` & `idcn-1.1.0/idcn/releases/3.11/idlelib/Icons/idle_48.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/NEWS2x.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/NEWS2x.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/News3.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/News3.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/README.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/TODO.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/TODO.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/autocomplete.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/autoexpand.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/browser.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/calltip.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/calltip_w.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/codecontext.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/colorizer.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/config-extensions.def` & `idcn-1.1.0/idcn/releases/3.11/idlelib/config-extensions.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/config-highlight.def` & `idcn-1.1.0/idcn/releases/3.11/idlelib/config-highlight.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/config-keys.def` & `idcn-1.1.0/idcn/releases/3.11/idlelib/config-keys.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/config-main.def` & `idcn-1.1.0/idcn/releases/3.11/idlelib/config-main.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/config.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/config_key.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/configdialog.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/debugger.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/debugger_r.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/debugobj.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/delegator.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/dynoption.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/dynoption.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/editor.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/extend.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/extend.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/filelist.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/format.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/grep.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/help.html` & `idcn-1.1.0/idcn/releases/3.11/idlelib/help.html`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/help.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/help_about.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/history.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/hyperparser.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle.pyw` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle.pyw`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/README.txt` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/__init__.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/__init__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/htest.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/htest.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/mock_idle.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/mock_idle.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/mock_tk.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/mock_tk.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/template.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/template.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_autocomplete.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_autoexpand.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_browser.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_calltip.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_calltip_w.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_codecontext.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_colorizer.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_config.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_config_key.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_configdialog.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugger.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugger_r.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugobj.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_delegator.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_editmenu.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_editmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_editor.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_filelist.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_format.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_grep.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_help.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_help_about.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_history.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_hyperparser.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_iomenu.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_macosx.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_mainmenu.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_multicall.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_outwin.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_parenmatch.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_percolator.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_pyparse.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_pyshell.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_query.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_redirector.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_replace.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_rpc.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_run.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_runscript.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_search.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_searchbase.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_searchengine.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_sidebar.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_squeezer.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_stackviewer.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_statusbar.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_text.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_text.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_textview.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_tooltip.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_tree.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_undo.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_warning.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_warning.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_window.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_zoomheight.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/test_zzdummy.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/test_zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/idle_test/tkinter_testing_utils.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/idle_test/tkinter_testing_utils.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/iomenu.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/macosx.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/mainmenu.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/multicall.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/outwin.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/parenmatch.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/percolator.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/pyparse.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/pyshell.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/query.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/redirector.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/replace.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/rpc.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/run.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/runscript.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/scrolledlist.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/scrolledlist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/search.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/searchbase.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/searchengine.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/sidebar.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/squeezer.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/stackviewer.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/statusbar.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/textview.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/tooltip.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/tree.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/undo.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/util.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/util.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/window.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/zoomheight.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/idlelib/zzdummy.py` & `idcn-1.1.0/idcn/releases/3.11/idlelib/zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/__main__.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/__main__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/分形曲线.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/分形曲线.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/双画布.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/双画布.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/和平旗.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/和平旗.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/字节设计.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/字节设计.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/平铺图案.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/平铺图案.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/拿火柴.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/拿火柴.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/排序动画.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/排序动画.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/时钟.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/时钟.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/极简汉诺塔.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/极简汉诺塔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/林登麦伊尔.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/林登麦伊尔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/树.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/树.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/森林.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/森林.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/混乱.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/混乱.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/画图.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/画图.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/花形.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/花形.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/行星系统.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/行星系统.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/跳舞.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/跳舞.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/阴阳.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/阴阳.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.11/turtledemo/颜色混合器.py` & `idcn-1.1.0/idcn/releases/3.11/turtledemo/颜色混合器.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/CREDITS.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/ChangeLog` & `idcn-1.1.0/idcn/releases/3.12/idlelib/ChangeLog`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/HISTORY.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle.ico` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle.ico`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_16.gif` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_16.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_16.png` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_16.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_256.png` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_256.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_32.gif` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_32.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_32.png` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_32.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_48.gif` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_48.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/Icons/idle_48.png` & `idcn-1.1.0/idcn/releases/3.12/idlelib/Icons/idle_48.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/NEWS2x.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/NEWS2x.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/News3.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/News3.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/README.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/TODO.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/TODO.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/autocomplete.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/autoexpand.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/browser.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/calltip.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/calltip_w.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/codecontext.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/colorizer.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/config-extensions.def` & `idcn-1.1.0/idcn/releases/3.12/idlelib/config-extensions.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/config-highlight.def` & `idcn-1.1.0/idcn/releases/3.12/idlelib/config-highlight.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/config-keys.def` & `idcn-1.1.0/idcn/releases/3.12/idlelib/config-keys.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/config-main.def` & `idcn-1.1.0/idcn/releases/3.12/idlelib/config-main.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/config.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/config_key.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/configdialog.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/debugger.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/debugger_r.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/debugobj.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/delegator.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/dynoption.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/dynoption.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/editor.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/extend.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/extend.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/filelist.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/format.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/grep.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/help.html` & `idcn-1.1.0/idcn/releases/3.12/idlelib/help.html`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/help.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/help_about.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/history.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/hyperparser.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle.pyw` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle.pyw`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/README.txt` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/__init__.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/__init__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/htest.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/htest.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/mock_idle.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/mock_idle.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/mock_tk.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/mock_tk.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/template.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/template.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_autocomplete.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_autoexpand.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_browser.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_calltip.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_calltip_w.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_codecontext.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_colorizer.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_config.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_config_key.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_configdialog.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugger.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugger_r.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugobj.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_delegator.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_editmenu.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_editmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_editor.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_filelist.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_format.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_grep.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_help.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_help_about.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_history.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_hyperparser.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_iomenu.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_macosx.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_mainmenu.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_multicall.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_outwin.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_parenmatch.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_percolator.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_pyparse.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_pyshell.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_query.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_redirector.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_replace.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_rpc.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_run.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_runscript.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_search.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_searchbase.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_searchengine.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_sidebar.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_squeezer.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_stackviewer.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_statusbar.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_text.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_text.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_textview.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_tooltip.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_tree.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_undo.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_warning.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_warning.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_window.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_zoomheight.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/test_zzdummy.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/test_zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/idle_test/tkinter_testing_utils.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/idle_test/tkinter_testing_utils.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/iomenu.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/macosx.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/mainmenu.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/multicall.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/outwin.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/parenmatch.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/percolator.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/pyparse.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/pyshell.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/query.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/redirector.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/replace.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/rpc.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/run.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/runscript.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/scrolledlist.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/scrolledlist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/search.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/searchbase.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/searchengine.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/sidebar.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/squeezer.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/stackviewer.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/statusbar.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/textview.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/tooltip.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/tree.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/undo.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/util.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/util.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/window.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/zoomheight.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/idlelib/zzdummy.py` & `idcn-1.1.0/idcn/releases/3.12/idlelib/zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/__main__.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/__main__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/分形曲线.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/分形曲线.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/双画布.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/双画布.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/和平旗.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/和平旗.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/字节设计.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/字节设计.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/平铺图案.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/平铺图案.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/拿火柴.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/拿火柴.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/排序动画.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/排序动画.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/时钟.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/时钟.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/极简汉诺塔.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/极简汉诺塔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/林登麦伊尔.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/林登麦伊尔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/树.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/树.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/森林.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/森林.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/混乱.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/混乱.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/画图.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/画图.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/花形.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/花形.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/行星系统.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/行星系统.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/跳舞.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/跳舞.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/阴阳.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/阴阳.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.12/turtledemo/颜色混合器.py` & `idcn-1.1.0/idcn/releases/3.12/turtledemo/颜色混合器.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/CREDITS.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/ChangeLog` & `idcn-1.1.0/idcn/releases/3.13/idlelib/ChangeLog`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/HISTORY.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle.ico` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle.ico`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_16.gif` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_16.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_16.png` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_16.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_256.png` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_256.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_32.gif` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_32.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_32.png` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_32.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_48.gif` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_48.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/Icons/idle_48.png` & `idcn-1.1.0/idcn/releases/3.13/idlelib/Icons/idle_48.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/NEWS2x.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/NEWS2x.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/News3.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/News3.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/README.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/TODO.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/TODO.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/autocomplete.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/autoexpand.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/browser.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/calltip.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/calltip_w.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/codecontext.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/colorizer.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/config-extensions.def` & `idcn-1.1.0/idcn/releases/3.13/idlelib/config-extensions.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/config-highlight.def` & `idcn-1.1.0/idcn/releases/3.13/idlelib/config-highlight.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/config-keys.def` & `idcn-1.1.0/idcn/releases/3.13/idlelib/config-keys.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/config-main.def` & `idcn-1.1.0/idcn/releases/3.13/idlelib/config-main.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/config.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/config_key.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/configdialog.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/debugger.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/debugger_r.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/debugobj.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/delegator.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/dynoption.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/dynoption.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/editor.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/extend.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/extend.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/filelist.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/format.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/grep.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/help.html` & `idcn-1.1.0/idcn/releases/3.13/idlelib/help.html`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/help.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/help_about.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/history.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/hyperparser.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle.pyw` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle.pyw`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/README.txt` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/__init__.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/__init__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/htest.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/htest.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/mock_idle.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/mock_idle.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/mock_tk.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/mock_tk.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/template.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/template.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_autocomplete.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_autoexpand.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_browser.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_calltip.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_calltip_w.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_codecontext.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_colorizer.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_config.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_config_key.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_configdialog.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugger.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugger_r.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugobj.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_delegator.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_editmenu.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_editmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_editor.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_filelist.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_format.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_grep.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_help.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_help_about.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_history.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_hyperparser.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_iomenu.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_macosx.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_mainmenu.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_multicall.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_outwin.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_parenmatch.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_percolator.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_pyparse.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_pyshell.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_query.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_redirector.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_replace.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_rpc.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_run.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_runscript.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_search.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_searchbase.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_searchengine.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_sidebar.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_squeezer.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_stackviewer.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_statusbar.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_text.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_text.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_textview.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_tooltip.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_tree.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_undo.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_warning.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_warning.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_window.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_zoomheight.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/test_zzdummy.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/test_zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/idle_test/tkinter_testing_utils.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/idle_test/tkinter_testing_utils.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/iomenu.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/macosx.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/mainmenu.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/multicall.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/outwin.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/parenmatch.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/percolator.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/pyparse.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/pyshell.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/query.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/redirector.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/replace.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/rpc.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/run.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/runscript.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/scrolledlist.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/scrolledlist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/search.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/searchbase.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/searchengine.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/sidebar.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/squeezer.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/stackviewer.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/statusbar.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/textview.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/tooltip.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/tree.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/undo.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/util.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/util.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/window.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/zoomheight.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/idlelib/zzdummy.py` & `idcn-1.1.0/idcn/releases/3.13/idlelib/zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/__main__.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/__main__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/分形曲线.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/分形曲线.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/双画布.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/双画布.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/和平旗.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/和平旗.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/字节设计.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/字节设计.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/平铺图案.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/平铺图案.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/拿火柴.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/拿火柴.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/排序动画.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/排序动画.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/时钟.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/时钟.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/极简汉诺塔.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/极简汉诺塔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/林登麦伊尔.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/林登麦伊尔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/树.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/树.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/森林.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/森林.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/混乱.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/混乱.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/画图.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/画图.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/花形.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/花形.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/行星系统.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/行星系统.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/跳舞.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/跳舞.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/阴阳.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/阴阳.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.13/turtledemo/颜色混合器.py` & `idcn-1.1.0/idcn/releases/3.13/turtledemo/颜色混合器.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/CREDITS.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/ChangeLog` & `idcn-1.1.0/idcn/releases/3.8/idlelib/ChangeLog`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/HISTORY.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle.ico` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle.ico`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_16.gif` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_16.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_16.png` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_16.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_256.png` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_256.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_32.gif` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_32.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_32.png` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_32.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_48.gif` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_48.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/idle_48.png` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/idle_48.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/Icons/python.gif` & `idcn-1.1.0/idcn/releases/3.8/idlelib/Icons/python.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/NEWS.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/NEWS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/NEWS2x.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/NEWS2x.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/README.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/TODO.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/TODO.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/autocomplete.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/autoexpand.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/browser.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/calltip.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/calltip_w.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/codecontext.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/colorizer.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/config-extensions.def` & `idcn-1.1.0/idcn/releases/3.8/idlelib/config-extensions.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/config-highlight.def` & `idcn-1.1.0/idcn/releases/3.8/idlelib/config-highlight.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/config-keys.def` & `idcn-1.1.0/idcn/releases/3.8/idlelib/config-keys.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/config-main.def` & `idcn-1.1.0/idcn/releases/3.8/idlelib/config-main.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/config.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/config_key.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/configdialog.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/debugger.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/debugger_r.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/debugobj.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/delegator.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/dynoption.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/dynoption.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/editor.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/extend.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/extend.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/filelist.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/format.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/grep.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/help.html` & `idcn-1.1.0/idcn/releases/3.8/idlelib/help.html`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/help.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/help_about.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/history.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/hyperparser.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle.pyw` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle.pyw`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/README.txt` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/__init__.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/__init__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/htest.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/htest.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/mock_idle.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/mock_idle.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/mock_tk.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/mock_tk.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/template.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/template.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_autocomplete.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_autoexpand.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_browser.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_calltip.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_calltip_w.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_codecontext.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_colorizer.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_config.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_config_key.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_configdialog.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugger.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugger_r.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugobj.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_delegator.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_editmenu.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_editmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_editor.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_filelist.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_format.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_grep.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_help.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_help_about.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_history.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_hyperparser.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_iomenu.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_macosx.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_mainmenu.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_multicall.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_outwin.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_parenmatch.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_percolator.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_pyparse.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_pyshell.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_query.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_redirector.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_replace.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_rpc.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_run.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_runscript.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_search.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_searchbase.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_searchengine.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_sidebar.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_squeezer.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_stackviewer.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_statusbar.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_text.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_text.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_textview.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_tooltip.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_tree.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_undo.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_warning.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_warning.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_window.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_zoomheight.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/idle_test/test_zzdummy.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/idle_test/test_zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/iomenu.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/macosx.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/mainmenu.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/multicall.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/outwin.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/parenmatch.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/percolator.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/pyparse.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/pyshell.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/query.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/redirector.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/replace.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/rpc.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/run.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/runscript.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/scrolledlist.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/scrolledlist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/search.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/searchbase.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/searchengine.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/sidebar.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/squeezer.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/stackviewer.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/statusbar.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/textview.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/tooltip.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/tree.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/undo.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/window.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/zoomheight.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/idlelib/zzdummy.py` & `idcn-1.1.0/idcn/releases/3.8/idlelib/zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/__main__.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/__main__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/分形曲线.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/分形曲线.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/双画布.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/双画布.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/和平旗.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/和平旗.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/字节设计.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/字节设计.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/平铺图案.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/平铺图案.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/拿火柴.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/拿火柴.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/排序动画.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/排序动画.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/时钟.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/时钟.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/极简汉诺塔.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/极简汉诺塔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/林登麦伊尔.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/林登麦伊尔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/树.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/树.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/森林.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/森林.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/混乱.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/混乱.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/画图.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/画图.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/花形.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/花形.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/行星系统.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/行星系统.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/跳舞.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/跳舞.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/阴阳.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/阴阳.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.8/turtledemo/颜色混合器.py` & `idcn-1.1.0/idcn/releases/3.8/turtledemo/颜色混合器.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/CREDITS.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/ChangeLog` & `idcn-1.1.0/idcn/releases/3.9/idlelib/ChangeLog`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/HISTORY.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle.ico` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle.ico`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_16.gif` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_16.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_16.png` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_16.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_256.png` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_256.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_32.gif` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_32.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_32.png` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_32.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_48.gif` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_48.gif`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/Icons/idle_48.png` & `idcn-1.1.0/idcn/releases/3.9/idlelib/Icons/idle_48.png`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/NEWS.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/NEWS.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/NEWS2x.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/NEWS2x.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/README.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/TODO.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/TODO.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/autocomplete.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/autoexpand.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/browser.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/calltip.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/calltip_w.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/codecontext.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/colorizer.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/config-extensions.def` & `idcn-1.1.0/idcn/releases/3.9/idlelib/config-extensions.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/config-highlight.def` & `idcn-1.1.0/idcn/releases/3.9/idlelib/config-highlight.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/config-keys.def` & `idcn-1.1.0/idcn/releases/3.9/idlelib/config-keys.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/config-main.def` & `idcn-1.1.0/idcn/releases/3.9/idlelib/config-main.def`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/config.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/config_key.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/configdialog.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/debugger.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/debugger_r.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/debugobj.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/delegator.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/dynoption.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/dynoption.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/editor.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/extend.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/extend.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/filelist.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/format.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/grep.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/help.html` & `idcn-1.1.0/idcn/releases/3.9/idlelib/help.html`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/help.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/help_about.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/history.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/hyperparser.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle.pyw` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle.pyw`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/README.txt` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/README.txt`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/__init__.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/__init__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/htest.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/htest.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/mock_idle.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/mock_idle.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/mock_tk.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/mock_tk.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/template.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/template.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_autocomplete.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_autocomplete_w.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_autocomplete_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_autoexpand.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_autoexpand.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_browser.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_browser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_calltip.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_calltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_calltip_w.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_calltip_w.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_codecontext.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_codecontext.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_colorizer.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_colorizer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_config.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_config.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_config_key.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_config_key.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_configdialog.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_configdialog.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugger.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugger.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugger_r.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugger_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugobj.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugobj.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_debugobj_r.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_debugobj_r.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_delegator.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_delegator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_editmenu.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_editmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_editor.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_editor.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_filelist.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_format.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_format.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_grep.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_grep.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_help.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_help.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_help_about.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_help_about.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_history.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_history.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_hyperparser.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_hyperparser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_iomenu.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_macosx.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_mainmenu.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_multicall.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_outwin.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_parenmatch.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_percolator.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_pyparse.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_pyshell.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_query.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_redirector.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_replace.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_rpc.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_run.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_runscript.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_search.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_searchbase.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_searchengine.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_sidebar.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_squeezer.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_stackviewer.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_statusbar.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_text.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_text.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_textview.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_tooltip.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_tree.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_undo.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_warning.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_warning.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_window.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_zoomheight.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/idle_test/test_zzdummy.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/idle_test/test_zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/iomenu.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/iomenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/macosx.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/macosx.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/mainmenu.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/mainmenu.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/multicall.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/multicall.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/outwin.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/outwin.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/parenmatch.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/parenmatch.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/pathbrowser.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/pathbrowser.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/percolator.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/percolator.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/pyparse.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/pyparse.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/pyshell.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/pyshell.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/query.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/query.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/redirector.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/redirector.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/replace.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/replace.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/rpc.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/rpc.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/run.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/run.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/runscript.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/runscript.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/scrolledlist.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/scrolledlist.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/search.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/search.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/searchbase.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/searchbase.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/searchengine.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/searchengine.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/sidebar.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/sidebar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/squeezer.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/squeezer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/stackviewer.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/stackviewer.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/statusbar.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/statusbar.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/textview.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/textview.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/tooltip.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/tooltip.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/tree.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/tree.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/undo.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/undo.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/util.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/util.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/window.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/window.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/zoomheight.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/zoomheight.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/idlelib/zzdummy.py` & `idcn-1.1.0/idcn/releases/3.9/idlelib/zzdummy.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/__main__.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/__main__.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/分形曲线.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/分形曲线.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/双画布.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/双画布.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/和平旗.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/和平旗.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/字节设计.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/字节设计.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/平铺图案.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/平铺图案.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/拿火柴.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/拿火柴.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/排序动画.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/排序动画.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/时钟.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/时钟.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/极简汉诺塔.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/极简汉诺塔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/林登麦伊尔.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/林登麦伊尔.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/树.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/树.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/森林.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/森林.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/混乱.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/混乱.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/画图.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/画图.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/花形.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/花形.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/行星系统.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/行星系统.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/跳舞.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/跳舞.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/阴阳.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/阴阳.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn/releases/3.9/turtledemo/颜色混合器.py` & `idcn-1.1.0/idcn/releases/3.9/turtledemo/颜色混合器.py`

 * *Files identical despite different names*

### Comparing `idcn-1.0.1/idcn.egg-info/PKG-INFO` & `idcn-1.1.0/idcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idcn
-Version: 1.0.1
+Version: 1.1.0
 Summary: IDLE Chinese Translation | IDLE 汉化包
 Home-page: https://github.com/zetaloop/IDLE-CN
 Author: zetaloop
 Author-email: zetaloop@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `idcn-1.0.1/idcn.egg-info/SOURCES.txt` & `idcn-1.1.0/idcn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE
 README.md
-idcn.pth
 setup.py
 idcn/__init__.py
 idcn.egg-info/PKG-INFO
 idcn.egg-info/SOURCES.txt
 idcn.egg-info/dependency_links.txt
 idcn.egg-info/not-zip-safe
 idcn.egg-info/top_level.txt
+idcn/../idcn.pth
 idcn/releases/3.10/idlelib/CREDITS.txt
 idcn/releases/3.10/idlelib/ChangeLog
 idcn/releases/3.10/idlelib/HISTORY.txt
 idcn/releases/3.10/idlelib/NEWS.txt
 idcn/releases/3.10/idlelib/NEWS2x.txt
 idcn/releases/3.10/idlelib/README.txt
 idcn/releases/3.10/idlelib/TODO.txt
```

### Comparing `idcn-1.0.1/setup.py` & `idcn-1.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 from setuptools import setup
 from pathlib import Path
-import sys
 
 
 def find_idcn_release_files():
     release_dir = Path("idcn/releases")
     release_files = []
     for file in release_dir.rglob("*"):
         if file.is_file():
             release_files.append(str(file.relative_to("idcn")))
+    release_files.append("../idcn.pth")
     return release_files
 
 
-def get_site_packages_dir():
-    if sys.platform == "win32":
-        return "lib/site-packages"
-    else:
-        return "lib/python{0}/site-packages".format(
-            ".".join(str(i) for i in sys.version_info[:2])
-        )
-
-
 setup(
     name="idcn",
-    version="1.0.1",
+    version="1.1.0",
     author="zetaloop",
     author_email="zetaloop@outlook.com",
     description="IDLE Chinese Translation | IDLE 汉化包",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/zetaloop/IDLE-CN",
     packages=["idcn"],
     package_data={"idcn": find_idcn_release_files()},
-    data_files=[(get_site_packages_dir(), ["idcn.pth"])],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Topic :: Software Development :: Internationalization",
         "Topic :: Software Development :: Localization",
         "License :: OSI Approved :: MIT License",
@@ -48,10 +38,9 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Operating System :: OS Independent",
         "Natural Language :: Chinese (Simplified)",
     ],
     python_requires=">=3.8",
-    include_package_data=True,
     zip_safe=False,
 )
```

