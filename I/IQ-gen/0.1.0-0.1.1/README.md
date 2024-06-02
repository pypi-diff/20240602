# Comparing `tmp/iq_gen-0.1.0.tar.gz` & `tmp/iq_gen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iq_gen-0.1.0.tar", last modified: Tue May 21 04:37:57 2024, max compression
+gzip compressed data, was "iq_gen-0.1.1.tar", last modified: Sun Jun  2 14:09:07 2024, max compression
```

## Comparing `iq_gen-0.1.0.tar` & `iq_gen-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-08 23:41:29.093384 iq_gen-0.1.0/LICENSE
--rw-r--r--   0        0        0      974 2024-05-08 23:45:05.647705 iq_gen-0.1.0/README.md
--rw-r--r--   0        0        0      568 2024-05-21 04:37:57.183714 iq_gen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-21 03:58:16.677821 iq_gen-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     4805 2024-05-08 23:37:40.021800 iq_gen-0.1.0/src/app.py
--rw-r--r--   0        0        0     8582 2024-05-08 23:37:40.022152 iq_gen-0.1.0/src/sentiment_text_helpers.py
--rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 iq_gen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3298 2024-06-02 13:51:49.934366 iq_gen-0.1.1/README.md
+-rw-r--r--   0        0        0      473 2024-06-02 14:09:07.283593 iq_gen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 14:08:13.975406 iq_gen-0.1.1/src/iq_gen/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:08:13.974368 iq_gen-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 iq_gen-0.1.1/PKG-INFO
```

