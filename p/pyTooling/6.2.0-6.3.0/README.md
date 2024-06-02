# Comparing `tmp/pytooling-6.2.0.tar.gz` & `tmp/pytooling-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytooling-6.2.0.tar", last modified: Thu May 30 23:03:43 2024, max compression
+gzip compressed data, was "pytooling-6.3.0.tar", last modified: Sun Jun  2 00:31:14 2024, max compression
```

## Comparing `pytooling-6.2.0.tar` & `pytooling-6.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.197213 pytooling-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-30 23:03:39.000000 pytooling-6.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-05-30 23:03:43.197213 pytooling-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-05-30 23:03:39.000000 pytooling-6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.181213 pytooling-6.2.0/pyTooling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.181213 pytooling-6.2.0/pyTooling/Attributes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/Attributes/ArgParse/
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/Argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/Flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/ArgParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/CLIAbstraction/
--rw-r--r--   0 runner    (1001) docker     (127)    24815 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/Argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/Command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/Flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlagList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)    17086 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CLIAbstraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/CallByRef/
--rw-r--r--   0 runner    (1001) docker     (127)    23206 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/CallByRef/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.185213 pytooling-6.2.0/pyTooling/Common/
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Configuration/JSON.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Configuration/YAML.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/GenericPath/
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/GenericPath/URL.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/GenericPath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Graph/
--rw-r--r--   0 runner    (1001) docker     (127)    20618 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Graph/GraphML.py
--rw-r--r--   0 runner    (1001) docker     (127)    92485 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Licensing/
--rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Licensing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/MetaClasses/
--rw-r--r--   0 runner    (1001) docker     (127)    36214 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/MetaClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Packaging/
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Packaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Platform/
--rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/StateMachine/
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/StateMachine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/TerminalUI/
--rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/TerminalUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Timer/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Timer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Tree/
--rw-r--r--   0 runner    (1001) docker     (127)    35173 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.189213 pytooling-6.2.0/pyTooling/Versioning/
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/Versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyTooling/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:03:43.193213 pytooling-6.2.0/pyTooling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 23:03:43.000000 pytooling-6.2.0/pyTooling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-30 23:03:39.000000 pytooling-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:03:43.197213 pytooling-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-30 23:03:39.000000 pytooling-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.845620 pytooling-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-06-02 00:31:07.000000 pytooling-6.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-06-02 00:31:14.845620 pytooling-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-06-02 00:31:07.000000 pytooling-6.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.829620 pytooling-6.3.0/pyTooling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.829620 pytooling-6.3.0/pyTooling/Attributes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.833620 pytooling-6.3.0/pyTooling/Attributes/ArgParse/
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/ArgParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.833620 pytooling-6.3.0/pyTooling/CLIAbstraction/
+-rw-r--r--   0 runner    (1001) docker     (127)    24815 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/Command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/ValuedFlagList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17086 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CLIAbstraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.833620 pytooling-6.3.0/pyTooling/CallByRef/
+-rw-r--r--   0 runner    (1001) docker     (127)    23206 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/CallByRef/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.833620 pytooling-6.3.0/pyTooling/Common/
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Configuration/JSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Configuration/YAML.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/GenericPath/
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/GenericPath/URL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/GenericPath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    20618 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Graph/GraphML.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96963 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Licensing/
+-rw-r--r--   0 runner    (1001) docker     (127)    10709 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Licensing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/MetaClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)    36214 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/MetaClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Packaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Platform/
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/StateMachine/
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/StateMachine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/TerminalUI/
+-rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/TerminalUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Timer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Timer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Tree/
+-rw-r--r--   0 runner    (1001) docker     (127)    36541 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling/Versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/Versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyTooling/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:31:14.837620 pytooling-6.3.0/pyTooling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21788 2024-06-02 00:31:14.000000 pytooling-6.3.0/pyTooling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-02 00:31:14.000000 pytooling-6.3.0/pyTooling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:31:14.000000 pytooling-6.3.0/pyTooling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-02 00:31:14.000000 pytooling-6.3.0/pyTooling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 00:31:14.000000 pytooling-6.3.0/pyTooling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-06-02 00:31:07.000000 pytooling-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:31:14.845620 pytooling-6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-06-02 00:31:07.000000 pytooling-6.3.0/setup.py
```

### Comparing `pytooling-6.2.0/LICENSE.md` & `pytooling-6.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/PKG-INFO` & `pytooling-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 6.2.0
+Version: 6.3.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -21,65 +21,65 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: doc
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: docutils~=0.18.0; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: docutils~=0.18.0; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: setuptools~=70.0; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
 Provides-Extra: test
