# Comparing `tmp/Starco-3.3.1.tar.gz` & `tmp/Starco-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Starco-3.3.1.tar", last modified: Fri May 31 21:04:17 2024, max compression
+gzip compressed data, was "Starco-3.3.2.tar", last modified: Sat Jun  1 22:29:15 2024, max compression
```

## Comparing `Starco-3.3.1.tar` & `Starco-3.3.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.855523 Starco-3.3.1/
--rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-05-31 21:04:17.855523 Starco-3.3.1/PKG-INFO
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/Starco.egg-info/
--rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-05-31 21:04:17.000000 Starco-3.3.1/Starco.egg-info/PKG-INFO
--rw-rw-r--   0 starco    (1000) starco    (1000)     1274 2024-05-31 21:04:17.000000 Starco-3.3.1/Starco.egg-info/SOURCES.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)        1 2024-05-31 21:04:17.000000 Starco-3.3.1/Starco.egg-info/dependency_links.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)      359 2024-05-31 21:04:17.000000 Starco-3.3.1/Starco.egg-info/requires.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)        7 2024-05-31 21:04:17.000000 Starco-3.3.1/Starco.egg-info/top_level.txt
--rw-rw-r--   0 starco    (1000) starco    (1000)       38 2024-05-31 21:04:17.855523 Starco-3.3.1/setup.cfg
--rw-rw-r--   0 starco    (1000) starco    (1000)      776 2024-05-31 21:04:07.000000 Starco-3.3.1/setup.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/
--rw-rw-r--   0 starco    (1000) starco    (1000)       15 2023-11-10 08:57:48.000000 Starco-3.3.1/starco/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/cloudflare/
--rw-rw-r--   0 starco    (1000) starco    (1000)     4060 2023-12-25 11:56:49.000000 Starco-3.3.1/starco/cloudflare/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/crypto_gates/
--rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-17 13:29:58.000000 Starco-3.3.1/starco/crypto_gates/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/crypto_gates/nowpayments/
--rw-rw-r--   0 starco    (1000) starco    (1000)      586 2023-12-17 13:30:45.000000 Starco-3.3.1/starco/crypto_gates/nowpayments/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/db/
--rw-rw-r--   0 starco    (1000) starco    (1000)     3601 2023-11-27 16:38:44.000000 Starco-3.3.1/starco/db/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/debug/
--rw-rw-r--   0 starco    (1000) starco    (1000)     1051 2023-12-01 08:39:29.000000 Starco-3.3.1/starco/debug/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/gateways/
--rw-rw-r--   0 starco    (1000) starco    (1000)     1426 2023-12-11 14:39:40.000000 Starco-3.3.1/starco/gateways/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/gateways/gates/
--rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-11 12:22:45.000000 Starco-3.3.1/starco/gateways/gates/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1675 2023-12-23 09:24:08.000000 Starco-3.3.1/starco/gateways/gates/aqayepardakht.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     3382 2023-12-23 09:24:40.000000 Starco-3.3.1/starco/gateways/gates/idpay.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1950 2023-12-23 09:24:43.000000 Starco-3.3.1/starco/gateways/gates/nextpay.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1140 2023-12-23 09:24:28.000000 Starco-3.3.1/starco/gateways/gates/utils.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1826 2023-12-23 09:24:48.000000 Starco-3.3.1/starco/gateways/gates/vandar.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1182 2023-12-23 09:24:49.000000 Starco-3.3.1/starco/gateways/gates/zibalpay.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/gui/
--rw-rw-r--   0 starco    (1000) starco    (1000)     9174 2024-03-31 08:39:11.000000 Starco-3.3.1/starco/gui/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)    32861 2024-03-16 18:40:57.000000 Starco-3.3.1/starco/gui/utils.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/hetzner/
--rw-rw-r--   0 starco    (1000) starco    (1000)     6113 2023-12-25 18:28:35.000000 Starco-3.3.1/starco/hetzner/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/pkl/
--rw-rw-r--   0 starco    (1000) starco    (1000)     2208 2023-11-10 08:07:45.000000 Starco-3.3.1/starco/pkl/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/proxy/
--rw-rw-r--   0 starco    (1000) starco    (1000)     2248 2023-12-01 08:40:12.000000 Starco-3.3.1/starco/proxy/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/scraper/
--rw-rw-r--   0 starco    (1000) starco    (1000)     1693 2024-05-03 15:02:33.000000 Starco-3.3.1/starco/scraper/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/tlg/
--rw-rw-r--   0 starco    (1000) starco    (1000)       35 2024-01-09 13:06:48.000000 Starco-3.3.1/starco/tlg/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/tlg/app/
--rw-rw-r--   0 starco    (1000) starco    (1000)    39525 2024-05-31 11:17:26.000000 Starco-3.3.1/starco/tlg/app/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      812 2024-01-09 13:06:48.000000 Starco-3.3.1/starco/tlg/app/utils.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.851523 Starco-3.3.1/starco/tlg/bot/
--rw-rw-r--   0 starco    (1000) starco    (1000)     6829 2024-05-31 19:41:33.000000 Starco-3.3.1/starco/tlg/bot/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)    47327 2024-01-09 14:36:18.000000 Starco-3.3.1/starco/tlg/bot/base.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     3146 2024-01-09 13:06:48.000000 Starco-3.3.1/starco/tlg/bot/classes.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.855523 Starco-3.3.1/starco/tlg/bot/util/
--rw-rw-r--   0 starco    (1000) starco    (1000)        0 2024-01-09 13:06:48.000000 Starco-3.3.1/starco/tlg/bot/util/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      849 2024-01-11 11:40:27.000000 Starco-3.3.1/starco/tlg/bot/util/enum.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     4701 2024-01-09 13:06:48.000000 Starco-3.3.1/starco/tlg/bot/util/filteres.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     5494 2024-02-24 13:19:42.000000 Starco-3.3.1/starco/tlg/bot/util/functions.py
--rw-rw-r--   0 starco    (1000) starco    (1000)    35667 2024-02-24 13:21:45.000000 Starco-3.3.1/starco/tlg/bot/util/packs.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.855523 Starco-3.3.1/starco/utils/
--rw-rw-r--   0 starco    (1000) starco    (1000)      125 2023-12-25 07:41:52.000000 Starco-3.3.1/starco/utils/__init__.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1122 2024-05-31 16:20:17.000000 Starco-3.3.1/starco/utils/directories.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1469 2024-02-24 13:20:03.000000 Starco-3.3.1/starco/utils/ext.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     1323 2023-12-06 19:14:01.000000 Starco-3.3.1/starco/utils/scheduler.py
--rw-rw-r--   0 starco    (1000) starco    (1000)      823 2024-03-24 07:26:00.000000 Starco-3.3.1/starco/utils/structures.py
--rw-rw-r--   0 starco    (1000) starco    (1000)     2247 2024-01-01 09:30:33.000000 Starco-3.3.1/starco/utils/time.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.855523 Starco-3.3.1/starco/wp_api/
--rw-rw-r--   0 starco    (1000) starco    (1000)     4370 2023-12-15 13:34:21.000000 Starco-3.3.1/starco/wp_api/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.855523 Starco-3.3.1/starco/wscraper/
--rw-rw-r--   0 starco    (1000) starco    (1000)     8229 2024-05-31 20:12:12.000000 Starco-3.3.1/starco/wscraper/__init__.py
-drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-05-31 21:04:17.855523 Starco-3.3.1/starco/xray_connctor/
--rw-rw-r--   0 starco    (1000) starco    (1000)    10800 2024-05-10 20:32:56.000000 Starco-3.3.1/starco/xray_connctor/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/
+-rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-06-01 22:29:15.366605 Starco-3.3.2/PKG-INFO
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/Starco.egg-info/
+-rw-r--r--   0 starco    (1000) starco    (1000)      795 2024-06-01 22:29:15.000000 Starco-3.3.2/Starco.egg-info/PKG-INFO
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1274 2024-06-01 22:29:15.000000 Starco-3.3.2/Starco.egg-info/SOURCES.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)        1 2024-06-01 22:29:15.000000 Starco-3.3.2/Starco.egg-info/dependency_links.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)      359 2024-06-01 22:29:15.000000 Starco-3.3.2/Starco.egg-info/requires.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)        7 2024-06-01 22:29:15.000000 Starco-3.3.2/Starco.egg-info/top_level.txt
+-rw-rw-r--   0 starco    (1000) starco    (1000)       38 2024-06-01 22:29:15.366605 Starco-3.3.2/setup.cfg
+-rw-rw-r--   0 starco    (1000) starco    (1000)      776 2024-06-01 22:26:24.000000 Starco-3.3.2/setup.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/
+-rw-rw-r--   0 starco    (1000) starco    (1000)       15 2023-11-10 08:57:48.000000 Starco-3.3.2/starco/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/cloudflare/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     4060 2023-12-25 11:56:49.000000 Starco-3.3.2/starco/cloudflare/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/crypto_gates/
+-rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-17 13:29:58.000000 Starco-3.3.2/starco/crypto_gates/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/crypto_gates/nowpayments/
+-rw-rw-r--   0 starco    (1000) starco    (1000)      586 2023-12-17 13:30:45.000000 Starco-3.3.2/starco/crypto_gates/nowpayments/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/db/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     3601 2023-11-27 16:38:44.000000 Starco-3.3.2/starco/db/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/debug/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1051 2023-12-01 08:39:29.000000 Starco-3.3.2/starco/debug/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/gateways/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1426 2023-12-11 14:39:40.000000 Starco-3.3.2/starco/gateways/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/gateways/gates/
+-rw-rw-r--   0 starco    (1000) starco    (1000)        0 2023-12-11 12:22:45.000000 Starco-3.3.2/starco/gateways/gates/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1675 2023-12-23 09:24:08.000000 Starco-3.3.2/starco/gateways/gates/aqayepardakht.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     3382 2023-12-23 09:24:40.000000 Starco-3.3.2/starco/gateways/gates/idpay.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1950 2023-12-23 09:24:43.000000 Starco-3.3.2/starco/gateways/gates/nextpay.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1140 2023-12-23 09:24:28.000000 Starco-3.3.2/starco/gateways/gates/utils.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1826 2023-12-23 09:24:48.000000 Starco-3.3.2/starco/gateways/gates/vandar.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1182 2023-12-23 09:24:49.000000 Starco-3.3.2/starco/gateways/gates/zibalpay.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/gui/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     9174 2024-03-31 08:39:11.000000 Starco-3.3.2/starco/gui/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)    32861 2024-03-16 18:40:57.000000 Starco-3.3.2/starco/gui/utils.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/hetzner/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     7565 2024-06-01 22:29:04.000000 Starco-3.3.2/starco/hetzner/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.362605 Starco-3.3.2/starco/pkl/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     2208 2023-11-10 08:07:45.000000 Starco-3.3.2/starco/pkl/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/proxy/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     2248 2023-12-01 08:40:12.000000 Starco-3.3.2/starco/proxy/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/scraper/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1693 2024-05-03 15:02:33.000000 Starco-3.3.2/starco/scraper/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/tlg/
+-rw-rw-r--   0 starco    (1000) starco    (1000)       35 2024-01-09 13:06:48.000000 Starco-3.3.2/starco/tlg/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/tlg/app/
+-rw-rw-r--   0 starco    (1000) starco    (1000)    39525 2024-05-31 11:17:26.000000 Starco-3.3.2/starco/tlg/app/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      812 2024-01-09 13:06:48.000000 Starco-3.3.2/starco/tlg/app/utils.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/tlg/bot/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     7040 2024-06-01 22:26:31.000000 Starco-3.3.2/starco/tlg/bot/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)    47327 2024-01-09 14:36:18.000000 Starco-3.3.2/starco/tlg/bot/base.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     3146 2024-01-09 13:06:48.000000 Starco-3.3.2/starco/tlg/bot/classes.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/tlg/bot/util/
+-rw-rw-r--   0 starco    (1000) starco    (1000)        0 2024-01-09 13:06:48.000000 Starco-3.3.2/starco/tlg/bot/util/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      849 2024-01-11 11:40:27.000000 Starco-3.3.2/starco/tlg/bot/util/enum.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     4701 2024-01-09 13:06:48.000000 Starco-3.3.2/starco/tlg/bot/util/filteres.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     5494 2024-02-24 13:19:42.000000 Starco-3.3.2/starco/tlg/bot/util/functions.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)    35667 2024-02-24 13:21:45.000000 Starco-3.3.2/starco/tlg/bot/util/packs.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/utils/
+-rw-rw-r--   0 starco    (1000) starco    (1000)      125 2023-12-25 07:41:52.000000 Starco-3.3.2/starco/utils/__init__.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1122 2024-05-31 16:20:17.000000 Starco-3.3.2/starco/utils/directories.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1469 2024-02-24 13:20:03.000000 Starco-3.3.2/starco/utils/ext.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     1323 2023-12-06 19:14:01.000000 Starco-3.3.2/starco/utils/scheduler.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)      823 2024-03-24 07:26:00.000000 Starco-3.3.2/starco/utils/structures.py
+-rw-rw-r--   0 starco    (1000) starco    (1000)     2247 2024-01-01 09:30:33.000000 Starco-3.3.2/starco/utils/time.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/wp_api/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     4370 2023-12-15 13:34:21.000000 Starco-3.3.2/starco/wp_api/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/wscraper/
+-rw-rw-r--   0 starco    (1000) starco    (1000)     8229 2024-05-31 20:12:12.000000 Starco-3.3.2/starco/wscraper/__init__.py
+drwxrwxr-x   0 starco    (1000) starco    (1000)        0 2024-06-01 22:29:15.366605 Starco-3.3.2/starco/xray_connctor/
+-rw-rw-r--   0 starco    (1000) starco    (1000)    10800 2024-05-10 20:32:56.000000 Starco-3.3.2/starco/xray_connctor/__init__.py
```

### Comparing `Starco-3.3.1/PKG-INFO` & `Starco-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Starco
-Version: 3.3.1
+Version: 3.3.2
 Author: Mojtaba Tahmasbi
 Requires-Dist: cffi==1.15.1
 Requires-Dist: cryptography==41.0.3
 Requires-Dist: pycparser==2.21
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: lxml==4.9.3
 Requires-Dist: requests==2.31.0
