# Comparing `tmp/homelab_assistant-0.1.tar.gz` & `tmp/homelab_assistant-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homelab_assistant-0.1.tar", last modified: Thu May 30 11:09:08 2024, max compression
+gzip compressed data, was "homelab_assistant-1.0.tar", last modified: Sun Jun  2 10:52:08 2024, max compression
```

## Comparing `homelab_assistant-0.1.tar` & `homelab_assistant-1.0.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxr-xr-x   0 jono      (1000) jono      (1000)        0 2024-05-30 11:09:08.108501 homelab_assistant-0.1/
--rw-r--r--   0 jono      (1000) jono      (1000)    35149 2024-05-30 11:07:57.000000 homelab_assistant-0.1/LICENSE
--rw-r--r--   0 jono      (1000) jono      (1000)      115 2024-05-30 11:09:08.108501 homelab_assistant-0.1/PKG-INFO
-drwxr-xr-x   0 jono      (1000) jono      (1000)        0 2024-05-30 11:09:08.108501 homelab_assistant-0.1/homelab_assistant.egg-info/
--rw-r--r--   0 jono      (1000) jono      (1000)      115 2024-05-30 11:09:08.000000 homelab_assistant-0.1/homelab_assistant.egg-info/PKG-INFO
--rw-r--r--   0 jono      (1000) jono      (1000)      186 2024-05-30 11:09:08.000000 homelab_assistant-0.1/homelab_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 jono      (1000) jono      (1000)        1 2024-05-30 11:09:08.000000 homelab_assistant-0.1/homelab_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 jono      (1000) jono      (1000)        1 2024-05-30 11:09:08.000000 homelab_assistant-0.1/homelab_assistant.egg-info/top_level.txt
--rw-r--r--   0 jono      (1000) jono      (1000)       94 2024-05-30 11:08:39.000000 homelab_assistant-0.1/pyproject.toml
--rw-r--r--   0 jono      (1000) jono      (1000)       38 2024-05-30 11:09:08.108501 homelab_assistant-0.1/setup.cfg
+drwxr-xr-x   0 jono      (1000) jono      (1000)        0 2024-06-02 10:52:08.983606 homelab_assistant-1.0/
+-rw-r--r--   0 jono      (1000) jono      (1000)    35149 2024-06-01 07:50:12.000000 homelab_assistant-1.0/LICENSE
+-rw-r--r--   0 jono      (1000) jono      (1000)      363 2024-06-02 10:52:08.917046 homelab_assistant-1.0/PKG-INFO
+drwxr-xr-x   0 jono      (1000) jono      (1000)        0 2024-06-02 10:52:08.658486 homelab_assistant-1.0/homelab_assistant/
+-rw-r--r--   0 jono      (1000) jono      (1000)        0 2024-06-02 10:01:28.000000 homelab_assistant-1.0/homelab_assistant/__init__.py
+-rw-r--r--   0 jono      (1000) jono      (1000)     1495 2024-06-02 10:01:20.000000 homelab_assistant-1.0/homelab_assistant/main.py
+-rw-r--r--   0 jono      (1000) jono      (1000)     6333 2024-06-02 09:52:35.000000 homelab_assistant-1.0/homelab_assistant/portainer.py
+drwxr-xr-x   0 jono      (1000) jono      (1000)        0 2024-06-02 10:52:08.910045 homelab_assistant-1.0/homelab_assistant.egg-info/
+-rw-r--r--   0 jono      (1000) jono      (1000)      363 2024-06-02 10:52:08.000000 homelab_assistant-1.0/homelab_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 jono      (1000) jono      (1000)      357 2024-06-02 10:52:08.000000 homelab_assistant-1.0/homelab_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 jono      (1000) jono      (1000)        1 2024-06-02 10:52:08.000000 homelab_assistant-1.0/homelab_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 jono      (1000) jono      (1000)       57 2024-06-02 10:52:08.000000 homelab_assistant-1.0/homelab_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 jono      (1000) jono      (1000)       57 2024-06-02 10:52:08.000000 homelab_assistant-1.0/homelab_assistant.egg-info/requires.txt
+-rw-r--r--   0 jono      (1000) jono      (1000)       18 2024-06-02 10:52:08.000000 homelab_assistant-1.0/homelab_assistant.egg-info/top_level.txt
+-rw-r--r--   0 jono      (1000) jono      (1000)     3111 2024-06-02 10:51:09.000000 homelab_assistant-1.0/pyproject.toml
+-rw-r--r--   0 jono      (1000) jono      (1000)       38 2024-06-02 10:52:08.984575 homelab_assistant-1.0/setup.cfg
```

### Comparing `homelab_assistant-0.1/LICENSE` & `homelab_assistant-1.0/LICENSE`

 * *Files identical despite different names*