+Requires-Dist: typing_extensions~=4.12; extra == "test"
+Requires-Dist: colorama>=0.4.6; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: pytest~=8.2; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: typing_extensions~=4.11; extra == "test"
-Requires-Dist: colorama>=0.4.6; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
 Provides-Extra: packaging
 Requires-Dist: setuptools>=69.0.0; extra == "packaging"
 Provides-Extra: terminal
 Requires-Dist: colorama>=0.4.6; extra == "terminal"
 Provides-Extra: yaml
 Requires-Dist: ruamel.yaml>=0.18; extra == "yaml"
 Provides-Extra: all
+Requires-Dist: sphinx~=7.3; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: docutils~=0.18.0; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
-Requires-Dist: mypy~=1.10; extra == "all"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
 Requires-Dist: setuptools>=69.0.0; extra == "all"
+Requires-Dist: docutils~=0.18.0; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: setuptools~=70.0; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: typing_extensions~=4.12; extra == "all"
 Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: ruamel.yaml>=0.18; extra == "all"
 Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
 Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyTooling-pyTooling-63bf7f.svg?longCache=true&style=flat-square&longCache=true&logo=GitHub)](https://GitHub.com/pyTooling/pyTooling)
 [![Sourcecode License](https://img.shields.io/pypi/l/pyTooling?longCache=true&style=flat-square&logo=Apache&label=code)](LICENSE.md)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=pyTooling.github.io%2FpyTooling&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2FpyTooling.github.io%2FpyTooling%2Findex.html)](https://pyTooling.github.io/pyTooling/)
 [![Documentation License](https://img.shields.io/badge/doc-CC--BY%204.0-green?longCache=true&style=flat-square&logo=CreativeCommons&logoColor=fff)](LICENSE.md)  
 [![PyPI](https://img.shields.io/pypi/v/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyTooling/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
```

### Comparing `pytooling-6.2.0/README.md` & `pytooling-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/Argument.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/Argument.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/BooleanFlag.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/BooleanFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/Flag.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/Flag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/ValuedFlag.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/ValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/ArgParse/__init__.py` & `pytooling-6.3.0/pyTooling/Attributes/ArgParse/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Attributes/__init__.py` & `pytooling-6.3.0/pyTooling/Attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/Argument.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/Argument.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/BooleanFlag.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/BooleanFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/Command.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/Command.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/Flag.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/Flag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/KeyValueFlag.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/KeyValueFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlag.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/ValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedFlagList.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/ValuedFlagList.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CLIAbstraction/__init__.py` & `pytooling-6.3.0/pyTooling/CLIAbstraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/CallByRef/__init__.py` & `pytooling-6.3.0/pyTooling/CallByRef/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Common/__init__.py` & `pytooling-6.3.0/pyTooling/Common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 .. hint:: See :ref:`high-level help <COMMON>` for explanations and usage examples.
 """
 __author__ =        "Patrick Lehmann"
 __email__ =         "Paebbels@gmail.com"
 __copyright__ =     "2017-2024, Patrick Lehmann"
 __license__ =       "Apache License, Version 2.0"
-__version__ =       "6.2.0"
+__version__ =       "6.3.0"
 __keywords__ =      ["abstract", "argparse", "attributes", "bfs", "cli", "console", "data structure", "decorators",
 					  "dfs", "exceptions", "generators", "generic library", "generic path", "graph", "installation",
 					  "iterators", "licensing", "message logging", "meta-classes", "overloading", "override", "packaging",
 					  "path", "platform", "setuptools", "shell", "singleton", "slots","terminal", "text user interface",
 					  "timer", "tree", "TUI", "url", "versioning", "wheel"]
 __issue_tracker__ = "https://GitHub.com/pyTooling/pyTooling/issues"
```

### Comparing `pytooling-6.2.0/pyTooling/Configuration/JSON.py` & `pytooling-6.3.0/pyTooling/Configuration/JSON.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Configuration/YAML.py` & `pytooling-6.3.0/pyTooling/Configuration/YAML.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Configuration/__init__.py` & `pytooling-6.3.0/pyTooling/Configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Decorators/__init__.py` & `pytooling-6.3.0/pyTooling/Decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Exceptions/__init__.py` & `pytooling-6.3.0/pyTooling/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/GenericPath/URL.py` & `pytooling-6.3.0/pyTooling/GenericPath/URL.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/GenericPath/__init__.py` & `pytooling-6.3.0/pyTooling/GenericPath/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Graph/GraphML.py` & `pytooling-6.3.0/pyTooling/Graph/GraphML.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Graph/__init__.py` & `pytooling-6.3.0/pyTooling/Graph/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
 			 classDef node fill:#eee,stroke:#777,font-size:smaller;
 """
 import heapq
 from collections import deque
 from itertools   import chain
 from sys         import version_info           # needed for versions before Python 3.11
-from typing      import TypeVar, Generic, Optional as Nullable, Iterable, Hashable, Generator, Callable
-from typing      import List, Union, Dict, Iterator as typing_Iterator, Set, Deque, Tuple
+from typing      import TypeVar, Generic, List, Tuple, Dict, Set, Deque, Union, Optional as Nullable
+from typing      import Callable, Iterator as typing_Iterator, Generator, Iterable, Mapping, Hashable
 
 try:
 	from pyTooling.Decorators  import export, readonly
 	from pyTooling.MetaClasses import ExtendedType
 	from pyTooling.Exceptions  import ToolingException
 	from pyTooling.Common      import getFullyQualifiedName
 	from pyTooling.Tree        import Node
@@ -218,22 +218,26 @@
 
 
 @export
 class Base(
 	Generic[DictKeyType, DictValueType],
 	metaclass=ExtendedType, slots=True
 ):
-	_dict: Dict[DictKeyType, DictValueType]  #: Dictionary to store key-value-pairs.
+	_dict: Dict[DictKeyType, DictValueType]  #: A dictionary to store arbitrary key-value-pairs.
 
-	def __init__(self) -> None:
+	def __init__(
+		self,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Base::init Needs documentation.
 
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
-		self._dict = {}
+		self._dict = {key: value for key, value in keyValuePairs.items()} if keyValuePairs is not None else {}
 
 	def __del__(self):
 		"""
 		.. todo:: GRAPH::Base::del Needs documentation.
 
 		"""
 		try:
@@ -296,20 +300,30 @@
 	Base[DictKeyType, DictValueType],
 	Generic[IDType, ValueType, WeightType, DictKeyType, DictValueType]
 ):
 	_id:        Nullable[IDType]      #: Field storing the object's Identifier.
 	_value:     Nullable[ValueType]   #: Field storing the object's value of any type.
 	_weight:    Nullable[WeightType]  #: Field storing the object's weight.
 
-	def __init__(self, identifier: Nullable[IDType] = None, value: Nullable[ValueType] = None, weight: Nullable[WeightType] = None) -> None:
+	def __init__(
+		self,
+		identifier: Nullable[IDType] = None,
+		value: Nullable[ValueType] = None,
+		weight: Nullable[WeightType] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Vertex::init Needs documentation.
 
+		:param identifier:    The optional unique ID.
+		:param value:         The optional value.
+		:param weight:        The optional weight.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
-		super().__init__()
+		super().__init__(keyValuePairs)
 
 		self._id = identifier
 		self._value = value
 		self._weight = weight
 
 	@readonly
 	def ID(self) -> Nullable[IDType]:
@@ -352,26 +366,32 @@
 @export
 class BaseWithName(
 	Base[DictKeyType, DictValueType],
 	Generic[DictKeyType, DictValueType]
 ):
 	_name: Nullable[str]  #: Field storing the object's name.
 
-	def __init__(self, name: Nullable[str] = None) -> None:
+	def __init__(
+		self,
+		name: Nullable[str] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None,
+	) -> None:
 		"""
 		.. todo:: GRAPH::BaseWithName::init Needs documentation.
 
+		:param name:          The optional name.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
 		if name is not None and not isinstance(name, str):
 			ex = TypeError("Parameter 'name' is not of type 'str'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(name)}'.")
 			raise ex
 
-		super().__init__()
+		super().__init__(keyValuePairs)
 
 		self._name = name
 
 	@property
 	def Name(self) -> Nullable[str]:
 		"""
 		Property to get and set the name (:attr:`_name`).
@@ -409,28 +429,38 @@
 								']'   #: Field storing a reference to the graph.
 	_vertices: Set['Vertex[GraphDictKeyType, GraphDictValueType,'
 								'VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,'
 								'EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,'
 								'LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType'
 								']']  #: Field storing a set of vertices.
 
-	def __init__(self, graph: 'Graph', name: Nullable[str] = None, vertices: Nullable[Iterable['Vertex']] = None) -> None:
+	def __init__(
+		self,
+		graph: 'Graph',
+		name: Nullable[str] = None,
+		vertices: Nullable[Iterable['Vertex']] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Component::init Needs documentation.
 
+		:param graph:         The reference to the graph.
+		:param name:          The optional name.
+		:param vertices:      The optional list of vertices.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
 		if graph is None:
 			raise ValueError("Parameter 'graph' is None.")
-		if not isinstance(graph, Graph):
+		elif not isinstance(graph, Graph):
 			ex = TypeError("Parameter 'graph' is not of type 'Graph'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(graph)}'.")
 			raise ex
 
-		super().__init__(name)
+		super().__init__(name, keyValuePairs)
 
 		self._graph = graph
 		self._vertices = set() if vertices is None else {v for v in vertices}
 
 	def __del__(self):
 		"""
 		.. todo:: GRAPH::BaseWithVertices::del Needs documentation.
@@ -490,26 +520,40 @@
 	_component: 'Component'
 	_views:     Dict[Hashable, 'View']
 	_inboundEdges:   List['Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of inbound edges.
 	_outboundEdges:  List['Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of outbound edges.
 	_inboundLinks:   List['Link[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of inbound links.
 	_outboundLinks:  List['Link[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of outbound links.
 
-	def __init__(self, vertexID: Nullable[VertexIDType] = None, value: Nullable[VertexValueType] = None, weight: Nullable[VertexWeightType] = None, graph: Nullable['Graph'] = None, subgraph: Nullable['Subgraph'] = None) -> None:
+	def __init__(
+		self,
+		vertexID: Nullable[VertexIDType] = None,
+		value: Nullable[VertexValueType] = None,
+		weight: Nullable[VertexWeightType] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None,
+		graph: Nullable['Graph'] = None,
+		subgraph: Nullable['Subgraph'] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Vertex::init Needs documentation.
 
+		:param vertexID:      The optional ID for the new vertex.
+		:param value:         The optional value for the new vertex.
+		:param weight:        The optional weight for the new vertex.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
+		:param graph:         The optional reference to the graph.
+		:param subgraph:      undocumented
 		"""
 		if vertexID is not None and not isinstance(vertexID, Hashable):
 			ex = TypeError("Parameter 'vertexID' is not of type 'VertexIDType'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(vertexID)}'.")
 			raise ex
 
-		super().__init__(vertexID, value, weight)
+		super().__init__(vertexID, value, weight, keyValuePairs)
 
 		if subgraph is None:
 			self._graph = graph if graph is not None else Graph()
 			self._subgraph = None
 			self._component = Component(self._graph, vertices=(self,))
 
 			if vertexID is None:
@@ -1602,20 +1646,34 @@
 	"""
 	An **edge** can have a unique ID, a value, a weight and attached meta information as key-value-pairs. All edges are
 	directed.
 	"""
 	_source:      Vertex
 	_destination: Vertex
 
-	def __init__(self, source: Vertex, destination: Vertex, edgeID: Nullable[EdgeIDType] = None, value: Nullable[EdgeValueType] = None, weight: Nullable[EdgeWeightType] = None) -> None:
+	def __init__(
+		self,
+		source: Vertex,
+		destination: Vertex,
+		edgeID: Nullable[EdgeIDType] = None,
+		value: Nullable[EdgeValueType] = None,
+		weight: Nullable[EdgeWeightType] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::BaseEdge::init Needs documentation.
 
+		:param source:        The source of the new edge.
+		:param destination:   The destination of the new edge.
+		:param edgeID:        The optional unique ID for the new edge.
+		:param value:         The optional value for the new edge.
+		:param weight:        The optional weight for the new edge.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
-		super().__init__(edgeID, value, weight)
+		super().__init__(edgeID, value, weight, keyValuePairs)
 
 		self._source = source
 		self._destination = destination
 
 		component = source._component
 		if component is not destination._component:
 			# TODO: should it be divided into with/without ID?
@@ -1657,18 +1715,32 @@
 	Generic[EdgeIDType, EdgeValueType, EdgeWeightType, EdgeDictKeyType, EdgeDictValueType]
 ):
 	"""
 	An **edge** can have a unique ID, a value, a weight and attached meta information as key-value-pairs. All edges are
 	directed.
 	"""
 
-	def __init__(self, source: Vertex, destination: Vertex, edgeID: Nullable[EdgeIDType] = None, value: Nullable[EdgeValueType] = None, weight: Nullable[EdgeWeightType] = None) -> None:
+	def __init__(
+		self,
+		source: Vertex,
+		destination: Vertex,
+		edgeID: Nullable[EdgeIDType] = None,
+		value: Nullable[EdgeValueType] = None,
+		weight: Nullable[EdgeWeightType] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Edge::init Needs documentation.
 
+		:param source:        The source of the new edge.
+		:param destination:   The destination of the new edge.
+		:param edgeID:        The optional unique ID for the new edge.
+		:param value:         The optional value for the new edge.
+		:param weight:        The optional weight for the new edge.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
 		if not isinstance(source, Vertex):
 			ex = TypeError("Parameter 'source' is not of type 'Vertex'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(source)}'.")
 			raise ex
 		if not isinstance(destination, Vertex):
@@ -1687,15 +1759,15 @@
 			ex = TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(weight)}'.")
 			raise ex
 		if source._graph is not destination._graph:
 			raise NotInSameGraph(f"Source vertex and destination vertex are not in same graph.")
 
-		super().__init__(source, destination, edgeID, value, weight)
+		super().__init__(source, destination, edgeID, value, weight, keyValuePairs)
 
 	def Delete(self) -> None:
 		# Remove from Source and Destination
 		self._source._outboundEdges.remove(self)
 		self._destination._inboundEdges.remove(self)
 
 		# Remove from Graph and Subgraph
@@ -1729,18 +1801,32 @@
 	Generic[LinkIDType, LinkValueType, LinkWeightType, LinkDictKeyType, LinkDictValueType]
 ):
 	"""
 	A **link** can have a unique ID, a value, a weight and attached meta information as key-value-pairs. All links are
 	directed.
 	"""
 
-	def __init__(self, source: Vertex, destination: Vertex, linkID: LinkIDType = None, value: LinkValueType = None, weight: Nullable[LinkWeightType] = None) -> None:
+	def __init__(
+		self,
+		source: Vertex,
+		destination: Vertex,
+		linkID: LinkIDType = None,
+		value: LinkValueType = None,
+		weight: Nullable[LinkWeightType] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Edge::init Needs documentation.
 
+		:param source:        The source of the new link.
+		:param destination:   The destination of the new link.
+		:param linkID:        The optional unique ID for the new link.
+		:param value:         The optional value for the new v.
+		:param weight:        The optional weight for the new link.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
 		if not isinstance(source, Vertex):
 			ex = TypeError("Parameter 'source' is not of type 'Vertex'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(source)}'.")
 			raise ex
 		if not isinstance(destination, Vertex):
@@ -1759,15 +1845,15 @@
 			ex = TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(weight)}'.")
 			raise ex
 		if source._graph is not destination._graph:
 			raise NotInSameGraph(f"Source vertex and destination vertex are not in same graph.")
 
-		super().__init__(source, destination, linkID, value, weight)
+		super().__init__(source, destination, linkID, value, weight, keyValuePairs)
 
 	def Delete(self) -> None:
 		self._source._outboundEdges.remove(self)
 		self._destination._inboundEdges.remove(self)
 
 		if self._id is None:
 			self._source._graph._linksWithoutID.remove(self)
@@ -1808,20 +1894,27 @@
 	_verticesWithID:    Dict[VertexIDType, Vertex[GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_verticesWithoutID: List[Vertex[GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_edgesWithID:       Dict[EdgeIDType, Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]]
 	_edgesWithoutID:    List[Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]]
 	_linksWithID:       Dict[EdgeIDType, Link[LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_linksWithoutID:    List[Link[LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 
-	def __init__(self, name: Nullable[str] = None):  #, vertices: Nullable[Iterable[Vertex]] = None) -> None:
+	def __init__(
+		self,
+		name: Nullable[str] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+		#, vertices: Nullable[Iterable[Vertex]] = None) -> None:
+	):
 		"""
 		.. todo:: GRAPH::BaseGraph::init Needs documentation.
 
+		:param name:          The optional name of the graph.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
-		super().__init__(name)
+		super().__init__(name, keyValuePairs)
 
 		self._verticesWithoutID = []
 		self._verticesWithID = {}
 		self._edgesWithoutID = []
 		self._edgesWithID = {}
 		self._linksWithoutID = []
 		self._linksWithID = {}
@@ -2294,28 +2387,37 @@
 	"""
 	.. todo:: GRAPH::Subgraph Needs documentation.
 
 	"""
 
 	_graph:    'Graph'
 
-	def __init__(self, graph: 'Graph', name: Nullable[str] = None, vertices: Nullable[Iterable[Vertex]] = None) -> None:
+	def __init__(
+		self,
+		graph: 'Graph',
+		name: Nullable[str] = None,
+		# vertices: Nullable[Iterable[Vertex]] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Subgraph::init Needs documentation.
 
+		:param graph:         The reference to the graph.
+		:param name:          The optional name of the new sub-graph.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
 		if graph is None:
 			raise ValueError("Parameter 'graph' is None.")
 		if not isinstance(graph, Graph):
 			ex = TypeError("Parameter 'graph' is not of type 'Graph'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(graph)}'.")
 			raise ex
 
-		super().__init__(name)
+		super().__init__(name, keyValuePairs)
 
 		graph._subgraphs.add(self)
 
 		self._graph = graph
 
 	def __del__(self):
 		"""
@@ -2359,20 +2461,30 @@
 	]
 ):
 	"""
 	.. todo:: GRAPH::View Needs documentation.
 
 	"""
 
-	def __init__(self, graph: 'Graph', name: Nullable[str] = None, vertices: Nullable[Iterable[Vertex]] = None) -> None:
+	def __init__(
+		self,
+		graph: 'Graph',
+		name: Nullable[str] = None,
+		vertices: Nullable[Iterable[Vertex]] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::View::init Needs documentation.
 
+		:param graph:         The reference to the graph.
+		:param name:          The optional name of the new view.
+		:param vertices:      The optional list of vertices in the new view.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
-		super().__init__(graph, name, vertices)
+		super().__init__(graph, name, vertices, keyValuePairs)
 
 		graph._views.add(self)
 
 	def __del__(self):
 		"""
 		.. todo:: GRAPH::View::del Needs documentation.
 
@@ -2405,20 +2517,30 @@
 	]
 ):
 	"""
 	.. todo:: GRAPH::Component Needs documentation.
 
 	"""
 
-	def __init__(self, graph: 'Graph', name: Nullable[str] = None, vertices: Nullable[Iterable[Vertex]] = None) -> None:
+	def __init__(
+		self,
+		graph: 'Graph',
+		name: Nullable[str] = None,
+		vertices: Nullable[Iterable[Vertex]] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Component::init Needs documentation.
 
+		:param graph:         The reference to the graph.
+		:param name:          The optional name of the new component.
+		:param vertices:      The optional list of vertices in the new component.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
 		"""
-		super().__init__(graph, name, vertices)
+		super().__init__(graph, name, vertices, keyValuePairs)
 
 		graph._components.add(self)
 
 	def __del__(self):
 		"""
 		.. todo:: GRAPH::Component::del Needs documentation.
 
@@ -2456,20 +2578,26 @@
 	all nodes. Nodes are instances of :class:`~pyTooling.Graph.Vertex` classes and directed links between nodes are
 	made of :class:`~pyTooling.Graph.Edge` instances. A graph can have attached meta information as key-value-pairs.
 	"""
 	_subgraphs:         Set[Subgraph[SubgraphDictKeyType, SubgraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_views:             Set[View[ViewDictKeyType, ViewDictValueType, GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_components:        Set[Component[ComponentDictKeyType, ComponentDictValueType, GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 
-	def __init__(self, name: Nullable[str] = None) -> None:
+	def __init__(
+		self,
+		name: Nullable[str] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None
+	) -> None:
 		"""
 		.. todo:: GRAPH::Graph::init Needs documentation.
 
+		:param name:          The optional name of the new graph.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.#
 		"""
-		super().__init__(name)
+		super().__init__(name, keyValuePairs)
 
 		self._subgraphs = set()
 		self._views = set()
 		self._components = set()
 
 	def __del__(self):
 		"""
```

### Comparing `pytooling-6.2.0/pyTooling/Licensing/__init__.py` & `pytooling-6.3.0/pyTooling/Licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/MetaClasses/__init__.py` & `pytooling-6.3.0/pyTooling/MetaClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Packaging/__init__.py` & `pytooling-6.3.0/pyTooling/Packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Platform/__init__.py` & `pytooling-6.3.0/pyTooling/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/StateMachine/__init__.py` & `pytooling-6.3.0/pyTooling/StateMachine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/TerminalUI/__init__.py` & `pytooling-6.3.0/pyTooling/TerminalUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Timer/__init__.py` & `pytooling-6.3.0/pyTooling/Timer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling/Tree/__init__.py` & `pytooling-6.3.0/pyTooling/Tree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """A powerful tree data structure for Python."""
 from collections   import deque
 from sys           import version_info           # needed for versions before Python 3.11
-from typing        import List, Generator, Iterable, TypeVar, Generic, Dict, Optional as Nullable, Hashable, Tuple, Callable, Union, Deque, Iterator
+from typing        import TypeVar, Generic, List, Tuple, Dict, Deque, Union, Optional as Nullable
+from typing        import Callable, Iterator, Generator, Iterable, Mapping, Hashable
 
 try:
 	from pyTooling.Decorators  import export, readonly
 	from pyTooling.MetaClasses import ExtendedType
 	from pyTooling.Exceptions  import ToolingException
 	from pyTooling.Common      import getFullyQualifiedName
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
@@ -158,22 +159,46 @@
 	_children: List['Node']                       #: List of all children
 #	_links: List['Node']
 
 	_level: int                                   #: Level of the node (distance to the root).
 	_value: Nullable[ValueType]                   #: Field to store the node's value.
 	_dict: Dict[DictKeyType, DictValueType]       #: Dictionary to store key-value-pairs attached to the node.
 
-	def __init__(self, nodeID: Nullable[IDType] = None, value: Nullable[ValueType] = None, parent: 'Node' = None, children: Nullable[List['Node']] = None) -> None:
+	_format: Nullable[Callable[["Node"], str]]    #: A node formatting function returning a one-line representation for tree-rendering.
+
+	def __init__(
+		self,
+		nodeID: Nullable[IDType] = None,
+		value: Nullable[ValueType] = None,
+		keyValuePairs: Nullable[Mapping[DictKeyType, DictValueType]] = None,
+		parent: 'Node' = None,
+		children: Nullable[Iterable['Node']] = None,
+		format: Nullable[Callable[["Node"], str]] = None
+	) -> None:
 		"""
 		.. todo:: TREE::Node::init Needs documentation.
 
+		:param nodeID:        The optional unique ID of a node within the whole tree data structure.
+		:param value:         The optional value of the node.
+		:param keyValuePairs: The optional mapping (dictionary) of key-value-pairs.
+		:param parent:        The optional parent node in the tree.
+		:param children:      The optional list of child nodes.
+		:param format:        The optional node formatting function returning a one-line representation for tree-rendering.
+
+		:raises TypeError:    If parameter parent is not an instance of Node.
+		:raises ValueError:   If nodeID already exists in the tree.
+		:raises TypeError:    If parameter children is not iterable.
+		:raises ValueError:   If an element of children is not an instance of Node.
 		"""
+
 		self._id = nodeID
 		self._value = value
-		self._dict = {}
+		self._dict = {key: value for key, value in keyValuePairs.items()} if keyValuePairs is not None else {}
+
+		self._format = format
 
 		if parent is not None and not isinstance(parent, Node):
 			ex = TypeError(f"Parameter 'parent' is not of type 'Node'.")
 			if version_info >= (3, 11):  # pragma: no cover
 				ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
 			raise ex
 
@@ -200,15 +225,14 @@
 				raise ValueError(f"ID '{nodeID}' already exists in this tree.")
 			else:
 				self._root._nodesWithID[nodeID] = self
 
 			parent._children.append(self)
 
 		self._children = []
-
 		if children is not None:
 			if not isinstance(children, Iterable):
 				ex = TypeError(f"Parameter 'children' is not iterable.")
 				if version_info >= (3, 11):  # pragma: no cover
 					ex.add_note(f"Got type '{getFullyQualifiedName(children)}'.")
 				raise ex
 
@@ -937,42 +961,50 @@
 		if self._value is not None:
 			return str(self._value)
 		elif self._id is not None:
 			return str(self._id)
 		else:
 			return self.__repr__()
 
-	def Render(self, prefix: str = "", lineend: str = "\n", nodeMarker: str = "o-- ", bypassMarker: str = "|   ") -> str:
+	def Render(
+		self,
+		prefix: str = "",
+		lineend: str = "\n",
+		nodeMarker: str = "├─",
+		lastNodeMarker: str = "└─",
+		bypassMarker: str = "│ "
+	) -> str:
 		"""
 		Render the tree as ASCII art.
 
-		:param prefix:       A string printed in front of every line, e.g. for indentation. Default: ``""``.
-		:param lineend:      A string printed at the end of every line. Default: ``"\\n"``.
-		:param nodeMarker:   A string printed before every tree node. Default: ``"o-- "``.
-		:param bypassMarker: A string printed when there are further nodes in the parent level. Default: ``"|   "``.
-		:return:             A rendered tree as multiline string.
+		:param prefix:         A string printed in front of every line, e.g. for indentation. Default: ``""``.
+		:param lineend:        A string printed at the end of every line. Default: ``"\\n"``.
+		:param nodeMarker:     A string printed before every non-last tree node. Default: ``"├─"``.
+		:param lastNodeMarker: A string printed before every last tree node. Default: ``"└─"``.
+		:param bypassMarker:   A string printed when there are further nodes in the parent level. Default: ``"│ "``.
+		:return:               A rendered tree as multiline string.
 		"""
 		emptyMarker = " " * len(bypassMarker)
 
 		def _render(node: Node, markers: str):
 			result = []
 
 			if node.HasChildren:
 				for child in node._children[:-1]:
-					result.append(f"{prefix}{markers}{nodeMarker}{child}{lineend}")
+					nodeRepresentation = child._format(child) if child._format else str(child)
+					result.append(f"{prefix}{markers}{nodeMarker}{nodeRepresentation}{lineend}")
 					result.extend(_render(child, markers + bypassMarker))
-				result.append(f"{prefix}{markers}{nodeMarker}{node._children[-1]}{lineend}")
-				result.extend(_render(node._children[-1], markers + emptyMarker))
+
+				# last child node
+				child = node._children[-1]
+				nodeRepresentation = child._format(child) if child._format else str(child)
+				result.append(f"{prefix}{markers}{lastNodeMarker}{nodeRepresentation}{lineend}")
+				result.extend(_render(child, markers + emptyMarker))
 
 			return result
 
 		# Root element
-		result = [f"{prefix}{self}{lineend}"]
-
-		if self.HasChildren:
-			for child in self._children[:-1]:
-				result.append(f"{prefix}{nodeMarker}{child}{lineend}")
-				result.extend(_render(child, bypassMarker))
-			result.append(f"{prefix}{nodeMarker}{self._children[-1]}{lineend}")
-			result.extend(_render(self._children[-1], emptyMarker))
+		nodeRepresentation = self._format(self) if self._format else str(self)
+		result = [f"{prefix}{nodeRepresentation}{lineend}"]
+		result.extend(_render(self, ""))
 
 		return "".join(result)
```

### Comparing `pytooling-6.2.0/pyTooling/Versioning/__init__.py` & `pytooling-6.3.0/pyTooling/Versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyTooling.egg-info/PKG-INFO` & `pytooling-6.3.0/pyTooling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 6.2.0
+Version: 6.3.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -21,65 +21,65 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: doc
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: docutils~=0.18.0; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: docutils~=0.18.0; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: setuptools~=70.0; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
 Provides-Extra: test
+Requires-Dist: typing_extensions~=4.12; extra == "test"
+Requires-Dist: colorama>=0.4.6; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: pytest~=8.2; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: typing_extensions~=4.11; extra == "test"
-Requires-Dist: colorama>=0.4.6; extra == "test"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
 Provides-Extra: packaging
 Requires-Dist: setuptools>=69.0.0; extra == "packaging"
 Provides-Extra: terminal
 Requires-Dist: colorama>=0.4.6; extra == "terminal"
 Provides-Extra: yaml
 Requires-Dist: ruamel.yaml>=0.18; extra == "yaml"
 Provides-Extra: all
+Requires-Dist: sphinx~=7.3; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: docutils~=0.18.0; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
-Requires-Dist: mypy~=1.10; extra == "all"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
 Requires-Dist: setuptools>=69.0.0; extra == "all"
+Requires-Dist: docutils~=0.18.0; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: setuptools~=70.0; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: typing_extensions~=4.12; extra == "all"
 Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: ruamel.yaml>=0.18; extra == "all"
 Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
+Requires-Dist: mypy~=1.10; extra == "all"
 Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyTooling-pyTooling-63bf7f.svg?longCache=true&style=flat-square&longCache=true&logo=GitHub)](https://GitHub.com/pyTooling/pyTooling)
 [![Sourcecode License](https://img.shields.io/pypi/l/pyTooling?longCache=true&style=flat-square&logo=Apache&label=code)](LICENSE.md)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=pyTooling.github.io%2FpyTooling&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2FpyTooling.github.io%2FpyTooling%2Findex.html)](https://pyTooling.github.io/pyTooling/)
 [![Documentation License](https://img.shields.io/badge/doc-CC--BY%204.0-green?longCache=true&style=flat-square&logo=CreativeCommons&logoColor=fff)](LICENSE.md)  
 [![PyPI](https://img.shields.io/pypi/v/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyTooling/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
```

### Comparing `pytooling-6.2.0/pyTooling.egg-info/SOURCES.txt` & `pytooling-6.3.0/pyTooling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/pyproject.toml` & `pytooling-6.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytooling-6.2.0/setup.py` & `pytooling-6.3.0/setup.py`

 * *Files identical despite different names*