```

### Comparing `Starco-3.3.1/Starco.egg-info/PKG-INFO` & `Starco-3.3.2/Starco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Starco
-Version: 3.3.1
+Version: 3.3.2
 Author: Mojtaba Tahmasbi
 Requires-Dist: cffi==1.15.1
 Requires-Dist: cryptography==41.0.3
 Requires-Dist: pycparser==2.21
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: lxml==4.9.3
 Requires-Dist: requests==2.31.0
```

### Comparing `Starco-3.3.1/Starco.egg-info/SOURCES.txt` & `Starco-3.3.2/Starco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/setup.py` & `Starco-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
     'selenium==4.17.2',
     'pyperclip==1.8.2',
     
 ]
 
 setup(
     name = 'Starco',long_description='starco project',
-    version='3.3.1',
+    version='3.3.2',
     author='Mojtaba Tahmasbi',
     packages=find_packages(),
     install_requires=requires,
 )
```

### Comparing `Starco-3.3.1/starco/cloudflare/__init__.py` & `Starco-3.3.2/starco/cloudflare/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/crypto_gates/nowpayments/__init__.py` & `Starco-3.3.2/starco/crypto_gates/nowpayments/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/db/__init__.py` & `Starco-3.3.2/starco/db/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/debug/__init__.py` & `Starco-3.3.2/starco/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/__init__.py` & `Starco-3.3.2/starco/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/gates/aqayepardakht.py` & `Starco-3.3.2/starco/gateways/gates/aqayepardakht.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/gates/idpay.py` & `Starco-3.3.2/starco/gateways/gates/idpay.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/gates/nextpay.py` & `Starco-3.3.2/starco/gateways/gates/nextpay.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/gates/utils.py` & `Starco-3.3.2/starco/gateways/gates/utils.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/gates/vandar.py` & `Starco-3.3.2/starco/gateways/gates/vandar.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gateways/gates/zibalpay.py` & `Starco-3.3.2/starco/gateways/gates/zibalpay.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gui/__init__.py` & `Starco-3.3.2/starco/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/gui/utils.py` & `Starco-3.3.2/starco/gui/utils.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/hetzner/__init__.py` & `Starco-3.3.2/starco/hetzner/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -97,32 +97,73 @@
             sleep(2)
         self.delete_primary_ips(primary_ipv6.id)
         sleep(5)
         self.power_on(server_id)
         return True
 
     def change_server_ip(self,server_id,ip_id):
