# Comparing `tmp/LLM-Toolbox-0.1.9.tar.gz` & `tmp/llm_toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.9.tar", last modified: Mon Jul 24 01:22:06 2023, max compression
+gzip compressed data, was "llm_toolbox-0.2.0.tar", last modified: Sun Jun  2 07:10:50 2024, max compression
```

## Comparing `LLM-Toolbox-0.1.9.tar` & `llm_toolbox-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,11 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.9/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-07-24 01:22:06.000000 LLM-Toolbox-0.1.9/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17200 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16662 2023-06-28 10:02:44.000000 LLM-Toolbox-0.1.9/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.9/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15930 2023-07-24 01:18:04.000000 LLM-Toolbox-0.1.9/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      832 2023-07-24 01:14:52.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/life.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.9/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-24 01:22:06.266284 LLM-Toolbox-0.1.9/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2178 2023-07-24 01:21:02.000000 LLM-Toolbox-0.1.9/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-06-02 07:10:50.127624 llm_toolbox-0.2.0/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      356 2024-06-02 07:10:50.117624 llm_toolbox-0.2.0/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      150 2024-06-02 06:47:41.000000 llm_toolbox-0.2.0/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-06-02 07:10:50.117624 llm_toolbox-0.2.0/llm_toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      356 2024-06-02 07:10:50.000000 llm_toolbox-0.2.0/llm_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      192 2024-06-02 07:10:50.000000 llm_toolbox-0.2.0/llm_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2024-06-02 07:10:50.000000 llm_toolbox-0.2.0/llm_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       10 2024-06-02 07:10:50.000000 llm_toolbox-0.2.0/llm_toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2024-06-02 07:10:50.000000 llm_toolbox-0.2.0/llm_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2024-06-02 07:10:50.127624 llm_toolbox-0.2.0/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      537 2024-06-02 06:47:41.000000 llm_toolbox-0.2.0/setup.py
```