-        self.power_off(server_id)
-        sleep(10)
-        server_info = self.client.servers.get_by_id(server_id)
+        print("turning off")
+        for _ in range(10):
+            server_info = self.client.servers.get_by_id(server_id)
+            if server_info.status!='off':
+                try:self.power_off(server_id)
+                except:pass
+            else:break
+            sleep(3)
+        else:raise Exception(f"/hsrv{server_id} cant be power off")
+
+        # unassign ip
+        print("unassign ip")
+
         old_ip = None
-        sleep(2)
-        primary_ipv4 = server_info.public_net.primary_ipv4
-        if type(primary_ipv4)!=type(None):
-            old_ip = server_info.public_net.ipv4.ip
-            self.client.primary_ips.unassign(primary_ipv4)
-            sleep(2)
-        if ip_id==0:
-            new_ip_name= f'ip{int(time())}'
-            primary_ip = self.client.primary_ips.create('ipv4',datacenter=server_info.datacenter,name=new_ip_name).primary_ip
-        else:primary_ip = self.get_primary_ips_by_id(ip_id)
-        sleep(5)
-        self.client.primary_ips.assign(primary_ip,server_id)
-        sleep(5)
-        self.power_on(server_id)
+        for _ in range(10):
+            server_info = self.client.servers.get_by_id(server_id)
+            primary_ipv4 = server_info.public_net.primary_ipv4
+            print(primary_ipv4)
+            if type(primary_ipv4)!=type(None):
+                try:
+                    old_ip = server_info.public_net.ipv4.ip
+                    self.client.primary_ips.unassign(primary_ipv4)
+                except:pass
+            else:break
+            sleep(3)
+        else:raise Exception(f"/hsrv{server_id} cant unassign ip")
+
+        # create ip
+        print("create ip")
+        try:
+            if ip_id==0:
+                new_ip_name= f'ip{int(time())}'
+                primary_ip = self.client.primary_ips.create('ipv4',datacenter=server_info.datacenter,name=new_ip_name).primary_ip
+            else:primary_ip = self.get_primary_ips_by_id(ip_id)
+        except Exception as e:
+            raise Exception(f"/hsrv{server_id} cant create ip")
+
+        print("assign new ip")
+        for _ in range(10):
+            server_info = self.client.servers.get_by_id(server_id)
+            primary_ipv4 = server_info.public_net.primary_ipv4
+            if type(primary_ipv4)==type(None):
+                try:
+                    self.client.primary_ips.assign(primary_ip,server_id)
+                except Exception as e:print(e)
+            else:break
+            sleep(3)
+        else:raise Exception(f"/hsrv{server_id} cant assign new ip")
+
+        print("turning on")
+        for _ in range(10):
+            server_info = self.client.servers.get_by_id(server_id)
+            if server_info.status!='running':
+                try:self.power_on(server_id)
+                except:pass
+            else:break
+            sleep(5)
+        else:raise Exception(f"/hsrv{server_id} cant turning on")
+
         return old_ip
     
     def assign_to_server(self,ip_id,server_id):
         self.power_off(server_id)
         sleep(10)
         server_info = self.client.servers.get_by_id(server_id)
         sleep(2)
```

### Comparing `Starco-3.3.1/starco/pkl/__init__.py` & `Starco-3.3.2/starco/pkl/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/proxy/__init__.py` & `Starco-3.3.2/starco/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/scraper/__init__.py` & `Starco-3.3.2/starco/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/app/__init__.py` & `Starco-3.3.2/starco/tlg/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/app/utils.py` & `Starco-3.3.2/starco/tlg/app/utils.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/bot/__init__.py` & `Starco-3.3.2/starco/tlg/bot/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,28 +42,33 @@
         self.db_relative_path = db_relative_path
         self.db_type = 'sqlite'
         self.debug_relative_path = debug_relative_path
         self.debug_mode = debug_mode
         self.debug = Debug(debug_mode=debug_mode,
                            relative_path=debug_relative_path)
         request_kwargs = None
+        self.db_config = db_config
+        self.db_tables_need_init = db_tables_need_init
+        self.init_db()
+        if self.token==None:
+            try:
+                self.token = self.db.do('setting',condition=f"key='bot_token'")[0]['value']
+            except:
+                raise Exception('bot token not set')
         if proxy:
             self.bot = Bot(self.token, request=Request(proxy_url=proxy))
             request_kwargs = {'proxy_url': proxy}
         else:
             self.bot = Bot(self.token)
         
         self.updater = Updater(self.token, use_context=True,
                                request_kwargs=request_kwargs)
         self.dp = self.updater.dispatcher
         self.bot_username = None
         
-        self.db_config = db_config
-        self.db_tables_need_init = db_tables_need_init
-        self.init_db()
         self.scheduler_status = scheduler_status
         self.scheduler = Scheduler(self)
 
     def init_db(self):
         self.forced_tables_init()
         self.db = DB(self.db_config, relative_path=self.db_relative_path,
                      debug_mode=self.debug_mode, debug_relative_path=self.debug_relative_path)
```

### Comparing `Starco-3.3.1/starco/tlg/bot/base.py` & `Starco-3.3.2/starco/tlg/bot/base.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/bot/classes.py` & `Starco-3.3.2/starco/tlg/bot/classes.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/bot/util/enum.py` & `Starco-3.3.2/starco/tlg/bot/util/enum.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/bot/util/filteres.py` & `Starco-3.3.2/starco/tlg/bot/util/filteres.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/bot/util/functions.py` & `Starco-3.3.2/starco/tlg/bot/util/functions.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/tlg/bot/util/packs.py` & `Starco-3.3.2/starco/tlg/bot/util/packs.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/utils/directories.py` & `Starco-3.3.2/starco/utils/directories.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/utils/ext.py` & `Starco-3.3.2/starco/utils/ext.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/utils/scheduler.py` & `Starco-3.3.2/starco/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/utils/structures.py` & `Starco-3.3.2/starco/utils/structures.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/utils/time.py` & `Starco-3.3.2/starco/utils/time.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/wp_api/__init__.py` & `Starco-3.3.2/starco/wp_api/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/wscraper/__init__.py` & `Starco-3.3.2/starco/wscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `Starco-3.3.1/starco/xray_connctor/__init__.py` & `Starco-3.3.2/starco/xray_connctor/__init__.py`

 * *Files identical despite different names*

