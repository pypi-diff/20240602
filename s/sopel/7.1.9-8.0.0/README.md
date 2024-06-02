# Comparing `tmp/sopel-7.1.9.tar.gz` & `tmp/sopel-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sopel-7.1.9.tar", last modified: Sun May  1 06:36:21 2022, max compression
+gzip compressed data, was "sopel-8.0.0.tar", last modified: Sun Jun  2 06:27:16 2024, max compression
```

## Comparing `sopel-7.1.9.tar` & `sopel-8.0.0.tar`

### file list

```diff
@@ -1,121 +1,102 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.012404 sopel-7.1.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1022 2022-05-01 06:34:49.000000 sopel-7.1.9/COPYING
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2022-05-01 06:34:49.000000 sopel-7.1.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     6111 2022-05-01 06:36:21.012404 sopel-7.1.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5008 2022-05-01 06:34:49.000000 sopel-7.1.9/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1462 2022-05-01 06:34:49.000000 sopel-7.1.9/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1240 2022-05-01 06:34:49.000000 sopel-7.1.9/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2022-05-01 06:36:21.012404 sopel-7.1.9/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2174 2022-05-01 06:34:49.000000 sopel-7.1.9/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:20.996402 sopel-7.1.9/sopel/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52838 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/bot.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:20.996402 sopel-7.1.9/sopel/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/cli/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6371 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/cli/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18513 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/cli/plugins.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    25134 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/cli/run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12646 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/cli/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:20.996402 sopel-7.1.9/sopel/config/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13832 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/config/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32115 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/config/core_section.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28104 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/config/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49896 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/coretasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33259 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8436 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/formatting.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.000403 sopel-7.1.9/sopel/irc/
--rw-rw-r--   0 travis    (2000) travis    (2000)    29905 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/irc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7542 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/irc/abstract_backends.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13044 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/irc/backends.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11229 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/irc/isupport.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3802 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/irc/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9742 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6169 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1417 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/module.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.004403 sopel-7.1.9/sopel/modules/
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15379 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10724 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/adminchannel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/announce.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2950 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/bugzilla.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/calc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3654 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/choose.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11588 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/clock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1585 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/countdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10271 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8247 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/dice.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2918 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/emoticons.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7461 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/find.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3074 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/find_updates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12412 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/help.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2790 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/invite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6911 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/ip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3477 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/isup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      941 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/lmgtfy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19155 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/meetbot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/ping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3925 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/pronouns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/py.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/rand.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16801 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/reddit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3671 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/reload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17983 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/remind.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10681 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/safety.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6588 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/seen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10590 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/tell.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13787 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/tld.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9070 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/translate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2324 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/unicode_info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6262 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/units.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      853 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/uptime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18006 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/url.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2247 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13380 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/wikipedia.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5192 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/wiktionary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4320 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/modules/xkcd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50884 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/plugin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.008403 sopel-7.1.9/sopel/plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8166 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      958 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/plugins/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/plugins/handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3347 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/plugins/jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57153 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/plugins/rules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5847 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/test_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.008403 sopel-7.1.9/sopel/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      636 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tests/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14755 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tests/mocks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8797 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tests/pytest_plugin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.008403 sopel-7.1.9/sopel/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    29976 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5765 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/_events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9847 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/calculation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15723 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12220 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/target.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11670 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/time.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8530 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/tools/web.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14979 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/trigger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5650 2022-05-01 06:34:49.000000 sopel-7.1.9/sopel/web.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:20.996402 sopel-7.1.9/sopel.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6111 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2412 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1910 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2022-05-01 06:36:20.000000 sopel-7.1.9/sopel.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-01 06:36:21.012404 sopel-7.1.9/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)    39007 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_bot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13300 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13342 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_coretasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10100 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3431 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_formatting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10759 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_irc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26556 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11210 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_module.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8979 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3922 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_plugins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1534 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_regression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7218 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11525 2022-05-01 06:34:49.000000 sopel-7.1.9/test/test_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.174786 sopel-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-02 06:27:11.000000 sopel-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-06-02 06:27:16.174786 sopel-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-06-02 06:27:11.000000 sopel-8.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-06-02 06:27:11.000000 sopel-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-02 06:27:16.174786 sopel-8.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.158786 sopel-8.0.0/sopel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55121 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.166786 sopel-8.0.0/sopel/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/adminchannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/announce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/choose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12934 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/countdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/find_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/isup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/lmgtfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/pronouns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/seen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10753 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/tell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13830 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/tld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/unicode_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/uptime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20766 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/wiktionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/builtins/xkcd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.170786 sopel-8.0.0/sopel/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/cli/plugins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15185 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.170786 sopel-8.0.0/sopel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37762 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/config/core_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28688 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57448 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/coretasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38346 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.170786 sopel-8.0.0/sopel/irc/
+-rw-r--r--   0 runner    (1001) docker     (127)    35074 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/abstract_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20201 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/isupport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12332 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/irc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72057 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.174786 sopel-8.0.0/sopel/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugins/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20711 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugins/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugins/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63830 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/plugins/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/privileges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.174786 sopel-8.0.0/sopel/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tests/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.174786 sopel-8.0.0/sopel/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/tools/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19312 2024-06-02 06:27:11.000000 sopel-8.0.0/sopel/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:27:16.162786 sopel-8.0.0/sopel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-06-02 06:27:16.000000 sopel-8.0.0/sopel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-06-02 06:27:16.000000 sopel-8.0.0/sopel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:27:16.000000 sopel-8.0.0/sopel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-02 06:27:16.000000 sopel-8.0.0/sopel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 06:27:16.000000 sopel-8.0.0/sopel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 06:27:16.000000 sopel-8.0.0/sopel.egg-info/top_level.txt
```

### Comparing `sopel-7.1.9/PKG-INFO` & `sopel-8.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: sopel
-Version: 7.1.9
+Version: 8.0.0
 Summary: Simple and extensible IRC bot
-Home-page: https://sopel.chat/
-Author: dgw
-Author-email: dgw@technobabbl.es
-License: Eiffel Forum License, version 2
-Platform: Linux x86
-Platform: x86-64
+Author: dgw, Florian Strzelecki, Sean B. Palmer, Else Powell, Elad Alfassa, Dimitri Molenaars, Michael Yanovich
+Maintainer: dgw, Florian Strzelecki
+License: EFL-2.0
+Project-URL: Homepage, https://sopel.chat/
+Project-URL: Release notes, https://sopel.chat/changelog/
+Project-URL: Documentation, https://sopel.chat/docs/
+Project-URL: Bug Tracker, https://github.com/sopel-irc/sopel/issues
+Project-URL: Donate on Open Collective, https://opencollective.com/sopel
+Project-URL: Donate on GitHub, https://github.com/sponsors/sopel-irc
+Project-URL: Source, https://github.com/sopel-irc/sopel
+Project-URL: Coverage, https://coveralls.io/github/sopel-irc/sopel
+Platform: Linux x86, x86-64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,<4,>=2.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: COPYING
 
 =======
  Sopel
 =======
 
-|version| |build| |issues| |alerts| |coverage-status| |license|
+|version| |build| |issues| |coverage-status| |license|
 
 Introduction
 ------------
 
 Sopel is a simple, lightweight, open source, easy-to-use IRC Utility bot,
 written in Python. It's designed to be easy to use, run and extend.
 
@@ -53,25 +55,18 @@
 Failing both of those options, you can grab the latest tarball `from GitHub
 <https://github.com/sopel-irc/sopel/releases/latest>`_  and follow the steps
 for installing from the latest source below.
 
 Latest source
 =============
 First, either clone the repository with ``git clone
-git://github.com/sopel-irc/sopel.git`` or download a tarball `from GitHub
-<https://github.com/sopel-irc/sopel/releases/latest>`_.
+https://github.com/sopel-irc/sopel.git`` or download a `source archive from
+GitHub <https://github.com/sopel-irc/sopel/archive/refs/heads/master.zip>`_.
 
-Note: Sopel requires Python 2.7.x or Python 3.3+ to run. On Python 2.7,
-Sopel requires ``backports.ssl_match_hostname`` to be installed. Use
-``pip install backports.ssl_match_hostname`` or
-``yum install python-backports.ssl_match_hostname`` to install it, or download
-and install it manually `from PyPI <https://pypi.org/project/backports.ssl_match_hostname>`_.
-
-Important: Sopel 8.0 will drop support for many old Python versions,
-including Python 2.7!
+Note: Sopel requires Python 3.8+ to run.
 
 In the source directory (whether cloned or from the tarball) run ``pip install
 -e .``. You can then run ``sopel`` to configure and start the bot.
 
 Database support
 ----------------
 Sopel leverages SQLAlchemy to support the following database types: SQLite,
@@ -125,19 +120,15 @@
 `Netlify <https://www.netlify.com/>`_, but we are considering building a few
 new features that would require more than static hosting. All project-related
 `expenses <https://opencollective.com/sopel/expenses>`_ are tracked on our
 Open Collective profile, for transparency.
 
 .. |version| image:: https://img.shields.io/pypi/v/sopel.svg
    :target: https://pypi.python.org/pypi/sopel
-.. |build| image:: https://travis-ci.org/sopel-irc/sopel.svg?branch=master
-   :target: https://travis-ci.org/sopel-irc/sopel
+.. |build| image:: https://github.com/sopel-irc/sopel/actions/workflows/ci.yml/badge.svg?branch=master&event=push
+   :target: https://github.com/sopel-irc/sopel/actions/workflows/ci.yml?query=branch%3Amaster+event%3Apush
 .. |issues| image:: https://img.shields.io/github/issues/sopel-irc/sopel.svg
    :target: https://github.com/sopel-irc/sopel/issues
-.. |alerts| image:: https://img.shields.io/lgtm/alerts/g/sopel-irc/sopel.svg
-   :target: https://lgtm.com/projects/g/sopel-irc/sopel/alerts/
 .. |coverage-status| image:: https://coveralls.io/repos/github/sopel-irc/sopel/badge.svg?branch=master
    :target: https://coveralls.io/github/sopel-irc/sopel?branch=master
 .. |license| image:: https://img.shields.io/pypi/l/sopel.svg
    :target: https://github.com/sopel-irc/sopel/blob/master/COPYING
-
-
```

### Comparing `sopel-7.1.9/README.rst` & `sopel-8.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =======
  Sopel
 =======
 
-|version| |build| |issues| |alerts| |coverage-status| |license|
+|version| |build| |issues| |coverage-status| |license|
 
 Introduction
 ------------
 
 Sopel is a simple, lightweight, open source, easy-to-use IRC Utility bot,
 written in Python. It's designed to be easy to use, run and extend.
 
@@ -24,25 +24,18 @@
 Failing both of those options, you can grab the latest tarball `from GitHub
 <https://github.com/sopel-irc/sopel/releases/latest>`_  and follow the steps
 for installing from the latest source below.
 
 Latest source
 =============
 First, either clone the repository with ``git clone
-git://github.com/sopel-irc/sopel.git`` or download a tarball `from GitHub
-<https://github.com/sopel-irc/sopel/releases/latest>`_.
+https://github.com/sopel-irc/sopel.git`` or download a `source archive from
+GitHub <https://github.com/sopel-irc/sopel/archive/refs/heads/master.zip>`_.
 
-Note: Sopel requires Python 2.7.x or Python 3.3+ to run. On Python 2.7,
-Sopel requires ``backports.ssl_match_hostname`` to be installed. Use
-``pip install backports.ssl_match_hostname`` or
-``yum install python-backports.ssl_match_hostname`` to install it, or download
-and install it manually `from PyPI <https://pypi.org/project/backports.ssl_match_hostname>`_.
-
-Important: Sopel 8.0 will drop support for many old Python versions,
-including Python 2.7!
+Note: Sopel requires Python 3.8+ to run.
 
 In the source directory (whether cloned or from the tarball) run ``pip install
 -e .``. You can then run ``sopel`` to configure and start the bot.
 
 Database support
 ----------------
 Sopel leverages SQLAlchemy to support the following database types: SQLite,
@@ -96,17 +89,15 @@
 `Netlify <https://www.netlify.com/>`_, but we are considering building a few
 new features that would require more than static hosting. All project-related
 `expenses <https://opencollective.com/sopel/expenses>`_ are tracked on our
 Open Collective profile, for transparency.
 
 .. |version| image:: https://img.shields.io/pypi/v/sopel.svg
    :target: https://pypi.python.org/pypi/sopel
-.. |build| image:: https://travis-ci.org/sopel-irc/sopel.svg?branch=master
-   :target: https://travis-ci.org/sopel-irc/sopel
+.. |build| image:: https://github.com/sopel-irc/sopel/actions/workflows/ci.yml/badge.svg?branch=master&event=push
+   :target: https://github.com/sopel-irc/sopel/actions/workflows/ci.yml?query=branch%3Amaster+event%3Apush
 .. |issues| image:: https://img.shields.io/github/issues/sopel-irc/sopel.svg
    :target: https://github.com/sopel-irc/sopel/issues
-.. |alerts| image:: https://img.shields.io/lgtm/alerts/g/sopel-irc/sopel.svg
-   :target: https://lgtm.com/projects/g/sopel-irc/sopel/alerts/
 .. |coverage-status| image:: https://coveralls.io/repos/github/sopel-irc/sopel/badge.svg?branch=master
    :target: https://coveralls.io/github/sopel-irc/sopel?branch=master
 .. |license| image:: https://img.shields.io/pypi/l/sopel.svg
    :target: https://github.com/sopel-irc/sopel/blob/master/COPYING
```

### Comparing `sopel-7.1.9/sopel/bot.py` & `sopel-8.0.0/sopel/bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,166 +1,155 @@
-# coding=utf-8
 # Copyright 2008, Sean B. Palmer, inamidst.com
 # Copyright © 2012, Elad Alfassa <elad@fedoraproject.org>
 # Copyright 2012-2015, Elsie Powell, http://embolalia.com
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 from ast import literal_eval
-from datetime import datetime
 import inspect
 import itertools
 import logging
 import re
-import signal
-import sys
 import threading
 import time
-
-from sopel import irc, logger, plugins, tools
-from sopel.db import SopelDB
-import sopel.loader
-from sopel.module import NOLIMIT
-from sopel.plugins import jobs as plugin_jobs, rules as plugin_rules
-from sopel.tools import deprecated, Identifier
-import sopel.tools.jobs
+from types import MappingProxyType
+from typing import (
+    Any,
+    Optional,
+    TYPE_CHECKING,
+    TypeVar,
+    Union,
+)
+
+from sopel import db, irc, logger, plugin, plugins, tools
+from sopel.irc import modes
+from sopel.lifecycle import deprecated
+from sopel.plugins import (
+    capabilities as plugin_capabilities,
+    jobs as plugin_jobs,
+    rules as plugin_rules,
+)
+from sopel.tools import jobs as tools_jobs
 from sopel.trigger import Trigger
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable, Mapping
+    from sopel.trigger import PreTrigger
+
 
 __all__ = ['Sopel', 'SopelWrapper']
 
 LOGGER = logging.getLogger(__name__)
-QUIT_SIGNALS = [
-    getattr(signal, name)
-    for name in ['SIGUSR1', 'SIGTERM', 'SIGINT']
-    if hasattr(signal, name)
-]
-RESTART_SIGNALS = [
-    getattr(signal, name)
-    for name in ['SIGUSR2', 'SIGILL']
-    if hasattr(signal, name)
-]
-SIGNALS = QUIT_SIGNALS + RESTART_SIGNALS
-
-
-if sys.version_info.major >= 3:
-    unicode = str
-    basestring = str
-    py3 = True
-else:
-    py3 = False
+
+AbstractRuleType = TypeVar('AbstractRuleType', bound=plugin_rules.AbstractRule)
 
 
 class Sopel(irc.AbstractBot):
     def __init__(self, config, daemon=False):
-        super(Sopel, self).__init__(config)
+        super().__init__(config)
         self._daemon = daemon  # Used for iPython. TODO something saner here
-        self.wantsrestart = False
         self._running_triggers = []
         self._running_triggers_lock = threading.Lock()
-        self._plugins = {}
+        self._plugins: dict[str, Any] = {}
         self._rules_manager = plugin_rules.Manager()
+        self._cap_requests_manager = plugin_capabilities.Manager()
         self._scheduler = plugin_jobs.Scheduler(self)
 
+        self._url_callbacks = tools.SopelMemory()
+        """Tracking of manually registered URL callbacks.
+
+        Should be manipulated only by use of :meth:`register_url_callback` and
+        :meth:`unregister_url_callback` methods, which are deprecated.
+
+        Remove in Sopel 9, along with the above related methods.
+        """
+
         self._times = {}
         """
         A dictionary mapping lowercased nicks to dictionaries which map
         function names to the time which they were last used by that nick.
         """
 
-        self.server_capabilities = {}
-        """A dict mapping supported IRCv3 capabilities to their options.
+        self.modeparser = modes.ModeParser()
+        """A mode parser used to parse ``MODE`` messages and modestrings."""
 
-        For example, if the server specifies the capability ``sasl=EXTERNAL``,
-        it will be here as ``{"sasl": "EXTERNAL"}``. Capabilities specified
-        without any options will have ``None`` as the value.
-
-        For servers that do not support IRCv3, this will be an empty set.
-        """
-
-        self.privileges = dict()
-        """A dictionary of channels to their users and privilege levels.
-
-        The value associated with each channel is a dictionary of
-        :class:`sopel.tools.Identifier`\\s to a bitwise integer value,
-        determined by combining the appropriate constants from
-        :mod:`sopel.plugin`.
-
-        .. deprecated:: 6.2.0
-            Use :attr:`channels` instead. Will be removed in Sopel 8.
-        """
-
-        self.channels = tools.SopelIdentifierMemory()
+        self.channels = self.make_identifier_memory()
         """A map of the channels that Sopel is in.
 
-        The keys are :class:`sopel.tools.Identifier`\\s of the channel names,
-        and map to :class:`sopel.tools.target.Channel` objects which contain
-        the users in the channel and their permissions.
+        The keys are :class:`~sopel.tools.identifiers.Identifier`\\s of the
+        channel names, and map to :class:`~sopel.tools.target.Channel` objects
+        which contain the users in the channel and their permissions.
         """
 
-        self.users = tools.SopelIdentifierMemory()
+        self.users = self.make_identifier_memory()
         """A map of the users that Sopel is aware of.
 
-        The keys are :class:`sopel.tools.Identifier`\\s of the nicknames, and
-        map to :class:`sopel.tools.target.User` instances. In order for Sopel
-        to be aware of a user, it must share at least one mutual channel.
+        The keys are :class:`~sopel.tools.identifiers.Identifier`\\s of the
+        nicknames, and map to :class:`~sopel.tools.target.User` instances. In
+        order for Sopel to be aware of a user, it must share at least one
+        mutual channel.
         """
 
-        self.db = SopelDB(config)
+        self.db = db.SopelDB(config, identifier_factory=self.make_identifier)
         """The bot's database, as a :class:`sopel.db.SopelDB` instance."""
 
         self.memory = tools.SopelMemory()
         """
         A thread-safe dict for storage of runtime data to be shared between
-        plugins. See :class:`sopel.tools.SopelMemory`.
+        plugins. See :class:`sopel.tools.memories.SopelMemory`.
         """
 
         self.shutdown_methods = []
         """List of methods to call on shutdown."""
 
     @property
-    def rules(self):
+    def cap_requests(self) -> plugin_capabilities.Manager:
+        """Capability Requests manager."""
+        return self._cap_requests_manager
+
+    @property
+    def rules(self) -> plugin_rules.Manager:
         """Rules manager."""
         return self._rules_manager
 
     @property
-    def scheduler(self):
+    def scheduler(self) -> plugin_jobs.Scheduler:
         """Job Scheduler. See :func:`sopel.plugin.interval`."""
         return self._scheduler
 
     @property
-    def command_groups(self):
+    def command_groups(self) -> dict[str, list]:
         """A mapping of plugin names to lists of their commands.
 
         .. versionchanged:: 7.1
             This attribute is now generated on the fly from the registered list
             of commands and nickname commands.
         """
         # This was supposed to be deprecated, but the built-in help plugin needs it
         # TODO: create a new, better, doc interface to remove it
         plugin_commands = itertools.chain(
             self._rules_manager.get_all_commands(),
             self._rules_manager.get_all_nick_commands(),
         )
         result = {}
 
-        for plugin, commands in plugin_commands:
-            if plugin not in result:
-                result[plugin] = list(sorted(commands.keys()))
+        for plugin_name, commands in plugin_commands:
+            if plugin_name not in result:
+                result[plugin_name] = list(sorted(commands.keys()))
             else:
-                result[plugin].extend(commands.keys())
-                result[plugin] = list(sorted(result[plugin]))
+                result[plugin_name].extend(commands.keys())
+                result[plugin_name] = list(sorted(result[plugin_name]))
 
         return result
 
     @property
-    def doc(self):
+    def doc(self) -> dict[str, tuple]:
         """A dictionary of command names to their documentation.
 
         Each command is mapped to its docstring and any available examples, if
         declared in the plugin's code.
 
         .. versionchanged:: 3.2
             Use the first item in each callable's commands list as the key,
@@ -173,127 +162,94 @@
         # TODO: create a new, better, doc interface to remove it
         plugin_commands = itertools.chain(
             self._rules_manager.get_all_commands(),
             self._rules_manager.get_all_nick_commands(),
         )
         commands = (
             (command, command.get_doc(), command.get_usages())
-            for plugin, commands in plugin_commands
+            for plugin_name, commands in plugin_commands
             for command in commands.values()
         )
 
         return dict(
             (name, (doc.splitlines(), [u['text'] for u in usages]))
             for command, doc, usages in commands
             for name in ((command.name,) + command.aliases)
         )
 
     @property
-    def hostmask(self):
-        """The current hostmask for the bot :class:`sopel.tools.target.User`.
-
-        :return: the bot's current hostmask
-        :rtype: str
+    def hostmask(self) -> Optional[str]:
+        """The current hostmask for the bot :class:`~sopel.tools.target.User`.
 
-        Bot must be connected and in at least one channel.
+        :return: the bot's current hostmask if the bot is connected and in
+                 a least one channel; ``None`` otherwise
+        :rtype: Optional[str]
         """
         if not self.users or self.nick not in self.users:
-            raise KeyError("'hostmask' not available: bot must be connected and in at least one channel.")
+            # bot must be connected and in at least one channel
+            return None
 
-        return self.users.get(self.nick).hostmask
+        return self.users[self.nick].hostmask
 
-    def has_channel_privilege(self, channel, privilege):
+    @property
+    def plugins(self) -> Mapping[str, plugins.handlers.AbstractPluginHandler]:
+        """A dict of the bot's currently loaded plugins.
+
+        :return: an immutable map of plugin name to plugin object
+        """
+        return MappingProxyType(self._plugins)
+
+    def has_channel_privilege(self, channel, privilege) -> bool:
         """Tell if the bot has a ``privilege`` level or above in a ``channel``.
 
         :param str channel: a channel the bot is in
         :param int privilege: privilege level to check
         :raise ValueError: when the channel is unknown
 
         This method checks the bot's privilege level in a channel, i.e. if it
         has this level or higher privileges::
 
             >>> bot.channels['#chan'].privileges[bot.nick] = plugin.OP
             >>> bot.has_channel_privilege('#chan', plugin.VOICE)
             True
 
-        The ``channel`` argument can be either a :class:`str` or a
-        :class:`sopel.tools.Identifier`, as long as Sopel joined said channel.
-        If the channel is unknown, a :exc:`ValueError` will be raised.
+        The ``channel`` argument can be either a :class:`str` or an
+        :class:`~sopel.tools.identifiers.Identifier`, as long as Sopel joined
+        said channel. If the channel is unknown, a :exc:`ValueError` will be
+        raised.
         """
         if channel not in self.channels:
             raise ValueError('Unknown channel %s' % channel)
 
         return self.channels[channel].has_privilege(self.nick, privilege)
 
-    # signal handlers
-
-    def set_signal_handlers(self):
-        """Set signal handlers for the bot.
-
-        Before running the bot, this method can be called from the main thread
-        to setup signals. If the bot is connected, upon receiving a signal it
-        will send a ``QUIT`` message. Otherwise, it raises a
-        :exc:`KeyboardInterrupt` error.
-
-        .. note::
-
-            Per the Python documentation of :func:`signal.signal`:
-
-                When threads are enabled, this function can only be called from
-                the main thread; attempting to call it from other threads will
-                cause a :exc:`ValueError` exception to be raised.
-
-        """
-        for obj in SIGNALS:
-            signal.signal(obj, self._signal_handler)
-
-    def _signal_handler(self, sig, frame):
-        if sig in QUIT_SIGNALS:
-            if self.backend.is_connected():
-                LOGGER.warning("Got quit signal, sending QUIT to server.")
-                self.quit('Closing')
-            else:
-                self.hasquit = True  # mark the bot as "want to quit"
-                LOGGER.warning("Got quit signal.")
-                raise KeyboardInterrupt
-        elif sig in RESTART_SIGNALS:
-            if self.backend.is_connected():
-                LOGGER.warning("Got restart signal, sending QUIT to server.")
-                self.restart('Restarting')
-            else:
-                LOGGER.warning("Got restart signal.")
-                self.wantsrestart = True  # mark the bot as "want to restart"
-                self.hasquit = True  # mark the bot as "want to quit"
-                raise KeyboardInterrupt
-
     # setup
 
-    def setup(self):
+    def setup(self) -> None:
         """Set up Sopel bot before it can run.
 
         The setup phase is in charge of:
 
         * setting up logging (configure Python's built-in :mod:`logging`)
         * setting up the bot's plugins (load, setup, and register)
         * starting the job scheduler
         """
         self.setup_logging()
         self.setup_plugins()
         self.post_setup()
 
-    def setup_logging(self):
+    def setup_logging(self) -> None:
         """Set up logging based on config options."""
         logger.setup_logging(self.settings)
-        base_level = self.settings.core.logging_level or 'INFO'
         base_format = self.settings.core.logging_format
         base_datefmt = self.settings.core.logging_datefmt
 
         # configure channel logging if required by configuration
         if self.settings.core.logging_channel:
-            channel_level = self.settings.core.logging_channel_level or base_level
+            channel_level = self.settings.core.logging_channel_level
             channel_format = self.settings.core.logging_channel_format or base_format
             channel_datefmt = self.settings.core.logging_channel_datefmt or base_datefmt
             channel_params = {}
             if channel_format:
                 channel_params['fmt'] = channel_format
             if channel_datefmt:
                 channel_params['datefmt'] = channel_datefmt
@@ -301,44 +257,42 @@
             handler = logger.IrcLoggingHandler(self, channel_level)
             handler.setFormatter(formatter)
 
             # set channel handler to `sopel` logger
             LOGGER = logging.getLogger('sopel')
             LOGGER.addHandler(handler)
 
-    def setup_plugins(self):
+    def setup_plugins(self) -> None:
         """Load plugins into the bot."""
         load_success = 0
         load_error = 0
         load_disabled = 0
 
         LOGGER.info("Loading plugins...")
         usable_plugins = plugins.get_usable_plugins(self.settings)
         for name, info in usable_plugins.items():
-            plugin, is_enabled = info
+            plugin_handler, is_enabled = info
             if not is_enabled:
                 load_disabled = load_disabled + 1
                 continue
 
             try:
-                plugin.load()
+                plugin_handler.load()
             except Exception as e:
                 load_error = load_error + 1
                 LOGGER.exception("Error loading %s: %s", name, e)
             except SystemExit:
                 load_error = load_error + 1
                 LOGGER.exception(
                     "Error loading %s (plugin tried to exit)", name)
             else:
                 try:
-                    if plugin.has_setup():
-                        plugin.setup(self)
-                        # TODO: remove in Sopel 8
-                        self.__setup_plugins_check_manual_url_callbacks(name)
-                    plugin.register(self)
+                    if plugin_handler.has_setup():
+                        plugin_handler.setup(self)
+                    plugin_handler.register(self)
                 except Exception as e:
                     load_error = load_error + 1
                     LOGGER.exception("Error in %s setup: %s", name, e)
                 else:
                     load_success = load_success + 1
                     LOGGER.info("Plugin loaded: %s", name)
 
@@ -348,40 +302,17 @@
                 "Registered %d plugins, %d failed, %d disabled",
                 (load_success - 1),
                 load_error,
                 load_disabled)
         else:
             LOGGER.warning("Warning: Couldn't load any plugins")
 
-    def __setup_plugins_check_manual_url_callbacks(self, name):
-        # check if a plugin modified bot.memory['url_callbacks'] manually
-        # TODO: remove in Sopel 8
-        if 'url_callbacks' not in self.memory:
-            # nothing to check
-            return
-
-        for key, callback in tools.iteritems(self.memory['url_callbacks']):
-            is_checked = getattr(
-                callback, '_sopel_url_callbacks_checked', False)
-            if is_checked:
-                # already checked; move on to next callback
-                continue
-
-            # deprecation warning
-            LOGGER.warning(
-                "Plugin `%s` uses `bot.memory['url_callbacks']`; "
-                'this key is deprecated and will be removed in Sopel 8. '
-                'Use `@url` or `@url_lazy` instead. Callback was: %s',
-                name, callback.__name__)
-            # mark callback as checked
-            setattr(callback, '_sopel_url_callbacks_checked', True)
-
     # post setup
 
-    def post_setup(self):
+    def post_setup(self) -> None:
         """Perform post-setup actions.
 
         This method handles everything that should happen after all the plugins
         are loaded, and before the bot can connect to the IRC server.
 
         At the moment, this method checks for undefined configuration options,
         and starts the job scheduler.
@@ -404,65 +335,67 @@
                         option_name,
                     )
 
         self._scheduler.start()
 
     # plugins management
 
-    def reload_plugin(self, name):
+    def reload_plugin(self, name) -> None:
         """Reload a plugin.
 
         :param str name: name of the plugin to reload
         :raise plugins.exceptions.PluginNotRegistered: when there is no
             ``name`` plugin registered
 
         This function runs the plugin's shutdown routine and unregisters the
         plugin from the bot. Then this function reloads the plugin, runs its
         setup routines, and registers it again.
         """
         if not self.has_plugin(name):
             raise plugins.exceptions.PluginNotRegistered(name)
 
-        plugin = self._plugins[name]
+        plugin_handler = self._plugins[name]
         # tear down
-        plugin.shutdown(self)
-        plugin.unregister(self)
+        plugin_handler.shutdown(self)
+        plugin_handler.unregister(self)
         LOGGER.info("Unloaded plugin %s", name)
         # reload & setup
-        plugin.reload()
-        plugin.setup(self)
-        plugin.register(self)
-        meta = plugin.get_meta_description()
+        plugin_handler.reload()
+        plugin_handler.setup(self)
+        plugin_handler.register(self)
+        meta = plugin_handler.get_meta_description()
         LOGGER.info("Reloaded %s plugin %s from %s",
                     meta['type'], name, meta['source'])
 
-    def reload_plugins(self):
+    def reload_plugins(self) -> None:
         """Reload all registered plugins.
 
         First, this function runs all plugin shutdown routines and unregisters
         all plugins. Then it reloads all plugins, runs their setup routines, and
         registers them again.
         """
         registered = list(self._plugins.items())
         # tear down all plugins
-        for name, plugin in registered:
-            plugin.shutdown(self)
-            plugin.unregister(self)
+        for name, handler in registered:
+            handler.shutdown(self)
+            handler.unregister(self)
             LOGGER.info("Unloaded plugin %s", name)
 
         # reload & setup all plugins
-        for name, plugin in registered:
-            plugin.reload()
-            plugin.setup(self)
-            plugin.register(self)
-            meta = plugin.get_meta_description()
+        for name, handler in registered:
+            handler.reload()
+            handler.setup(self)
+            handler.register(self)
+            meta = handler.get_meta_description()
             LOGGER.info("Reloaded %s plugin %s from %s",
                         meta['type'], name, meta['source'])
 
-    def add_plugin(self, plugin, callables, jobs, shutdowns, urls):
+    # TODO: deprecate both add_plugin and remove_plugin; see #2425
+
+    def add_plugin(self, plugin, callables, jobs, shutdowns, urls) -> None:
         """Add a loaded plugin to the bot's registry.
 
         :param plugin: loaded plugin to add
         :type plugin: :class:`sopel.plugins.handlers.AbstractPluginHandler`
         :param callables: an iterable of callables from the ``plugin``
         :type callables: :term:`iterable`
         :param jobs: an iterable of functions from the ``plugin`` that are
@@ -477,15 +410,15 @@
         """
         self._plugins[plugin.name] = plugin
         self.register_callables(callables)
         self.register_jobs(jobs)
         self.register_shutdowns(shutdowns)
         self.register_urls(urls)
 
-    def remove_plugin(self, plugin, callables, jobs, shutdowns, urls):
+    def remove_plugin(self, plugin, callables, jobs, shutdowns, urls) -> None:
         """Remove a loaded plugin from the bot's registry.
 
         :param plugin: loaded plugin to remove
         :type plugin: :class:`sopel.plugins.handlers.AbstractPluginHandler`
         :param callables: an iterable of callables from the ``plugin``
         :type callables: :term:`iterable`
         :param jobs: an iterable of functions from the ``plugin`` that are
@@ -506,24 +439,24 @@
         self._rules_manager.unregister_plugin(name)
         self._scheduler.unregister_plugin(name)
         self.unregister_shutdowns(shutdowns)
 
         # remove plugin from registry
         del self._plugins[name]
 
-    def has_plugin(self, name):
+    def has_plugin(self, name: str) -> bool:
         """Check if the bot has registered a plugin of the specified name.
 
         :param str name: name of the plugin to check for
         :return: whether the bot has a plugin named ``name`` registered
         :rtype: bool
         """
         return name in self._plugins
 
-    def get_plugin_meta(self, name):
+    def get_plugin_meta(self, name: str) -> dict:
         """Get info about a registered plugin by its name.
 
         :param str name: name of the plugin about which to get info
         :return: the plugin's metadata
                  (see :meth:`~.plugins.handlers.AbstractPluginHandler.get_meta_description`)
         :rtype: :class:`dict`
         :raise plugins.exceptions.PluginNotRegistered: when there is no
@@ -532,71 +465,15 @@
         if not self.has_plugin(name):
             raise plugins.exceptions.PluginNotRegistered(name)
 
         return self._plugins[name].get_meta_description()
 
     # callable management
 
-    @deprecated(
-        reason="Replaced by specific `unregister_*` methods.",
-        version='7.1',
-        removed_in='8.0')
-    def unregister(self, obj):
-        """Unregister a shutdown method.
-
-        :param obj: the shutdown method to unregister
-        :type obj: :term:`object`
-
-        This method was used to unregister anything (rules, commands, urls,
-        jobs, and shutdown methods), but since everything can be done by other
-        means, there is no use for it anymore.
-        """
-        callable_name = getattr(obj, "__name__", 'UNKNOWN')
-
-        if hasattr(obj, 'interval'):
-            self.unregister_jobs([obj])
-
-        if callable_name == "shutdown" and obj in self.shutdown_methods:
-            self.unregister_shutdowns([obj])
-
-    @deprecated(
-        reason="Replaced by specific `register_*` methods.",
-        version='7.1',
-        removed_in='8.0')
-    def register(self, callables, jobs, shutdowns, urls):
-        """Register rules, jobs, shutdown methods, and URL callbacks.
-
-        :param callables: an iterable of callables to register
-        :type callables: :term:`iterable`
-        :param jobs: an iterable of functions to periodically invoke
-        :type jobs: :term:`iterable`
-        :param shutdowns: an iterable of functions to call on shutdown
-        :type shutdowns: :term:`iterable`
-        :param urls: an iterable of functions to call when matched against a URL
-        :type urls: :term:`iterable`
-
-        The ``callables`` argument contains a list of "callable objects", i.e.
-        objects for which :func:`callable` will return ``True``. They can be:
-
-        * a callable with rules (will match triggers with a regex pattern)
-        * a callable without rules (will match any triggers, such as events)
-        * a callable with commands
-        * a callable with nick commands
-        * a callable with action commands
-
-        It is possible to have a callable with rules, commands, and nick
-        commands configured. It should not be possible to have a callable with
-        commands or nick commands but without rules.
-        """
-        self.register_callables(callables)
-        self.register_jobs(jobs)
-        self.register_shutdowns(shutdowns)
-        self.register_urls(urls)
-
-    def register_callables(self, callables):
+    def register_callables(self, callables: Iterable) -> None:
         match_any = re.compile(r'.*')
         settings = self.settings
 
         for callbl in callables:
             rules = getattr(callbl, 'rule', [])
             lazy_rules = getattr(callbl, 'rule_lazy_loaders', [])
             find_rules = getattr(callbl, 'find_rules', [])
@@ -667,36 +544,36 @@
                 self._rules_manager.register_action_command(rule)
 
             if not is_command and not is_rule:
                 callbl.rule = [match_any]
                 self._rules_manager.register(
                     plugin_rules.Rule.from_callable(self.settings, callbl))
 
-    def register_jobs(self, jobs):
+    def register_jobs(self, jobs: Iterable) -> None:
         for func in jobs:
-            job = sopel.tools.jobs.Job.from_callable(self.settings, func)
+            job = tools_jobs.Job.from_callable(self.settings, func)
             self._scheduler.register(job)
 
-    def unregister_jobs(self, jobs):
+    def unregister_jobs(self, jobs: Iterable) -> None:
         for job in jobs:
             self._scheduler.remove_callable_job(job)
 
-    def register_shutdowns(self, shutdowns):
+    def register_shutdowns(self, shutdowns: Iterable) -> None:
         # Append plugin's shutdown function to the bot's list of functions to
         # call on shutdown
         self.shutdown_methods = self.shutdown_methods + list(shutdowns)
 
-    def unregister_shutdowns(self, shutdowns):
+    def unregister_shutdowns(self, shutdowns: Iterable) -> None:
         self.shutdown_methods = [
             shutdown
             for shutdown in self.shutdown_methods
             if shutdown not in shutdowns
         ]
 
-    def register_urls(self, urls):
+    def register_urls(self, urls: Iterable) -> None:
         for func in urls:
             url_regex = getattr(func, 'url_regex', [])
             url_lazy_loaders = getattr(func, 'url_lazy_loaders', None)
 
             if url_regex:
                 rule = plugin_rules.URLCallback.from_callable(
                     self.settings, func)
@@ -706,71 +583,131 @@
                 try:
                     rule = plugin_rules.URLCallback.from_callable_lazy(
                         self.settings, func)
                     self._rules_manager.register_url_callback(rule)
                 except plugins.exceptions.PluginError as err:
                     LOGGER.error("Cannot register URL callback: %s", err)
 
-    @deprecated(
-        reason="Replaced by `say` method.",
-        version='6.0',
-        removed_in='8.0')
-    def msg(self, recipient, text, max_messages=1):
-        """Old way to make the bot say something on IRC.
-
-        :param str recipient: nickname or channel to which to send message
-        :param str text: message to send
-        :param int max_messages: split ``text`` into at most this many messages
-                                 if it is too long to fit in one (optional)
+    def rate_limit_info(
+        self,
+        rule: AbstractRuleType,
+        trigger: Trigger,
+    ) -> tuple[bool, Optional[str]]:
+        if trigger.admin or rule.is_unblockable():
+            return False, None
+
+        is_channel = trigger.sender and not trigger.sender.is_nick()
+        channel = trigger.sender if is_channel else None
+
+        at_time = trigger.time
+
+        user_metrics = rule.get_user_metrics(trigger.nick)
+        channel_metrics = rule.get_channel_metrics(channel)
+        global_metrics = rule.get_global_metrics()
+
+        if user_metrics.is_limited(at_time - rule.user_rate_limit):
+            template = rule.user_rate_template
+            rate_limit_type = "user"
+            rate_limit = rule.user_rate_limit
+            metrics = user_metrics
+        elif is_channel and channel_metrics.is_limited(at_time - rule.channel_rate_limit):
+            template = rule.channel_rate_template
+            rate_limit_type = "channel"
+            rate_limit = rule.channel_rate_limit
+            metrics = channel_metrics
+        elif global_metrics.is_limited(at_time - rule.global_rate_limit):
+            template = rule.global_rate_template
+            rate_limit_type = "global"
+            rate_limit = rule.global_rate_limit
+            metrics = global_metrics
+        else:
+            return False, None
 
-        .. deprecated:: 6.0
-            Use :meth:`say` instead. Will be removed in Sopel 8.
-        """
-        self.say(text, recipient, max_messages)
+        if not metrics.last_time:
+            # you and I know that is_limited() will never return True if
+            # last_time is None, but the type-checker doesn't
+            return False, None
+
+        next_time = metrics.last_time + rate_limit
+        time_left = next_time - at_time
+
+        message: Optional[str] = None
+
+        if template:
+            message = template.format(
+                nick=trigger.nick,
+                channel=channel or 'private message',
+                sender=trigger.sender,
+                plugin=rule.get_plugin_name(),
+                label=rule.get_rule_label(),
+                time_left=time_left,
+                time_left_sec=time_left.total_seconds(),
+                rate_limit=rate_limit,
+                rate_limit_sec=rate_limit.total_seconds(),
+                rate_limit_type=rate_limit_type,
+            )
+
+        return True, message
 
     # message dispatch
 
-    def call_rule(self, rule, sopel, trigger):
-        # rate limiting
-        if not trigger.admin and not rule.is_unblockable():
-            if rule.is_rate_limited(trigger.nick):
-                return
-            if not trigger.is_privmsg and rule.is_channel_rate_limited(trigger.sender):
-                return
-            if rule.is_global_rate_limited():
-                return
+    def call_rule(
+        self,
+        rule: plugin_rules.AbstractRule,
+        sopel: 'SopelWrapper',
+        trigger: Trigger,
+    ) -> None:
+        nick = trigger.nick
+        context = trigger.sender
+        is_channel = context and not context.is_nick()
+
+        limited, limit_msg = self.rate_limit_info(rule, trigger)
+        if limit_msg:
+            sopel.notice(limit_msg, destination=nick)
+        if limited:
+            return
 
         # channel config
-        if trigger.sender in self.config:
-            channel_config = self.config[trigger.sender]
+        if is_channel and context in self.config:
+            channel_config = self.config[context]
+            plugin_name = rule.get_plugin_name()
 
             # disable listed plugins completely on provided channel
             if 'disable_plugins' in channel_config:
                 disabled_plugins = channel_config.disable_plugins.split(',')
 
-                if '*' in disabled_plugins:
+                if plugin_name == 'coretasks':
+                    LOGGER.debug("disable_plugins refuses to skip a coretasks handler")
+                elif '*' in disabled_plugins:
                     return
-                elif rule.get_plugin_name() in disabled_plugins:
+                elif plugin_name in disabled_plugins:
                     return
 
             # disable chosen methods from plugins
             if 'disable_commands' in channel_config:
                 disabled_commands = literal_eval(channel_config.disable_commands)
-                disabled_commands = disabled_commands.get(rule.get_plugin_name(), [])
+                disabled_commands = disabled_commands.get(plugin_name, [])
                 if rule.get_rule_label() in disabled_commands:
-                    return
+                    if plugin_name != 'coretasks':
+                        return
+                    LOGGER.debug("disable_commands refuses to skip a coretasks handler")
 
         try:
             rule.execute(sopel, trigger)
         except KeyboardInterrupt:
             raise
         except Exception as error:
             self.error(trigger, exception=error)
 
-    def call(self, func, sopel, trigger):
+    def call(
+        self,
+        func: Any,
+        sopel: 'SopelWrapper',
+        trigger: Trigger,
+    ) -> None:
         """Call a function, applying any rate limits or other restrictions.
 
         :param func: the function to call
         :type func: :term:`function`
         :param sopel: a SopelWrapper instance
         :type sopel: :class:`SopelWrapper`
         :param Trigger trigger: the Trigger object for the line from the server
@@ -784,19 +721,19 @@
             self._times[self.nick] = dict()
         if not trigger.is_privmsg and trigger.sender not in self._times:
             self._times[trigger.sender] = dict()
 
         if not trigger.admin and not func.unblockable:
             if func in self._times[nick]:
                 usertimediff = current_time - self._times[nick][func]
-                if func.rate > 0 and usertimediff < func.rate:
+                if func.user_rate > 0 and usertimediff < func.user_rate:
                     LOGGER.info(
                         "%s prevented from using %s in %s due to user limit: %d < %d",
                         trigger.nick, func.__name__, trigger.sender, usertimediff,
-                        func.rate
+                        func.user_rate
                     )
                     return
             if func in self._times[self.nick]:
                 globaltimediff = current_time - self._times[self.nick][func]
                 if func.global_rate > 0 and globaltimediff < func.global_rate:
                     LOGGER.info(
                         "%s prevented from using %s in %s due to global limit: %d < %d",
@@ -811,16 +748,18 @@
                     LOGGER.info(
                         "%s prevented from using %s in %s due to channel limit: %d < %d",
                         trigger.nick, func.__name__, trigger.sender, chantimediff,
                         func.channel_rate
                     )
                     return
 
-        # if channel has its own config section, check for excluded plugins/plugin methods
-        if trigger.sender in self.config:
+        # if channel has its own config section, check for excluded plugins/plugin methods,
+        # but only if the source plugin is NOT coretasks, because we NEED those handlers.
+        # Normal, whole-bot configuration will not let you disable coretasks either.
+        if trigger.sender in self.config and func.plugin_name != 'coretasks':
             channel_config = self.config[trigger.sender]
             LOGGER.debug(
                 "Evaluating configuration for %s.%s in channel %s",
                 func.plugin_name, func.__name__, trigger.sender
             )
 
             # disable listed plugins completely on provided channel
@@ -855,30 +794,35 @@
 
         try:
             exit_code = func(sopel, trigger)
         except Exception as error:  # TODO: Be specific
             exit_code = None
             self.error(trigger, exception=error)
 
-        if exit_code != NOLIMIT:
+        if exit_code != plugin.NOLIMIT:
             self._times[nick][func] = current_time
             self._times[self.nick][func] = current_time
             if not trigger.is_privmsg:
                 self._times[trigger.sender][func] = current_time
 
-    def _is_pretrigger_blocked(self, pretrigger):
-        if self.settings.core.nick_blocks or self.settings.core.host_blocks:
-            nick_blocked = self._nick_blocked(pretrigger.nick)
-            host_blocked = self._host_blocked(pretrigger.host)
-        else:
-            nick_blocked = host_blocked = None
+    def _is_pretrigger_blocked(
+        self,
+        pretrigger: PreTrigger,
+    ) -> Union[tuple[bool, bool], tuple[None, None]]:
+        if not (
+            self.settings.core.nick_blocks
+            or self.settings.core.host_blocks
+        ):
+            return (None, None)
 
+        nick_blocked = self._nick_blocked(pretrigger.nick)
+        host_blocked = self._host_blocked(pretrigger.host)
         return (nick_blocked, host_blocked)
 
-    def dispatch(self, pretrigger):
+    def dispatch(self, pretrigger: PreTrigger) -> None:
         """Dispatch a parsed message to any registered callables.
 
         :param pretrigger: a parsed message from the server
         :type pretrigger: :class:`~sopel.trigger.PreTrigger`
 
         The ``pretrigger`` (a parsed message) is used to find matching rules;
         it will retrieve them by order of priority, and execute them. It runs
@@ -900,14 +844,20 @@
         blocked = bool(nick_blocked or host_blocked)
         list_of_blocked_rules = set()
         # account info
         nick = pretrigger.nick
         user_obj = self.users.get(nick)
         account = user_obj.account if user_obj else None
 
+        # skip processing replayed messages
+        if "time" in pretrigger.tags and pretrigger.sender in self.channels:
+            join_time = self.channels[pretrigger.sender].join_time
+            if join_time is not None and pretrigger.time < join_time:
+                return
+
         for rule, match in self._rules_manager.get_triggered_rules(self, pretrigger):
             trigger = Trigger(self.settings, pretrigger, match, account)
 
             is_unblockable = trigger.admin or rule.is_unblockable()
             if blocked and not is_unblockable:
                 list_of_blocked_rules.add(str(rule))
                 continue
@@ -942,26 +892,26 @@
                 "%s prevented from using %s by %s.",
                 pretrigger.nick,
                 ', '.join(list_of_blocked_rules),
                 block_type,
             )
 
     @property
-    def running_triggers(self):
+    def running_triggers(self) -> list:
         """Current active threads for triggers.
 
         :return: the running thread(s) currently processing trigger(s)
         :rtype: :term:`iterable`
 
         This is for testing and debugging purposes only.
         """
         with self._running_triggers_lock:
             return [t for t in self._running_triggers if t.is_alive()]
 
-    def _update_running_triggers(self, running_triggers):
+    def _update_running_triggers(self, running_triggers: list) -> None:
         """Update list of running triggers.
 
         :param list running_triggers: newly started threads
 
         We want to keep track of running triggers, mostly for testing and
         debugging purposes. For instance, it'll help make sure, in tests, that
         a bot plugin has finished processing a trigger, by manually joining
@@ -972,99 +922,176 @@
         """
         # update bot's global running triggers
         with self._running_triggers_lock:
             running_triggers = running_triggers + self._running_triggers
             self._running_triggers = [
                 t for t in running_triggers if t.is_alive()]
 
+    # capability negotiation
+    def request_capabilities(self) -> bool:
+        """Request available capabilities and return if negotiation is on.
+
+        :return: tell if the negotiation is active or not
+
+        This takes the available capabilities and asks the request manager to
+        request only these that are available.
+
+        If none is available or if none is requested, the negotiation is not
+        active and this returns ``False``. It is the responsibility of the
+        caller to make sure it signals the IRC server to end the negotiation
+        with a ``CAP END`` command.
+        """
+        available_capabilities = self._capabilities.available.keys()
+
+        if not available_capabilities:
+            LOGGER.debug('No client capability to negotiate.')
+            return False
+
+        LOGGER.info(
+            "Client capability negotiation list: %s",
+            ', '.join(available_capabilities),
+        )
+
+        self._cap_requests_manager.request_available(
+            self, available_capabilities)
+
+        return bool(self._cap_requests_manager.requested)
+
+    def resume_capability_negotiation(
+        self,
+        cap_req: tuple[str, ...],
+        plugin_name: str,
+    ) -> None:
+        """Resume capability negotiation and close when necessary.
+
+        :param cap_req: a capability request
+        :param plugin_name: plugin that requested the capability and wants to
+                            resume capability negotiation
+
+        This will resume a capability request through the bot's
+        :attr:`capability requests manager<cap_requests>`, and if the
+        negotiation wasn't completed before and is now complete, it will send
+        a ``CAP END`` command.
+
+        This method must be used by plugins that declare a capability request
+        with a handler that returns
+        :attr:`sopel.plugin.CapabilityNegotiation.CONTINUE` on acknowledgement
+        in order for the bot to resume and eventually close negotiation.
+
+        For example, this is useful for SASL auth which happens while
+        negotiating capabilities.
+        """
+        was_completed, is_complete = self._cap_requests_manager.resume(
+            cap_req, plugin_name,
+        )
+        if not was_completed and is_complete:
+            LOGGER.info("End of client capability negotiation requests.")
+            self.write(('CAP', 'END'))
+
     # event handlers
 
-    def on_scheduler_error(self, scheduler, exc):
+    def on_scheduler_error(
+        self,
+        scheduler: plugin_jobs.Scheduler,
+        exc: BaseException,
+    ):
         """Called when the Job Scheduler fails.
 
         :param scheduler: the job scheduler that errored
         :type scheduler: :class:`sopel.plugins.jobs.Scheduler`
         :param Exception exc: the raised exception
 
         .. seealso::
 
             :meth:`Sopel.error`
         """
         self.error(exception=exc)
 
-    def on_job_error(self, scheduler, job, exc):
+    def on_job_error(
+        self,
+        scheduler: plugin_jobs.Scheduler,
+        job: tools_jobs.Job,
+        exc: BaseException,
+    ):
         """Called when a job from the Job Scheduler fails.
 
         :param scheduler: the job scheduler responsible for the errored ``job``
         :type scheduler: :class:`sopel.plugins.jobs.Scheduler`
         :param job: the Job that errored
         :type job: :class:`sopel.tools.jobs.Job`
         :param Exception exc: the raised exception
 
         .. seealso::
 
             :meth:`Sopel.error`
         """
         self.error(exception=exc)
 
-    def error(self, trigger=None, exception=None):
+    def error(
+        self,
+        trigger: Optional[Trigger] = None,
+        exception: Optional[BaseException] = None,
+    ):
         """Called internally when a plugin causes an error.
 
         :param trigger: the ``Trigger``\\ing line (if available)
         :type trigger: :class:`sopel.trigger.Trigger`
         :param Exception exception: the exception raised by the error (if
                                     available)
         """
         message = 'Unexpected error'
         if exception:
-            message = '{} ({})'.format(message, exception)
+            detail = ' ({})'.format(exception) if str(exception) else ''
+            message = 'Unexpected {}{}'.format(type(exception).__name__, detail)
 
         if trigger:
-            message = '{} from {} at {}. Message was: {}'.format(
-                message, trigger.nick, str(datetime.utcnow()), trigger.group(0)
+            message = '{} from {}. Message was: {}'.format(
+                message, trigger.nick, trigger.group(0)
             )
 
         LOGGER.exception(message)
 
         if trigger and self.settings.core.reply_errors and trigger.sender is not None:
             self.say(message, trigger.sender)
 
-    def _host_blocked(self, host):
+    def _host_blocked(self, host: str) -> bool:
         """Check if a hostname is blocked.
 
         :param str host: the hostname to check
         """
         bad_masks = self.config.core.host_blocks
         for bad_mask in bad_masks:
             bad_mask = bad_mask.strip()
             if not bad_mask:
                 continue
             if (re.match(bad_mask + '$', host, re.IGNORECASE) or
                     bad_mask == host):
                 return True
         return False
 
-    def _nick_blocked(self, nick):
+    def _nick_blocked(self, nick: str) -> bool:
         """Check if a nickname is blocked.
 
         :param str nick: the nickname to check
         """
         bad_nicks = self.config.core.nick_blocks
         for bad_nick in bad_nicks:
             bad_nick = bad_nick.strip()
             if not bad_nick:
                 continue
             if (re.match(bad_nick + '$', nick, re.IGNORECASE) or
-                    Identifier(bad_nick) == nick):
+                    self.make_identifier(bad_nick) == nick):
                 return True
         return False
 
-    def _shutdown(self):
+    def _shutdown(self) -> None:
         """Internal bot shutdown method."""
         LOGGER.info("Shutting down")
+        # Proactively tell plugins (at least the ones that bother to check)
+        self._connection_registered.clear()
         # Stop Job Scheduler
         LOGGER.info("Stopping the Job Scheduler.")
         self._scheduler.stop()
 
         try:
             self._scheduler.join(timeout=15)
         except RuntimeError:
@@ -1127,25 +1154,24 @@
         callbacks through the use of :func:`sopel.plugin.url`.
 
         .. deprecated:: 7.1
 
             Made obsolete by fixes to the behavior of
             :func:`sopel.plugin.url`. Will be removed in Sopel 9.
 
-        """
-        if 'url_callbacks' not in self.memory:
-            self.memory['url_callbacks'] = tools.SopelMemory()
+        .. versionchanged:: 8.0
+
+            Stores registered callbacks in an internal property instead of
+            ``bot.memory['url_callbacks']``.
 
-        if isinstance(pattern, basestring):
+        """
+        if isinstance(pattern, str):
             pattern = re.compile(pattern)
 
-        # Mark the callback as checked: using this method is safe.
-        # TODO: remove in Sopel 8
-        setattr(callback, '_sopel_url_callbacks_checked', True)
-        self.memory['url_callbacks'][pattern] = callback
+        self._url_callbacks[pattern] = callback
 
     @deprecated(
         reason='Issues with @url decorator have been fixed. Simply use that.',
         version='7.1',
         warning_in='8.0',
         removed_in='9.0',
     )
@@ -1177,27 +1203,36 @@
         callbacks through the use of :func:`sopel.plugin.url`.
 
         .. deprecated:: 7.1
 
             Made obsolete by fixes to the behavior of
             :func:`sopel.plugin.url`. Will be removed in Sopel 9.
 
-        """
-        if 'url_callbacks' not in self.memory:
-            # nothing to unregister
-            return
+        .. versionchanged:: 8.0
+
+            Deletes registered callbacks from an internal property instead of
+            ``bot.memory['url_callbacks']``.
 
-        if isinstance(pattern, basestring):
+        """
+        if isinstance(pattern, str):
             pattern = re.compile(pattern)
 
         try:
-            del self.memory['url_callbacks'][pattern]
+            del self._url_callbacks[pattern]
         except KeyError:
             pass
 
+    @deprecated(
+        reason=(
+            'URL handling has been unified in the Rules system via the @url '
+            'decorator. Use RuleManager.check_url_callbacks() if needed.'),
+        version='8.0',
+        warning_in='8.1',
+        removed_in='9.0',
+    )
     def search_url_callbacks(self, url):
         """Yield callbacks whose regex pattern matches the ``url``.
 
         :param str url: URL found in a trigger
         :return: yield 2-value tuples of ``(callback, match)``
 
         For each pattern that matches the ``url`` parameter, it yields a
@@ -1205,55 +1240,59 @@
 
         The ``callable`` is the one registered with
         :meth:`register_url_callback`, and the ``match`` is the result of
         the regex pattern's ``search`` method.
 
         .. versionadded:: 7.0
 
+        .. versionchanged:: 8.0
+
+            Searches for registered callbacks in an internal property instead
+            of ``bot.memory['url_callbacks']``.
+
+        .. deprecated:: 8.0
+
+            Made obsolete by fixes to the behavior of
+            :func:`sopel.plugin.url`. Will be removed in Sopel 9.
+
         .. seealso::
 
             The Python documentation for the `re.search`__ function and
             the `match object`__.
 
-        .. __: https://docs.python.org/3.6/library/re.html#re.search
-        .. __: https://docs.python.org/3.6/library/re.html#match-objects
+        .. __: https://docs.python.org/3.11/library/re.html#re.search
+        .. __: https://docs.python.org/3.11/library/re.html#match-objects
 
         """
-        if 'url_callbacks' not in self.memory:
-            # nothing to search
-            return
-
-        for regex, function in tools.iteritems(self.memory['url_callbacks']):
+        for regex, function in self._url_callbacks.items():
             match = regex.search(url)
             if match:
                 yield function, match
 
-    def restart(self, message):
-        """Disconnect from IRC and restart the bot.
-
-        :param str message: QUIT message to send (e.g. "Be right back!")
-        """
-        self.wantsrestart = True
-        self.quit(message)
-
 
-class SopelWrapper(object):
+class SopelWrapper:
     """Wrapper around a Sopel instance and a Trigger.
 
     :param sopel: Sopel instance
     :type sopel: :class:`~sopel.bot.Sopel`
     :param trigger: IRC Trigger line
     :type trigger: :class:`~sopel.trigger.Trigger`
     :param str output_prefix: prefix for messages sent through this wrapper
                               (e.g. plugin tag)
 
     This wrapper will be used to call Sopel's triggered commands and rules as
-    their ``bot`` argument. It acts as a proxy to :meth:`send messages<say>`
-    to the sender (either a channel or in a private message) and even to
-    :meth:`reply to someone<reply>` in a channel.
+    their ``bot`` argument. It acts as a proxy, providing the ``trigger``'s
+    ``sender`` (source channel or private message) as the default
+    ``destination`` argument for overridden methods.
+
+    .. deprecated:: 8.0
+
+        ``SopelWrapper`` will be replaced with a ``contextvars`` based
+        alternative. For more information, see :issue:`2460`.
+
     """
     def __init__(self, sopel, trigger, output_prefix=''):
         if not output_prefix:
             # Just in case someone passes in False, None, etc.
             output_prefix = ''
         # The custom __setattr__ for this class sets the attribute on the
         # original bot object. We don't want that for these, so we set them
@@ -1269,14 +1308,43 @@
 
     def __getattr__(self, attr):
         return getattr(self._bot, attr)
 
     def __setattr__(self, attr, value):
         return setattr(self._bot, attr, value)
 
+    @property
+    def default_destination(self) -> Optional[str]:
+        """Default say/reply destination for the associated Trigger.
+
+        :return: the channel (with status prefix) or nick to send messages to
+
+        This property returns the :class:`str` version of the destination that
+        will be used by default by these methods:
+
+        * :meth:`say`
+        * :meth:`reply`
+        * :meth:`action`
+        * :meth:`notice`
+
+        For a channel, it also ensures that the status-specific prefix is added
+        to the result, so the bot replies with the same status.
+        """
+        if not self._trigger.sender:
+            return None
+
+        # ensure str and not Identifier
+        destination = str(self._trigger.sender)
+
+        # prepend status prefix if it exists
+        if self._trigger.status_prefix:
+            destination = self._trigger.status_prefix + destination
+
+        return destination
+
     def say(self, message, destination=None, max_messages=1, truncation='', trailing=''):
         """Override ``Sopel.say`` to use trigger source by default.
 
         :param str message: message to say
         :param str destination: channel or nickname; defaults to
             :attr:`trigger.sender <sopel.trigger.Trigger.sender>`
         :param int max_messages: split ``message`` into at most this many
@@ -1293,16 +1361,23 @@
         .. seealso::
 
             For more details about the optional arguments to this wrapper
             method, consult the documentation for :meth:`sopel.bot.Sopel.say`.
 
         """
         if destination is None:
-            destination = self._trigger.sender
-        self._bot.say(self._out_pfx + message, destination, max_messages, truncation, trailing)
+            destination = self.default_destination
+
+        self._bot.say(
+            self._out_pfx + message,
+            destination,
+            max_messages,
+            truncation,
+            trailing,
+        )
 
     def action(self, message, destination=None):
         """Override ``Sopel.action`` to use trigger source by default.
 
         :param str message: action message
         :param str destination: channel or nickname; defaults to
             :attr:`trigger.sender <sopel.trigger.Trigger.sender>`
@@ -1311,15 +1386,16 @@
         trigger happened (or nickname, if received in a private message).
 
         .. seealso::
 
             :meth:`sopel.bot.Sopel.action`
         """
         if destination is None:
-            destination = self._trigger.sender
+            destination = self.default_destination
+
         self._bot.action(message, destination)
 
     def notice(self, message, destination=None):
         """Override ``Sopel.notice`` to use trigger source by default.
 
         :param str message: notice message
         :param str destination: channel or nickname; defaults to
@@ -1329,15 +1405,16 @@
         trigger happened (or nickname, if received in a private message).
 
         .. seealso::
 
             :meth:`sopel.bot.Sopel.notice`
         """
         if destination is None:
-            destination = self._trigger.sender
+            destination = self.default_destination
+
         self._bot.notice(self._out_pfx + message, destination)
 
     def reply(self, message, destination=None, reply_to=None, notice=False):
         """Override ``Sopel.reply`` to ``reply_to`` sender by default.
 
         :param str message: reply message
         :param str destination: channel or nickname; defaults to
@@ -1352,17 +1429,19 @@
         ``reply_to`` will default to the nickname who sent the trigger.
 
         .. seealso::
 
             :meth:`sopel.bot.Sopel.reply`
         """
         if destination is None:
-            destination = self._trigger.sender
+            destination = self.default_destination
+
         if reply_to is None:
             reply_to = self._trigger.nick
+
         self._bot.reply(message, destination, reply_to, notice)
 
     def kick(self, nick, channel=None, message=None):
         """Override ``Sopel.kick`` to kick in a channel
 
         :param str nick: nick to kick out of the ``channel``
         :param str channel: optional channel to kick ``nick`` from
@@ -1377,10 +1456,12 @@
             :meth:`sopel.bot.Sopel.kick`
         """
         if channel is None:
             if self._trigger.is_privmsg:
                 raise RuntimeError('Error: KICK requires a channel.')
             else:
                 channel = self._trigger.sender
+
         if nick is None:
             raise RuntimeError('Error: KICK requires a nick.')
+
         self._bot.kick(nick, channel, message)
```

### Comparing `sopel-7.1.9/sopel/cli/config.py` & `sopel-8.0.0/sopel/cli/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# coding=utf-8
 """Sopel Config Command Line Interface (CLI): ``sopel-config``"""
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import argparse
 import os
 
-from sopel import tools
 from . import utils
 
 
 def build_parser():
     """Build and configure an argument parser for ``sopel-config``.
 
     :return: the argument parser
@@ -105,16 +103,16 @@
         if display_path:
             print(os.path.join(configdir, config_filename))
         else:
             name, _ = os.path.splitext(config_filename)
             print(name)
 
     if not found:
-        tools.stderr('No config file found at this location: %s' % configdir)
-        tools.stderr('Use `sopel-config init` to create a new config file.')
+        utils.stderr('No config file found at this location: %s' % configdir)
+        utils.stderr('Use `sopel-config init` to create a new config file.')
 
     return 0  # successful operation
 
 
 def handle_init(options):
     """Use config wizard to initialize a new configuration file for the bot.
 
@@ -129,28 +127,28 @@
        extension **must be** ``.cfg``.
 
     """
     config_filename = utils.find_config(options.configdir, options.config)
     config_name, ext = os.path.splitext(config_filename)
 
     if ext and ext != '.cfg':
-        tools.stderr('Configuration wizard accepts .cfg files only')
+        utils.stderr('Configuration wizard accepts .cfg files only')
         return 1
     elif not ext:
         config_filename = config_name + '.cfg'
 
     if os.path.isfile(config_filename):
-        tools.stderr('Configuration file %s already exists' % config_filename)
+        utils.stderr('Configuration file %s already exists' % config_filename)
         return 1
 
     print('Starting Sopel config wizard for: %s' % config_filename)
     try:
         utils.wizard(config_name)
     except KeyboardInterrupt:
-        tools.stderr('\nOperation cancelled; no file has been created.')
+        utils.stderr('\nOperation cancelled; no file has been created.')
         return 1  # cancelled operation
 
     return 0  # successful operation
 
 
 def handle_get(options):
     """Read the settings to display the value of ``<section> <key>``.
@@ -160,26 +158,26 @@
     :return: 0 if everything went fine;
              1 if the section and/or key does not exist;
              2 if the settings can't be loaded
     """
     try:
         settings = utils.load_settings(options)
     except Exception as error:
-        tools.stderr(error)
+        utils.stderr(error)
         return 2
 
     section = options.section
     option = options.option
 
     # Making sure the section.option exists
     if not settings.parser.has_section(section):
-        tools.stderr('Section "%s" does not exist' % section)
+        utils.stderr('Section "%s" does not exist' % section)
         return 1
     if not settings.parser.has_option(section, option):
-        tools.stderr(
+        utils.stderr(
             'Section "%s" does not have a "%s" option' % (section, option))
         return 1
 
     # Display the value
     print(settings.get(section, option))
     return 0  # successful operation
```

### Comparing `sopel-7.1.9/sopel/cli/plugins.py` & `sopel-8.0.0/sopel/cli/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding=utf-8
 """Sopel Plugins Command Line Interface (CLI): ``sopel-plugins``"""
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import argparse
 import inspect
 import operator
 
-from sopel import config, plugins, tools
+from sopel import config, plugins
 from . import utils
 
 
 ERR_CODE = 1
 """Error code: program exited with an error"""
 
 
@@ -188,17 +187,17 @@
     elif disabled_only:
         items = (
             (name, plugin, is_enabled)
             for name, plugin, is_enabled in items
             if not is_enabled
         )
     # sort plugins
-    items = sorted(items, key=operator.itemgetter(0))
+    sorted_plugins = sorted(items, key=operator.itemgetter(0))
 
-    for name, plugin, is_enabled in items:
+    for name, plugin, is_enabled in sorted_plugins:
         description = {
             'name': name,
             'status': 'enabled' if is_enabled else 'disabled',
         }
 
         # optional meta description from the plugin itself
         try:
@@ -251,15 +250,15 @@
     """
     plugin_name = options.name
     settings = utils.load_settings(options)
     usable_plugins = plugins.get_usable_plugins(settings)
 
     # plugin does not exist
     if plugin_name not in usable_plugins:
-        tools.stderr('No plugin named %s' % plugin_name)
+        utils.stderr('No plugin named %s' % plugin_name)
         return ERR_CODE
 
     plugin, is_enabled = usable_plugins[plugin_name]
     description = {
         'name': plugin_name,
         'status': 'enabled' if is_enabled else 'disabled',
     }
@@ -310,66 +309,66 @@
     """
     plugin_name = options.name
     settings = utils.load_settings(options)
     usable_plugins = plugins.get_usable_plugins(settings)
 
     # plugin does not exist
     if plugin_name not in usable_plugins:
-        tools.stderr('No plugin named %s' % plugin_name)
+        utils.stderr('No plugin named %s' % plugin_name)
         return ERR_CODE
 
     plugin, is_enabled = usable_plugins[plugin_name]
     try:
         plugin.load()
     except Exception as error:
-        tools.stderr('Cannot load plugin %s: %s' % (plugin_name, error))
+        utils.stderr('Cannot load plugin %s: %s' % (plugin_name, error))
         return ERR_CODE
 
     if not plugin.has_configure():
-        tools.stderr('Nothing to configure for plugin %s' % plugin_name)
+        utils.stderr('Nothing to configure for plugin %s' % plugin_name)
         return 0  # nothing to configure is not exactly an error case
 
     print('Configure %s' % plugin.get_label())
     try:
         plugin.configure(settings)
     except KeyboardInterrupt:
-        tools.stderr(
+        utils.stderr(
             '\nOperation cancelled; the config file has not been modified.')
         return ERR_CODE  # cancelled operation
 
     settings.save()
 
     if not is_enabled:
-        tools.stderr(
+        utils.stderr(
             "Plugin {0} has been configured but is not enabled. "
             "Use 'sopel-plugins enable {0}' to enable it".format(plugin_name)
         )
 
     return 0  # successful operation
 
 
 def _handle_disable_plugin(settings, plugin_name, force):
     excluded = settings.core.exclude
     # nothing left to do if already excluded
     if plugin_name in excluded:
-        tools.stderr('Plugin %s already disabled.' % plugin_name)
+        utils.stderr('Plugin %s already disabled.' % plugin_name)
         return False
 
     # recalculate state: at the moment, the plugin is not in the excluded list
     # however, with ensure_remove, the enable list may be empty, so we have
     # to compute the plugin's state here, and not use what comes from
     # plugins.get_usable_plugins
     is_enabled = (
         not settings.core.enable or
         plugin_name in settings.core.enable
     )
 
     # if not enabled at this point, exclude if options.force is used
     if not is_enabled and not force:
-        tools.stderr(
+        utils.stderr(
             'Plugin %s is disabled but not excluded; '
             'use -f/--force to force its exclusion.'
             % plugin_name)
         return False
 
     settings.core.exclude = excluded + [plugin_name]
     return True
@@ -377,15 +376,15 @@
 
 def display_unknown_plugins(unknown_plugins):
     """Print an error message when one or more plugins are unknown.
 
     :param list unknown_plugins: list of unknown plugins
     """
     # at least one of the plugins does not exist
-    tools.stderr(utils.get_many_text(
+    utils.stderr(utils.get_many_text(
         unknown_plugins,
         one='No plugin named {item}.',
         two='No plugin named {first} or {second}.',
         many='No plugin named {left}, or {last}.'
     ))
 
 
@@ -399,19 +398,18 @@
              or if attempting to disable coretasks (required)
     """
     plugin_names = options.names
     force = options.force
     ensure_remove = options.remove
     settings = utils.load_settings(options)
     usable_plugins = plugins.get_usable_plugins(settings)
-    actually_disabled = []
 
     # coretasks is sacred
     if 'coretasks' in plugin_names:
-        tools.stderr('Plugin coretasks cannot be disabled.')
+        utils.stderr('Plugin coretasks cannot be disabled.')
         return ERR_CODE  # do nothing and return an error code
 
     unknown_plugins = [
         name
         for name in plugin_names
         if name not in usable_plugins
     ]
@@ -454,26 +452,26 @@
 
 def _handle_enable_plugin(settings, usable_plugins, plugin_name, allow_only):
     enabled = settings.core.enable
     excluded = settings.core.exclude
 
     # coretasks is sacred
     if plugin_name == 'coretasks':
-        tools.stderr('Plugin coretasks is always enabled.')
+        utils.stderr('Plugin coretasks is always enabled.')
         return False
 
     # is it already enabled, but should we enforce anything?
     is_enabled = usable_plugins[plugin_name][1]
     if is_enabled and not allow_only:
         # already enabled, and no allow-only option: all good
         if plugin_name in enabled:
-            tools.stderr('Plugin %s is already enabled.' % plugin_name)
+            utils.stderr('Plugin %s is already enabled.' % plugin_name)
         else:
             # suggest to use --allow-only option
-            tools.stderr(
+            utils.stderr(
                 'Plugin %s is enabled; '
                 'use option -a/--allow-only to enforce allow only policy.'
                 % plugin_name)
 
         return False
 
     # not enabled, or option allow_only to enforce
@@ -482,15 +480,15 @@
         settings.core.exclude = [
             name
             for name in settings.core.exclude
             if plugin_name != name
         ]
     elif plugin_name in enabled:
         # not excluded, and already in enabled list: all good
-        tools.stderr('Plugin %s is already enabled' % plugin_name)
+        utils.stderr('Plugin %s is already enabled' % plugin_name)
         return False
 
     if plugin_name not in enabled and (enabled or allow_only):
         # not excluded, but not enabled either: allow-only mode required
         # either because of the current configuration, or by request
         settings.core.enable = enabled + [plugin_name]
 
@@ -560,13 +558,13 @@
         elif action == 'configure':
             return handle_configure(options)
         elif action == 'disable':
             return handle_disable(options)
         elif action == 'enable':
             return handle_enable(options)
     except KeyboardInterrupt:
-        tools.stderr('Bye!')
+        utils.stderr('Bye!')
         return ERR_CODE
     except config.ConfigurationNotFound as err:
-        tools.stderr(err)
-        tools.stderr('Use `sopel-config init` to create a new config file.')
+        utils.stderr(err)
+        utils.stderr('Use `sopel-config init` to create a new config file.')
         return ERR_CODE
```

### Comparing `sopel-7.1.9/sopel/cli/utils.py` & `sopel-8.0.0/sopel/cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# coding=utf-8
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import inspect
 import logging
 import os
 import sys
 
-from sopel import config, plugins, tools
+from sopel import config, plugins
 
 # Allow clean import *
 __all__ = [
     'enumerate_configs',
     'find_config',
     'add_common_arguments',
     'load_settings',
-    'redirect_outputs',
     'wizard',
     'plugins_wizard',
     # colors
     'green',
     'yellow',
     'red',
 ]
@@ -87,15 +85,15 @@
 
     try:
         if not os.path.isdir(configdir):
             print('Creating config directory at {}'.format(configdir))
             os.makedirs(configdir)
             print('Config directory created')
     except Exception:
-        tools.stderr('There was a problem creating {}'.format(configdir))
+        stderr('There was a problem creating {}'.format(configdir))
         raise
 
     name, ext = os.path.splitext(basename)
     if not ext:
         # Always add .cfg if filename does not have an extension
         filename = os.path.join(configdir, name + '.cfg')
     elif ext != '.cfg':
@@ -114,16 +112,16 @@
         'that need configuring'
     ):
         _plugins_wizard(settings)
 
     try:
         settings.save()
     except Exception:  # TODO: Be specific
-        tools.stderr("Encountered an error while writing the config file. "
-                     "This shouldn't happen. Check permissions.")
+        stderr("Encountered an error while writing the config file. "
+               "This shouldn't happen. Check permissions.")
         raise
 
     print("Config file written successfully!")
     return settings
 
 
 def plugins_wizard(filename):
@@ -140,16 +138,16 @@
 
     settings = config.Config(filename, validate=False)
     _plugins_wizard(settings)
 
     try:
         settings.save()
     except Exception:  # TODO: Be specific
-        tools.stderr("Encountered an error while writing the config file. "
-                     "This shouldn't happen. Check permissions.")
+        stderr("Encountered an error while writing the config file. "
+               "This shouldn't happen. Check permissions.")
         raise
 
     return settings
 
 
 def _plugins_wizard(settings):
     usable_plugins = plugins.get_usable_plugins(settings)
@@ -196,55 +194,64 @@
         return
 
     for item in os.listdir(config_dir):
         if item.endswith(extension):
             yield item
 
 
-def find_config(config_dir, name, extension='.cfg'):
+def find_config(config_dir: str, name: str, extension: str = '.cfg') -> str:
     """Build the absolute path for the given configuration file ``name``.
 
-    :param str config_dir: path to the configuration directory
-    :param str name: configuration file ``name``
-    :param str extension: configuration file's extension (default to ``.cfg``)
-    :return: the path of the configuration file, either in the current
-             directory or from the ``config_dir`` directory
-
-    This function tries different locations:
-
-    * the current directory
-    * the ``config_dir`` directory with the ``extension`` suffix
-    * the ``config_dir`` directory without a suffix
+    :param config_dir: path to the configuration directory
+    :param name: configuration file ``name``
+    :param extension: configuration file's extension (defaults to ``.cfg``)
+    :return: the absolute path to the configuration file, either in the current
+             directory or in the ``config_dir`` directory
+
+    This function appends the extension if absent before checking the following:
+
+    * If ``name`` is an absolute path, it is returned whether it exists or not
+    * If ``name`` exists in the ``config_dir``, the absolute path is returned
+    * If ``name`` exists in the current directory, its absolute path is returned
+    * Otherwise, the path to the nonexistent file within ``config_dir`` is returned
 
     Example::
 
         >>> from sopel.cli import utils
         >>> from sopel import config
+        >>> os.getcwd()
+        '/sopel'
         >>> os.listdir()
         ['local.cfg', 'extra.ini']
         >>> os.listdir(config.DEFAULT_HOMEDIR)
-        ['config.cfg', 'extra.ini', 'plugin.cfg', 'README']
+        ['config.cfg', 'extra.ini', 'logs', 'plugins']
         >>> utils.find_config(config.DEFAULT_HOMEDIR, 'local.cfg')
-        'local.cfg'
-        >>> utils.find_config(config.DEFAULT_HOMEDIR, 'local')
-        '/home/username/.sopel/local'
+        '/sopel/local.cfg'
         >>> utils.find_config(config.DEFAULT_HOMEDIR, 'config')
         '/home/username/.sopel/config.cfg'
         >>> utils.find_config(config.DEFAULT_HOMEDIR, 'extra', '.ini')
         '/home/username/.sopel/extra.ini'
 
+    .. versionchanged:: 8.0
+
+        Files in the ``config_dir`` are now preferred, and files without the
+        requested extension are no longer returned.
+
     """
-    if os.path.isfile(name):
-        return os.path.abspath(name)
-    name_ext = name + extension
-    for filename in enumerate_configs(config_dir, extension):
-        if name_ext == filename:
-            return os.path.join(config_dir, name_ext)
+    if not name.endswith(extension):
+        name = name + extension
 
-    return os.path.join(config_dir, name)
+    if os.path.isabs(name):
+        return name
+    conf_dir_name = os.path.join(config_dir, name)
+    if os.path.isfile(conf_dir_name):
+        return conf_dir_name
+    elif os.path.isfile(name):
+        return os.path.abspath(name)
+    return conf_dir_name
 
 
 def add_common_arguments(parser):
     """Add common and configuration-related arguments to a ``parser``.
 
     :param parser: Argument parser (or subparser)
     :type parser: argparse.ArgumentParser
@@ -338,38 +345,14 @@
 
     if not os.path.isfile(filename):
         raise config.ConfigurationNotFound(filename=filename)
 
     return config.Config(filename)
 
 
-@tools.deprecated(reason='Obsoleted by modernized logging.',
-                  version='7.0',
-                  removed_in='8.0')
-def redirect_outputs(settings, is_quiet=False):
-    """Redirect ``sys``'s outputs using Sopel's settings.
-
-    :param settings: Sopel's configuration
-    :type settings: :class:`sopel.config.Config`
-    :param bool is_quiet: Optional, set to True to make Sopel's outputs quiet
-
-    Both ``sys.stderr`` and ``sys.stdout`` are redirected to a logfile.
-
-    .. deprecated:: 7.0
-
-        Sopel now uses the built-in logging system for its output, and this
-        function is now deprecated.
-
-    """
-    logfile = os.path.os.path.join(
-        settings.core.logdir, settings.basename + '.stdio.log')
-    sys.stderr = tools.OutputRedirect(logfile, True, is_quiet)
-    sys.stdout = tools.OutputRedirect(logfile, False, is_quiet)
-
-
 def get_many_text(items, one, two, many):
     """Get the right text based on the number of ``items``."""
     message = ''
     if not items:
         return message
 
     items_count = len(items)
@@ -380,7 +363,50 @@
         message = two.format(first=items[0], second=items[1])
     else:
         left = ', '.join(items[:-1])
         last = items[-1]
         message = many.format(left=left, last=last)
 
     return message
+
+
+def check_pid(pid):
+    """Check if a process is running with the given ``PID``.
+
+    :param int pid: PID to check
+    :return bool: ``True`` if the given PID is running, ``False`` otherwise
+
+    *Availability: POSIX systems only.*
+
+    .. versionchanged:: 8.0
+
+        Moved from :mod:`sopel.tools` to :mod:`sopel.cli.utils`.
+
+    .. note::
+
+        Matching the :py:func:`os.kill` behavior this function needs on Windows
+        was rejected in
+        `Python issue #14480 <https://bugs.python.org/issue14480>`_, so
+        :func:`check_pid` cannot be used on Windows systems.
+
+    """
+    try:
+        os.kill(pid, 0)
+    except OSError:
+        return False
+    else:
+        return True
+
+
+def stderr(string):
+    """Print the given ``string`` to stderr.
+
+    :param str string: the string to output
+
+    Just a convenience function.
+
+    .. versionchanged:: 8.0
+
+        Moved from :mod:`sopel.tools` to :mod:`sopel.cli.utils`.
+
+    """
+    print(string, file=sys.stderr)
```

### Comparing `sopel-7.1.9/sopel/config/__init__.py` & `sopel-8.0.0/sopel/config/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 """Sopel's configuration module.
 
 The :class:`~sopel.config.Config` object provides an interface to access Sopel's
 configuration file. It exposes the configuration's sections through its
 attributes as objects, which in turn expose their directives through *their*
 attributes.
 
@@ -44,28 +43,21 @@
 
 .. versionadded:: 6.0.0
 """
 # Copyright 2012-2015, Elsie Powell, embolalia.com
 # Copyright © 2012, Elad Alfassa <elad@fedoraproject.org>
 # Licensed under the Eiffel Forum License 2.
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+import configparser
 import os
-import sys
 
-from sopel import tools
 from . import core_section, types
 
-if sys.version_info.major < 3:
-    import ConfigParser
-else:
-    basestring = str
-    import configparser as ConfigParser
-
 
 __all__ = [
     'core_section',
     'types',
     'DEFAULT_HOMEDIR',
     'ConfigurationError',
     'ConfigurationNotFound',
@@ -89,23 +81,23 @@
 
 class ConfigurationNotFound(ConfigurationError):
     """Exception type for use when the configuration file cannot be found.
 
     :param str filename: file path that could not be found
     """
     def __init__(self, filename):
-        super(ConfigurationNotFound, self).__init__(None)
+        super().__init__(None)
         self.filename = filename
         """Path to the configuration file that could not be found."""
 
     def __str__(self):
         return 'Unable to find the configuration file %s' % self.filename
 
 
-class Config(object):
+class Config:
     """The bot's configuration.
 
     :param str filename: the configuration file to load and use to populate this
                          ``Config`` instance
     :param bool validate: if ``True``, validate values in the ``[core]`` section
                           when it is loaded (optional; ``True`` by default)
 
@@ -127,15 +119,15 @@
 
         If the filename is ``libera.config.cfg``, then the ``basename`` will
         be ``libera.config``.
 
         The config's ``basename`` is useful as a component :ref:`of log file
         names <logging-basename>`, for example.
         """
-        self.parser = ConfigParser.RawConfigParser(allow_no_value=True)
+        self.parser = configparser.RawConfigParser(allow_no_value=True)
         """The configuration parser object that does the heavy lifting.
 
         .. seealso::
 
             Python's built-in :mod:`configparser` module and its
             :class:`~configparser.RawConfigParser` class.
 
@@ -196,18 +188,17 @@
 
             This will become less and less important as we continue to improve
             Sopel's tools for making automated changes to config files and
             eliminate most users' need to ever manually edit the text, but it's
             still worth keeping in mind.
 
         """
-        cfgfile = open(self.filename, 'w')
-        self.parser.write(cfgfile)
-        cfgfile.flush()
-        cfgfile.close()
+        with open(self.filename, 'w') as cfgfile:
+            self.parser.write(cfgfile)
+            cfgfile.flush()
 
     def add_section(self, name):
         """Add a new, empty section to the config file.
 
         :param str name: name of the new section
         :return: ``None`` if successful; ``False`` if a section named ``name``
                  already exists
@@ -221,28 +212,28 @@
             :meth:`define_section` and a child class of
             :class:`~.types.StaticSection`.
 
         .. important::
 
             The section's ``name`` SHOULD follow *snake_case* naming rules:
 
-              * use only lowercase letters, digits, and underscore (``_``)
-              * SHOULD NOT start with a digit
+            * use only lowercase letters, digits, and underscore (``_``)
+            * SHOULD NOT start with a digit
 
             Deviations from *snake_case* can break the following operations:
 
-              * :ref:`accessing the section <sopel.config>` from Python code using
-                the :class:`~.Config` object's attributes
-              * :ref:`overriding the section's values <Overriding individual
-                settings>` using environment variables
+            * :ref:`accessing the section <sopel.config>` from Python code
+              using the :class:`~.Config` object's attributes
+            * :ref:`overriding the section's values <Overriding individual
+              settings>` using environment variables
 
         """
         try:
             return self.parser.add_section(name)
-        except ConfigParser.DuplicateSectionError:
+        except configparser.DuplicateSectionError:
             return False
 
     def define_section(self, name, cls_, validate=True):
         """Define the available settings in a section.
 
         :param str name: name of the new section
         :param cls\\_: :term:`class` defining the settings within the section
@@ -258,23 +249,23 @@
         :func:`setup` function, for example, but might not be in the
         :func:`configure` function.
 
         .. important::
 
             The section's ``name`` SHOULD follow *snake_case* naming rules:
 
-              * use only lowercase letters, digits, and underscore (``_``)
-              * SHOULD NOT start with a digit
+            * use only lowercase letters, digits, and underscore (``_``)
+            * SHOULD NOT start with a digit
 
             Deviations from *snake_case* can break the following operations:
 
-              * :ref:`accessing the section <sopel.config>` from Python code using
-                the :class:`~.Config` object's attributes
-              * :ref:`overriding the section's values <Overriding individual
-                settings>` using environment variables
+            * :ref:`accessing the section <sopel.config>` from Python code
+              using the :class:`~.Config` object's attributes
+            * :ref:`overriding the section's values <Overriding individual
+              settings>` using environment variables
 
         """
         if not issubclass(cls_, types.StaticSection):
             raise ValueError("Class must be a subclass of StaticSection.")
         current = getattr(self, name, None)
         current_name = str(current.__class__)
         new_name = str(cls_)
@@ -282,15 +273,15 @@
                 not current_name == new_name):
             raise ValueError(
                 "Can not re-define class for section from {} to {}.".format(
                     current_name, new_name)
             )
         setattr(self, name, cls_(self, name, validate=validate))
 
-    class ConfigSection(object):
+    class ConfigSection:
         """Represents a section of the config file.
 
         :param str name: name of this section
         :param items: key-value pairs
         :type items: :term:`iterable` of two-item :class:`tuple`\\s
         :param parent: this section's containing object
         :type parent: :class:`Config`
@@ -315,37 +306,14 @@
 
         def __setattr__(self, name, value):
             object.__setattr__(self, name, value)
             if type(value) is list:
                 value = ','.join(value)
             self._parent.parser.set(self._name, name, value)
 
-        @tools.deprecated(
-            'No longer used; replaced by a dedicated ListAttribute type.'
-            '7.0', '8.0')
-        def get_list(self, name):
-            """Legacy way of getting a list from a config value.
-
-            :param str name: name of the attribute to fetch and interpret as a list
-            :return: the value of ``name`` as a list
-            :rtype: list
-
-            .. deprecated:: 7.0
-                Use :class:`~.types.ListAttribute` when storing a list value.
-                This legacy method will be removed in Sopel 8.0.
-            """
-            value = getattr(self, name)
-            if not value:
-                return []
-            if isinstance(value, basestring):
-                value = value.split(',')
-                # Keep the split value, so we don't have to keep doing this
-                setattr(self, name, value)
-            return value
-
     def __getattr__(self, name):
         if name in self.parser.sections():
             items = self.parser.items(name)
             section = self.ConfigSection(name, items, self)  # Return a section
             setattr(self, name, section)
             return section
         else:
@@ -371,11 +339,11 @@
         This will show a "y/n" prompt in the user's terminal, and return
         ``True`` or ``False`` based on the response. ``question`` should be
         phrased as a question, but without a question mark at the end.
         """
         d = 'n'
         if default:
             d = 'y'
-        ans = tools.get_input(question + ' (y/n)? [' + d + '] ')
+        ans = input(question + ' (y/n)? [' + d + '] ')
         if not ans:
             ans = d
         return ans.lower() == 'y'
```

### Comparing `sopel-7.1.9/sopel/config/core_section.py` & `sopel-8.0.0/sopel/config/core_section.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,44 @@
-# coding=utf-8
+from __future__ import annotations
 
-from __future__ import absolute_import, division, print_function, unicode_literals
-
-import os.path
+from ssl import TLSVersion
 
 from sopel.config.types import (
     BooleanAttribute,
     ChoiceAttribute,
     FilenameAttribute,
     ListAttribute,
     NO_DEFAULT,
     SecretAttribute,
     StaticSection,
     ValidatedAttribute,
 )
-from sopel.tools import Identifier
+from sopel.tools.identifiers import Identifier
 
 
 COMMAND_DEFAULT_PREFIX = r'\.'
 """Default prefix used for commands."""
 COMMAND_DEFAULT_HELP_PREFIX = '.'
 """Default help prefix used in commands' usage messages."""
 URL_DEFAULT_SCHEMES = ['http', 'https', 'ftp']
 """Default URL schemes allowed for URLs."""
 
 
-def _find_certs():
-    """Find the TLS root CA store.
+def _parse_ssl_version(var: str) -> TLSVersion:
+    """Parse an ssl_version config variable.
 
-    :returns: path to CA store file
-    :rtype: str
+    :param var: The input string, e.g. "TLSv1_3".
+    :return: The TLSVersion object for that version.
     """
-    # check if the root CA store is at a known location
-    locations = [
-        '/etc/pki/tls/cert.pem',  # best first guess
-        '/etc/ssl/certs/ca-certificates.crt',  # Debian
-        '/etc/ssl/cert.pem',  # FreeBSD base OpenSSL
-        '/usr/local/openssl/cert.pem',  # FreeBSD userland OpenSSL
-        '/etc/pki/tls/certs/ca-bundle.crt',  # RHEL 6 / Fedora
-        '/etc/pki/ca-trust/extracted/pem/tls-ca-bundle.pem',  # RHEL 7 / CentOS
-        '/etc/pki/tls/cacert.pem',  # OpenELEC
-        '/etc/ssl/ca-bundle.pem',  # OpenSUSE
-    ]
-    for certs in locations:
-        if os.path.isfile(certs):
-            return certs
-    return None
+    try:
+        return TLSVersion[var]
+    except KeyError:
+        raise ValueError(
+            "'{}' is not a valid TLSVersion. Try e.g. TLSv1_3'".format(var)
+        )
 
 
 def configure(config):
     """Interactively configure the bot's ``[core]`` config section.
 
     :param config: the bot's config object
     :type config: :class:`~.config.Config`
@@ -140,14 +129,100 @@
             Will
             Liam
 
     This would then allow both "William: Hi!" and "Bill: Hi!" to work with
     :func:`~sopel.plugin.nickname_command`.
     """
 
+    antiloop_repeat_text = ValidatedAttribute(
+        'antiloop_repeat_text', default='...')
+    """The replacement text sent when detecting a repeated message.
+
+    :default: ``...``
+
+    This is equivalent to the default value:
+
+    .. code-block:: ini
+
+        antiloop_repeat_text = ...
+
+    .. seealso::
+
+        The :ref:`Loop Prevention` chapter to learn what each antiloop-related
+        setting does.
+
+    .. versionadded:: 8.0
+    """
+
+    antiloop_silent_after = ValidatedAttribute(
+        'antiloop_silent_after', int, default=3)
+    """How many times the anti-looping message will be sent before stopping.
+
+    :default: ``3``
+
+    This is equivalent to the default value:
+
+    .. code-block:: ini
+
+        antiloop_silent_after = 3
+
+    .. seealso::
+
+        The :ref:`Loop Prevention` chapter to learn what each antiloop-related
+        setting does.
+
+    .. versionadded:: 8.0
+    """
+
+    antiloop_threshold = ValidatedAttribute(
+        'antiloop_threshold', int, default=5)
+    """How many times a message can be repeated without anti-looping action.
+
+    :default: ``5``
+
+    This is equivalent to the default value:
+
+    .. code-block:: ini
+
+        antiloop_threshold = 5
+
+    You can deactivate the anti-looping feature (not recommended) by setting
+    this to ``0``:
+
+    .. code-block:: ini
+
+        antiloop_threshold = 0
+
+    .. seealso::
+
+        The :ref:`Loop Prevention` chapter to learn what each antiloop-related
+        setting does.
+
+    .. versionadded:: 8.0
+    """
+
+    antiloop_window = ValidatedAttribute('antiloop_window', int, default=120)
+    """The time period (in seconds) checked when detecting repeated messages.
+
+    :default: ``120``
+
+    This is equivalent to the default value:
+
+    .. code-block:: ini
+
+        antiloop_window = 120
+
+    .. seealso::
+
+        The :ref:`Loop Prevention` chapter to learn what each antiloop-related
+        setting does.
+
+    .. versionadded:: 8.0
+    """
+
     auth_method = ChoiceAttribute('auth_method', choices=[
         'nickserv', 'authserv', 'Q', 'sasl', 'server', 'userserv'])
     """Simple method to authenticate with the server.
 
     Can be one of ``nickserv``, ``authserv``, ``Q``, ``sasl``, ``server``, or
     ``userserv``.
 
@@ -174,15 +249,17 @@
     :default:
         * ``NickServ`` if using the ``nickserv`` :attr:`auth_method`
         * ``UserServ`` if using the ``userserv`` :attr:`auth_method`
         * ``PLAIN`` if using the ``sasl`` :attr:`auth_method`
 
     The nickname of the NickServ or UserServ service, or the name of the
     desired SASL mechanism, if :attr:`auth_method` is set to one of these
-    methods. This value is otherwise ignored.
+    methods. For SASL, the ``EXTERNAL`` option is available in case the IRC
+    network requires it (e.g. for CertFP using :attr:`client_cert_file`). This
+    value is otherwise ignored.
 
     See :ref:`Authentication`.
     """
 
     auth_username = ValidatedAttribute('auth_username')
     """The user/account name to use when authenticating.
 
@@ -224,25 +301,24 @@
 
     .. code-block:: ini
 
         bind_host = 0.0.0.0
 
     """
 
-    ca_certs = FilenameAttribute('ca_certs', default=_find_certs())
-    """The path to the CA certs ``.pem`` file.
+    ca_certs = FilenameAttribute('ca_certs')
+    """The path to the CA certs ``PEM`` file.
 
     Example:
 
     .. code-block:: ini
 
         ca_certs = /etc/ssl/certs/ca-certificates.crt
 
-    If not specified, Sopel will try to find the certificate trust store
-    itself from a set of known locations.
+    If not specified, the system default will be used.
 
     If the given value is not an absolute path, it will be interpreted relative
     to the directory containing the config file with which Sopel was started.
     """
 
     channels = ListAttribute('channels')
     """List of channels for the bot to join when it connects.
@@ -263,14 +339,26 @@
         If you edit the config file manually, make sure to wrap each line
         starting with a ``#`` in double quotes, as shown in the example above.
         An unquoted ``#`` denotes a comment, which will be ignored by Sopel's
         configuration parser.
 
     """
 
+    client_cert_file = FilenameAttribute('client_cert_file')
+    """Filesystem path to a certificate file for CertFP.
+
+    This is expected to be a ``.pem`` file containing both the certificate and
+    private key. Most networks that support CertFP will give instructions for
+    generating this, typically using OpenSSL.
+
+    Some networks may refer to this authentication method as SASL EXTERNAL.
+
+    .. versionadded:: 8.0
+    """
+
     commands_on_connect = ListAttribute('commands_on_connect')
     """A list of commands to send upon successful connection to the IRC server.
 
     Each line is a message that will be sent to the server once connected,
     in the order they are defined:
 
     .. code-block:: ini
@@ -373,33 +461,50 @@
     .. note::
 
         Plugins originally written for Sopel 6.x and older *might* not work
         correctly with ``db_type``\\s other than ``sqlite``.
 
     """
 
+    db_url = ValidatedAttribute('db_url')
+    """A raw database URL.
+
+    If this option is present, Sopel will ignore **all** other ``db_*``
+    settings and use this option's value only.
+
+    .. note::
+
+        Specifying this option via the ``SOPEL_CORE_DB_URL`` :ref:`environment
+        variable <Overriding individual settings>` may prove especially useful
+        in certain cloud environments, avoiding the need to split a database
+        URI provided by the platform at runtime into its components with a
+        startup script.
+
+    .. versionadded:: 8.0
+    """
+
     db_user = ValidatedAttribute('db_user')
     """The user for Sopel's database.
 
     Ignored when using SQLite.
     """
 
     default_time_format = ValidatedAttribute('default_time_format',
-                                             default='%Y-%m-%d - %T%Z')
+                                             default='%Y-%m-%d - %T %Z')
     """The default format to use for time in messages.
 
-    :default: ``%Y-%m-%d - %T%Z``
+    :default: ``%Y-%m-%d - %T %Z``
 
     Used when plugins format times with :func:`sopel.tools.time.format_time`.
 
     This is equivalent to the default value:
 
     .. code-block:: ini
 
-        default_time_format = %Y-%m-%d - %T%Z
+        default_time_format = %Y-%m-%d - %T %Z
 
     .. seealso::
 
         Time format reference is available in the documentation for Python's
         :func:`time.strftime` function.
 
     """
@@ -531,18 +636,22 @@
         The :ref:`Flood Prevention` chapter to learn what each flood-related
         setting does.
 
     .. versionadded:: 7.0
     """
 
     flood_max_wait = ValidatedAttribute('flood_max_wait', float, default=2)
-    """How much time to wait at most when flood protection kicks in.
+    """How many seconds to wait at most when flood protection kicks in.
 
     :default: ``2``
 
+    .. note::
+
+        If the maximum wait is 0, flood protection is effectively disabled.
+
     This is equivalent to the default value:
 
     .. code-block:: ini
 
         flood_max_wait = 2
 
     .. seealso::
@@ -643,16 +752,19 @@
     built-in ``help`` functionality will provide incorrect example usage.
     """
 
     @property
     def homedir(self):
         """The directory in which various files are stored at runtime.
 
-        By default, this is the same directory as the config file. It cannot be
-        changed at runtime.
+        Specifying the ``homedir`` option is useful for e.g. :doc:`running Sopel
+        as a system service </run/service>`.
+
+        If not set, the config file's parent directory will be used. This value
+        cannot be changed at runtime.
         """
         return self._parent.homedir
 
     host = ValidatedAttribute('host', default='irc.libera.chat')
     """The IRC server to connect to.
 
     :default: ``irc.libera.chat``
@@ -664,33 +776,35 @@
         host = irc.libera.chat
 
     """
 
     host_blocks = ListAttribute('host_blocks')
     """A list of hostnames which Sopel should ignore.
 
-    Messages from any user whose connection hostname matches one of these
-    values will be ignored. :ref:`Regular expression syntax <re-syntax>`
-    is supported, so remember to escape special characters:
+    Sopel will :ref:`ignore <Ignoring Users>` messages from any user whose
+    connection hostname matches one of these values.
+    :ref:`Regular expression syntax <re-syntax>` is supported, so remember to
+    escape special characters:
 
     .. code-block:: ini
 
         host_blocks =
             (.+\\.)*domain\\.com
 
     .. seealso::
 
         The :attr:`nick_blocks` list can be used to block users by their nick.
 
     .. note::
 
-        We are working on a better block system; see `issue #1355`__ for more
-        information and update.
+        :ref:`Plugin callables` with the :func:`.plugin.unblockable` decorator
+        run regardless of matching ``*_blocks`` entries.
 
-    .. __: https://github.com/sopel-irc/sopel/issues/1355
+        We are working toward a better block system; see :issue:`1355` for more
+        information and updates.
 
     """
 
     log_raw = BooleanAttribute('log_raw', default=False)
     """Whether a log of raw lines as sent and received should be kept.
 
     :default: ``no``
@@ -709,15 +823,15 @@
 
     logdir = FilenameAttribute('logdir', directory=True, default='logs')
     """Directory in which to place logs.
 
     :default: ``logs``
 
     If the given value is not an absolute path, it will be interpreted relative
-    to the directory containing the config file with which Sopel was started.
+    to the :attr:`homedir` of the config file with which Sopel was started.
 
     .. seealso::
 
         The :ref:`Logging` chapter.
 
     """
 
@@ -755,25 +869,29 @@
         The :ref:`Log to a Channel` chapter.
 
     .. versionadded:: 7.0
     """
 
     logging_channel_level = ChoiceAttribute('logging_channel_level',
                                             ['CRITICAL', 'ERROR', 'WARNING',
-                                             'INFO', 'DEBUG'],
+                                             'INFO'],
                                             'WARNING')
     """The lowest severity of logs to display in IRC channel logs.
 
-    If not specified, this falls back to using :attr:`logging_level`.
-
     .. seealso::
 
         The :ref:`Log to a Channel` chapter.
 
     .. versionadded:: 7.0
+    .. versionchanged:: 8.0
+
+        No longer uses the value of :attr:`logging_level` if not set. Removed
+        ``DEBUG`` from the available choices; setting it caused the bot to get
+        caught in an ever-increasing flood prevention loop.
+
     """
 
     logging_datefmt = ValidatedAttribute('logging_datefmt')
     """The format string to use for timestamps in logs.
 
     If not set, the ``datefmt`` argument is not provided, and :mod:`logging`
     will use the Python default.
@@ -832,30 +950,36 @@
 
     .. code-block:: ini
 
         logging_level = WARNING
 
     """
 
-    modes = ValidatedAttribute('modes', default='B')
+    modes = ValidatedAttribute('modes')
     """User modes to be set on connection.
 
-    :default: ``B``
-
     Include only the mode letters; this value is automatically prefixed with
     ``+`` before Sopel sends the MODE command to IRC.
+
+    .. versionchanged:: 8.0.0
+
+        Now empty by default. Previous default was ``B``, which has been
+        dropped in favor of the formal `bot mode specification`__.
+
+        .. __: https://ircv3.net/specs/extensions/bot-mode
+
     """
 
     name = ValidatedAttribute('name', default='Sopel: https://sopel.chat/')
     """The "real name" of your bot for ``WHOIS`` responses.
 
     :default: ``Sopel: https://sopel.chat/``
     """
 
-    nick = ValidatedAttribute('nick', Identifier, default=Identifier('Sopel'))
+    nick = ValidatedAttribute('nick', default='Sopel')
     """The nickname for the bot.
 
     :default: ``Sopel``
 
     **Required**:
 
     .. code-block:: ini
@@ -915,34 +1039,36 @@
 
     .. versionadded:: 7.0
     """
 
     nick_blocks = ListAttribute('nick_blocks')
     """A list of nicks which Sopel should ignore.
 
-    Messages from any user whose nickname matches one of these values will be
-    ignored. :ref:`Regular expression syntax <re-syntax>` is supported, so
-    remember to escape special characters:
+    Sopel will :ref:`ignore <Ignoring Users>` messages from any user whose
+    nickname matches one of these values.
+    :ref:`Regular expression syntax <re-syntax>` is supported, so remember to
+    escape special characters:
 
     .. code-block:: ini
 
         nick_blocks =
             ExactNick
             _*RegexMatch_*
 
     .. seealso::
 
         The :attr:`host_blocks` list can be used to block users by their host.
 
     .. note::
 
-        We are working on a better block system; see `issue #1355`__ for more
-        information and update.
+        :ref:`Plugin callables` with the :func:`.plugin.unblockable` decorator
+        run regardless of matching ``*_blocks`` entries.
 
-    .. __: https://github.com/sopel-irc/sopel/issues/1355
+        We are working toward a better block system; see :issue:`1355` for more
+        information and updates.
 
     """
 
     not_configured = BooleanAttribute('not_configured', default=False)
     """For package maintainers. Not used in normal configurations.
 
     :default: ``False``
@@ -973,29 +1099,29 @@
     If the given value is not an absolute path, it will be interpreted relative
     to the directory containing the config file with which Sopel was started.
 
     You probably do not need to change this unless you're managing Sopel with
     ``systemd`` or similar.
     """
 
-    port = ValidatedAttribute('port', int, default=6667)
+    port = ValidatedAttribute('port', int, default=6697)
     """The port to connect on.
 
-    :default: ``6667`` normally; ``6697`` if :attr:`use_ssl` is ``True``
+    :default: ``6697``
 
     .. highlight:: ini
 
     **Required**::
 
-        port = 6667
+        port = 6697
 
-    And usually when SSL is enabled::
+    Or if SSL is disabled::
 
-        port = 6697
-        use_ssl = yes
+        port = 6667
+        use_ssl = false
 
     """
 
     prefix = ValidatedAttribute('prefix', default=COMMAND_DEFAULT_PREFIX)
     """The prefix to add to the beginning of commands as a regular expression.
 
     :default: ``\\.``
@@ -1068,15 +1194,20 @@
     """
 
     server_auth_sasl_mech = ValidatedAttribute('server_auth_sasl_mech')
     """The SASL mechanism.
 
     :default: ``PLAIN``
 
+    ``EXTERNAL`` is also supported, e.g. for using :attr:`client_cert_file` to
+    authenticate via CertFP.
+
     .. versionadded:: 7.0
+    .. versionchanged:: 8.0
+        Added support for SASL EXTERNAL mechanism.
     """
 
     server_auth_username = ValidatedAttribute('server_auth_username')
     """The username/account to use to authenticate with the server.
 
     .. versionadded:: 7.0
     """
@@ -1175,24 +1306,93 @@
             ping_interval = timeout * 0.45
 
         So for a timeout of 120s it's a PING every 54s. For a timeout of 250s
         it's a PING every 112.5s.
 
     """
 
-    use_ssl = BooleanAttribute('use_ssl', default=False)
+    ssl_ciphers = ListAttribute(
+        'ssl_ciphers',
+        default=[
+            "ECDHE-ECDSA-AES128-GCM-SHA256",
+            "ECDHE-RSA-AES128-GCM-SHA256",
+            "ECDHE-ECDSA-AES256-GCM-SHA384",
+            "ECDHE-RSA-AES256-GCM-SHA384",
+            "ECDHE-ECDSA-CHACHA20-POLY1305",
+            "ECDHE-RSA-CHACHA20-POLY1305",
+            "DHE-RSA-AES128-GCM-SHA256",
+            "DHE-RSA-AES256-GCM-SHA384",
+        ],
+    )
+    """The cipher suites enabled for SSL/TLS connections.
+
+    :default: ``ECDHE-ECDSA-AES128-GCM-SHA256
+                ECDHE-RSA-AES128-GCM-SHA256
+                ECDHE-ECDSA-AES256-GCM-SHA384
+                ECDHE-RSA-AES256-GCM-SHA384
+                ECDHE-ECDSA-CHACHA20-POLY1305
+                ECDHE-RSA-CHACHA20-POLY1305
+                DHE-RSA-AES128-GCM-SHA256
+                DHE-RSA-AES256-GCM-SHA384``
+
+    The default is the `Mozilla Intermediate configuration`__ as of February
+    2022. This parameter is in OpenSSL format; see the `ciphers manual page`__
+    for your version. This setting cannot be used to configure TLS 1.3.
+
+    .. __: https://wiki.mozilla.org/Security/Server_Side_TLS
+    .. __: https://www.openssl.org/docs/manmaster/man1/ciphers.html
+
+    .. code-block:: ini
+
+        ssl_ciphers =
+            ECDSA+AES256
+            !SHA1
+
+    .. note::
+
+        Cipher selection is also subject to the available SSL/TLS versions;
+        see :attr:`ssl_minimum_version`.
+
+    """
+
+    ssl_minimum_version = ValidatedAttribute(
+        'ssl_minimum_version',
+        default=TLSVersion.TLSv1_2,
+        parse=_parse_ssl_version,
+        serialize=lambda ver: ver.name,
+    )
+    """The minimum version allowed for SSL/TLS connections.
+
+    :default: ``TLSv1_2``
+
+    You should not set this lower than the default unless the server does not
+    support modern versions. Set this to a :class:`~ssl.TLSVersion` value,
+    e.g. ``TLSv1`` or ``TLSv1_3``.
+
+    .. code-block:: ini
+
+        ssl_minimum_version = TLSv1_3
+
+    .. note::
+
+        To use insecure SSL/TLS versions, you may also need to enable
+        insecure cipher suites. See :attr:`ssl_ciphers`.
+
+    """
+
+    use_ssl = BooleanAttribute('use_ssl', default=True)
     """Whether to use a SSL/TLS encrypted connection.
 
-    :default: ``False``
+    :default: ``True``
 
-    Example with SSL on:
+    Example with SSL off:
 
     .. code-block:: ini
 
-        use_ssl = yes
+        use_ssl = false
 
     """
 
     user = ValidatedAttribute('user', default='sopel')
     """The "user" for your bot (the part before the ``@`` in the hostname).
 
     :default: ``sopel``
@@ -1210,11 +1410,11 @@
 
     :default: ``True``
 
     Example with SSL on:
 
     .. code-block:: ini
 
-        use_ssl = yes
-        verify_ssl = yes
+        use_ssl = true
+        verify_ssl = true
 
     """
```

### Comparing `sopel-7.1.9/sopel/config/types.py` & `sopel-8.0.0/sopel/config/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 """Types for creating section definitions.
 
 A section definition consists of a subclass of :class:`StaticSection`, on which
 any number of subclasses of :class:`BaseValidated` (a few common ones of which
 are available in this module) are assigned as attributes. These descriptors
 define how to read values from, and write values to, the config file.
 
@@ -20,33 +19,33 @@
     ['goose', 'turkey', 'duck', 'chicken', 'quail']
     >>> config.spam.eggs = 'herring'
     Traceback (most recent call last):
         ...
     ValueError: ListAttribute value must be a list.
 """
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+import abc
 import getpass
+import logging
 import os.path
 import re
-import sys
 
-from sopel.tools import deprecated, get_input
+from sopel.lifecycle import deprecated
 
-if sys.version_info.major >= 3:
-    unicode = str
-    basestring = (str, bytes)
 
+LOGGER = logging.getLogger(__name__)
 
-class NO_DEFAULT(object):
+
+class NO_DEFAULT:
     """A special value to indicate that there should be no default."""
 
 
-class StaticSection(object):
+class StaticSection:
     """A configuration section with parsed and validated settings.
 
     This class is intended to be subclassed and customized with added
     attributes containing :class:`BaseValidated`-based objects.
 
     .. note::
 
@@ -97,16 +96,18 @@
         default value if it's unset, will be used. Note that if ``default`` is
         passed, the current value of the setting will be ignored, even if it is
         not the attribute's default.
         """
         attribute = getattr(self.__class__, name)
         if default is NO_DEFAULT and not attribute.is_secret:
             try:
+                # get current value of this setting to use as prompt default
                 default = getattr(self, name)
             except AttributeError:
+                # there is no current value; that's OK
                 pass
             except ValueError:
                 print('The configured value for this option was invalid.')
                 if attribute.default is not NO_DEFAULT:
                     default = attribute.default
         while True:
             try:
@@ -115,18 +116,15 @@
             except ValueError as exc:
                 print(exc)
             else:
                 break
         setattr(self, name, value)
 
 
-# TODO: Make this a proper abstract class when dropping Python 2 support.
-# Abstract classes are much simpler to deal with once we only need to worry
-# about Python 3.4 or newer. (https://stackoverflow.com/a/13646263/5991)
-class BaseValidated(object):
+class BaseValidated(abc.ABC):
     """The base type for a setting descriptor in a :class:`StaticSection`.
 
     :param str name: the attribute name to use in the config file
     :param default: the value to be returned if the setting has no value
                     (optional; defaults to :obj:`None`)
     :type default: mixed
     :param bool is_secret: tell if the attribute is secret/a password
@@ -137,23 +135,23 @@
     default value). Trying to read an empty ``NO_DEFAULT`` value will raise
     :class:`AttributeError`.
 
     .. important::
 
         Setting names SHOULD follow *snake_case* naming rules:
 
-          * use only lowercase letters, digits, and underscore (``_``)
-          * SHOULD NOT start with a digit
+        * use only lowercase letters, digits, and underscore (``_``)
+        * SHOULD NOT start with a digit
 
         Deviations from *snake_case* can break the following operations:
 
-          * :ref:`accessing the setting <sopel.config>` from Python code using
-            the :class:`~.Config` object's attributes
-          * :ref:`overriding the setting's value <Overriding individual
-            settings>` using environment variables
+        * :ref:`accessing the setting <sopel.config>` from Python code using
+          the :class:`~.Config` object's attributes
+        * :ref:`overriding the setting's value <Overriding individual
+          settings>` using environment variables
 
     """
     def __init__(self, name, default=None, is_secret=False):
         self.name = name
         """Name of the attribute."""
         self.default = default
         """Default value for this attribute.
@@ -188,36 +186,31 @@
         """
         if default is not NO_DEFAULT and default is not None:
             prompt = '{} [{}]'.format(prompt, default)
 
         if self.is_secret:
             value = getpass.getpass(prompt + ' (hidden input) ')
         else:
-            value = get_input(prompt + ' ')
+            value = input(prompt + ' ')
 
         if not value and default is NO_DEFAULT:
             raise ValueError("You must provide a value for this option.")
 
         value = value or default
         section = getattr(parent, section_name)
 
         return self._parse(value, parent, section)
 
+    @abc.abstractmethod
     def serialize(self, value, *args, **kwargs):
-        """Take some object, and return the string to be saved to the file.
-
-        Must be implemented in subclasses.
-        """
-        raise NotImplementedError("Serialize method must be implemented in subclass")
+        """Take some object, and return the string to be saved to the file."""
 
+    @abc.abstractmethod
     def parse(self, value, *args, **kwargs):
-        """Take a string from the file, and return the appropriate object.
-
-        Must be implemented in subclasses."""
-        raise NotImplementedError("Parse method must be implemented in subclass")
+        """Take a string from the file, and return the appropriate object."""
 
     def __get__(self, instance, owner=None):
         if instance is None:
             # If instance is None, we're getting from a section class, not an
             # instance of a section class. It makes the wizard code simpler
             # (and is really just more intuitive) to return the descriptor
             # instance here.
@@ -263,15 +256,15 @@
     def __delete__(self, instance):
         instance._parser.remove_option(instance._section_name, self.name)
 
 
 def _parse_boolean(value):
     if value is True or value == 1:
         return value
-    if isinstance(value, basestring):
+    if isinstance(value, str):
         return value.lower() in ['1', 'yes', 'y', 'true', 'on']
     return bool(value)
 
 
 def _serialize_boolean(value):
     return 'true' if _parse_boolean(value) else 'false'
 
@@ -307,58 +300,58 @@
     """
     def __init__(self,
                  name,
                  parse=None,
                  serialize=None,
                  default=None,
                  is_secret=False):
-        super(ValidatedAttribute, self).__init__(
-            name, default=default, is_secret=is_secret)
+        super().__init__(name, default=default, is_secret=is_secret)
 
         if parse == bool:
             parse, serialize = _deprecated_special_bool_handling(serialize)
 
-        self.parse = parse or self.parse
-        self.serialize = serialize or self.serialize
+        # ignore typing errors on these monkeypatches for now
+        # TODO: more dedicated subtypes; deprecate `parse`/`serialize` args
+        self.parse = parse or self.parse  # type: ignore
+        self.serialize = serialize or self.serialize  # type: ignore
 
     def serialize(self, value):
         """Return the ``value`` as a Unicode string.
 
         :param value: the option value
         :rtype: str
         """
-        return unicode(value)
+        return str(value)
 
     def parse(self, value):
         """No-op: simply returns the given ``value``, unchanged.
 
         :param str value: the string read from the config file
         :rtype: str
         """
         return value
 
     def configure(self, prompt, default, parent, section_name):
         if self.parse == _parse_boolean:
             prompt += ' (y/n)'
             default = 'y' if default else 'n'
-        return super(ValidatedAttribute, self).configure(prompt, default, parent, section_name)
+        return super().configure(prompt, default, parent, section_name)
 
 
 class BooleanAttribute(BaseValidated):
     """A descriptor for Boolean settings in a :class:`StaticSection`.
 
     :param str name: the attribute name to use in the config file
     :param bool default: the default value to use if this setting is not
                          present in the config file
 
     If the ``default`` value is not specified, it will be ``False``.
     """
     def __init__(self, name, default=False):
-        super(BooleanAttribute, self).__init__(
-            name, default=default, is_secret=False)
+        super().__init__(name, default=default, is_secret=False)
 
     def configure(self, prompt, default, parent, section_name):
         """Parse and return a value from user's input.
 
         :param str prompt: text to show the user
         :param bool default: default value used if no input given
         :param parent: usually the parent Config object
@@ -366,15 +359,15 @@
         :param str section_name: the name of the containing section
 
         This method displays the ``prompt`` and waits for user's input on the
         terminal. If no input is provided (i.e. the user just presses "Enter"),
         the ``default`` value is returned instead.
         """
         prompt = '{} ({})'.format(prompt, 'Y/n' if default else 'y/N')
-        value = get_input(prompt + ' ') or default
+        value = input(prompt + ' ') or default
         section = getattr(parent, section_name)
         return self._parse(value, parent, section)
 
     def serialize(self, value):
         """Convert a Boolean value to a string for saving to the config file.
 
         :param bool value: the value to serialize
@@ -389,15 +382,15 @@
         The literal values ``True`` or ``1`` will be parsed as ``True``. The
         strings ``'1'``, ``'yes'``, ``'y'``, ``'true'``, ``'enable'``,
         ``'enabled'``, and ``'on'`` will also be parsed as ``True``,
         regardless of case. All other values will be parsed as ``False``.
         """
         if value is True or value == 1:
             return True
-        if isinstance(value, basestring):
+        if isinstance(value, str):
             return value.lower() in [
                 '1',
                 'enable',
                 'enabled',
                 'on',
                 'true',
                 'y',
@@ -419,30 +412,30 @@
 class SecretAttribute(ValidatedAttribute):
     """A config attribute containing a value which must be kept secret.
 
     This attribute is always considered to be secret/sensitive data, but
     otherwise behaves like other any option.
     """
     def __init__(self, name, parse=None, serialize=None, default=None):
-        super(SecretAttribute, self).__init__(
+        super().__init__(
             name,
             parse=parse,
             serialize=serialize,
             default=default,
             is_secret=True,
         )
 
 
 class ListAttribute(BaseValidated):
     """A config attribute containing a list of string values.
 
     :param str name: the attribute name to use in the config file
     :param strip: whether to strip whitespace from around each value
-                  (optional; applies only to legacy comma-separated lists;
-                  multi-line lists are always stripped)
+                  (optional, deprecated; applies only to legacy comma-separated
+                  lists; multi-line lists are always stripped)
     :type strip: bool
     :param default: the default value if the config file does not define a
                     value for this option; to require explicit configuration,
                     use :const:`sopel.config.types.NO_DEFAULT` (optional)
     :type default: list
 
     From this :class:`StaticSection`::
@@ -478,38 +471,40 @@
 
         See the :meth:`parse` method for more information.
 
     .. note::
 
         **About:** backward compatibility with comma-separated values.
 
-        A :class:`ListAttribute` option allows to write, on a single line,
-        the values separated by commas. As of Sopel 7.x this behavior is
-        discouraged. It will be deprecated in Sopel 8.x, then removed in
-        Sopel 9.x.
+        A :class:`ListAttribute` option used to allow to write, on a single
+        line, the values separated by commas. It is still technically possible
+        while raising a deprecation warning.
+
+        In Sopel 7.x this behavior was discouraged; as of Sopel 8.x it is now
+        deprecated with warnings, and it will be removed in Sopel 9.x.
 
-        Bot owners are encouraged to update their configurations to use
-        newlines instead of commas.
+        Bot owners should update their configurations to use newlines instead
+        of commas.
 
         The comma delimiter fallback does not support commas within items in
         the list.
     """
-    DELIMITER = ','
+    DELIMITER = ','  # Deprecated, will be removed in Sopel 9
     QUOTE_REGEX = re.compile(r'^"(?P<value>#.*)"$')
     """Regex pattern to match value that requires quotation marks.
 
     This pattern matches values that start with ``#`` inside quotation marks
     only: ``"#sopel"`` will match, but ``"sopel"`` won't, and neither will any
     variant that doesn't conform to this pattern.
     """
 
     def __init__(self, name, strip=True, default=None):
         default = default or []
-        super(ListAttribute, self).__init__(name, default=default)
-        self.strip = strip
+        super().__init__(name, default=default)
+        self.strip = strip  # Warn in Sopel 9.x and remove in Sopel 10.x
 
     def parse(self, value):
         """Parse ``value`` into a list.
 
         :param str value: a multi-line string of values to parse into a list
         :return: a list of items from ``value``
         :rtype: list
@@ -517,27 +512,40 @@
         .. versionchanged:: 7.0
 
             The value is now split on newlines, with fallback to comma
             when there is no newline in ``value``.
 
             When modified and saved to a file, items will be stored as a
             multi-line string (see :meth:`serialize`).
+
+        .. versionchanged:: 8.0
+
+            When the value contains a delimiter without newline, it warns the
+            user to switch to a multi-line value, without a delimiter.
+
         """
         if "\n" in value:
             items = (
                 # remove trailing comma
                 # because `value,\nother` is valid in Sopel 7.x
                 item.strip(self.DELIMITER).strip()
                 for item in value.splitlines())
         else:
-            # this behavior will be:
-            # - Discouraged in Sopel 7.x (in the documentation)
-            # - Deprecated in Sopel 8.x
-            # - Removed from Sopel 9.x
+            # this behavior was discouraged in Sopel 7.x (in the documentation)
+            # this behavior is now deprecated in Sopel 8.x
+            # this behavior will be removed from Sopel 9.x
             items = value.split(self.DELIMITER)
+            if self.DELIMITER in value:
+                # trigger for "one, two" and "first line,"
+                # a single line without the delimiter is fine
+                LOGGER.warning(
+                    'Using "%s" as item delimiter in option "%s" '
+                    'is deprecated and will be removed in Sopel 9; '
+                    'use multi-line instead',
+                    self.DELIMITER, self.name)
 
         items = (self.parse_item(item) for item in items if item)
         if self.strip:
             return [item.strip() for item in items]
 
         return list(items)
 
@@ -595,24 +603,24 @@
 
         if default is not NO_DEFAULT:
             default_prompt = ','.join(['"{}"'.format(item) for item in default])
             prompt = '{} [{}]'.format(prompt, default_prompt)
         else:
             default = []
         print(prompt)
-        values = []
-        value = get_input(each_prompt + ' ') or default
+        values: list[str] = []
+        value = input(each_prompt + ' ') or default
         if (value == default) and not default:
             value = ''
         while value:
             if value == default:
                 values.extend(value)
             else:
                 values.append(value)
-            value = get_input(each_prompt + ' ')
+            value = input(each_prompt + ' ')
 
         section = getattr(parent, section_name)
         values = self._serialize(values, parent, section)
         return self._parse(values, parent, section)
 
 
 class ChoiceAttribute(BaseValidated):
@@ -623,15 +631,15 @@
     :type choices: list or tuple
     :param default: which choice to use if none is set in the config file; to
                     require explicit configuration, use
                     :const:`sopel.config.types.NO_DEFAULT` (optional)
     :type default: str
     """
     def __init__(self, name, choices, default=None):
-        super(ChoiceAttribute, self).__init__(name, default=default)
+        super().__init__(name, default=default)
         self.choices = choices
 
     def parse(self, value):
         """Check the loaded ``value`` against the valid ``choices``.
 
         :param str value: the value loaded from the config file
         :return: the ``value``, if it is valid
@@ -670,15 +678,15 @@
     :type directory: bool
     :param default: the value to use if none is defined in the config file; to
                     require explicit configuration, use
                     :const:`sopel.config.types.NO_DEFAULT` (optional)
     :type default: str
     """
     def __init__(self, name, relative=True, directory=False, default=None):
-        super(FilenameAttribute, self).__init__(name, default=default)
+        super().__init__(name, default=default)
         self.relative = relative
         self.directory = directory
 
     def _parse(self, value, settings, section):
         if value is None:
             if self.default == NO_DEFAULT:
                 raise AttributeError(
@@ -687,14 +695,19 @@
                     )
                 )
             value = self.default
 
         if not value:
             return self.parse(value)
 
+        if value.startswith('"') and value.endswith('"'):
+            value = value.strip('"')
+        elif value.startswith("'") and value.endswith("'"):
+            value = value.strip("'")
+
         result = os.path.expanduser(value)
         if not os.path.isabs(result):
             if not self.relative:
                 raise ValueError("Value must be an absolute path.")
             result = os.path.join(settings.homedir, result)
 
         return self.parse(result)
@@ -732,15 +745,16 @@
             try:
                 os.makedirs(value)
             except (IOError, OSError):
                 raise ValueError(
                     "Value must be an existing or creatable directory.")
         if not self.directory and not os.path.isfile(value):
             try:
-                open(value, 'w').close()
+                with open(value, 'w') as f:
+                    f.close()
             except (IOError, OSError):
                 raise ValueError("Value must be an existing or creatable file.")
         return value
 
     def serialize(self, value):
         """Directly return the ``value`` without modification.
```

### Comparing `sopel-7.1.9/sopel/coretasks.py` & `sopel-8.0.0/sopel/coretasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 """Core Sopel plugin that handles IRC protocol functions.
 
 This plugin allows the bot to run without user-facing functionality:
 
 * it handles client capability negotiation
 * it handles client auth (both nick auth and server auth)
 * it handles connection registration (RPL_WELCOME, RPL_LUSERCLIENT), dealing
@@ -17,71 +16,181 @@
 # Copyright 2008-2011, Sean B. Palmer (inamidst.com) and Michael Yanovich
 # (yanovich.net)
 # Copyright © 2012, Elad Alfassa <elad@fedoraproject.org>
 # Copyright 2012-2015, Elsie Powell embolalia.com
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import base64
 import collections
-import datetime
+import copy
+from datetime import datetime, timedelta, timezone
 import functools
 import logging
 import re
-import sys
 import time
+from typing import Callable, Optional, TYPE_CHECKING
 
-from sopel import loader, module, plugin
-from sopel.config import ConfigurationError
-from sopel.irc import isupport
-from sopel.irc.utils import CapReq, MyInfo
-from sopel.tools import events, Identifier, iteritems, SopelMemory, target, web
+from sopel import config, plugin
+from sopel.irc import isupport, utils
+from sopel.tools import events, jobs, SopelMemory, target
+
+if TYPE_CHECKING:
+    from sopel.bot import Sopel, SopelWrapper
+    from sopel.tools import Identifier
+    from sopel.trigger import Trigger
 
 
-if sys.version_info.major >= 3:
-    unicode = str
-
 LOGGER = logging.getLogger(__name__)
 
-CORE_QUERYTYPE = '999'
+WHOX_QUERY = '%nuachrtf'
+"""List of WHOX flags coretasks requests."""
+WHOX_QUERYTYPE = '999'
 """WHOX querytype to indicate requests/responses from coretasks.
 
 Other plugins should use a different querytype.
 """
 
-batched_caps = {}
+MODE_PREFIX_PRIVILEGES = {
+    "v": plugin.VOICE,
+    "h": plugin.HALFOP,
+    "o": plugin.OP,
+    "a": plugin.ADMIN,
+    "q": plugin.OWNER,
+    "y": plugin.OPER,
+    "Y": plugin.OPER,
+}
+
+
+def _handle_account_and_extjoin_capabilities(
+    cap_req: tuple[str, ...], bot: SopelWrapper, acknowledged: bool,
+) -> plugin.CapabilityNegotiation:
+    if acknowledged:
+        return plugin.CapabilityNegotiation.DONE
+
+    name = ', '.join(cap_req)
+    owner_account = bot.settings.core.owner_account
+    admin_accounts = bot.settings.core.admin_accounts
+
+    LOGGER.info(
+        'Server does not support "%s". '
+        'User account validation unavailable or limited.',
+        name,
+    )
+    if owner_account or admin_accounts:
+        LOGGER.warning(
+            'Owner or admin accounts are configured, but "%s" is not '
+            'supported by the server. This may cause unexpected behavior.',
+            name,
+        )
+
+    return plugin.CapabilityNegotiation.DONE
+
+
+def _handle_sasl_capability(
+    cap_req: tuple[str, ...], bot: SopelWrapper, acknowledged: bool,
+) -> plugin.CapabilityNegotiation:
+    # Manage CAP REQ :sasl
+    auth_method = bot.settings.core.auth_method
+    server_auth_method = bot.settings.core.server_auth_method
+    is_required = 'sasl' in (auth_method, server_auth_method)
+
+    if not is_required:
+        # not required: we are fine, available or not
+        return plugin.CapabilityNegotiation.DONE
+    elif not acknowledged:
+        # required but not available: error, we must stop here
+        LOGGER.error(
+            'SASL capability is not enabled; '
+            'cannot authenticate with SASL.',
+        )
+        return plugin.CapabilityNegotiation.ERROR
+
+    # Check SASL configuration (password is required for PLAIN/SCRAM)
+    password, mech = _get_sasl_pass_and_mech(bot)
+    if mech != "EXTERNAL" and not password:
+        raise config.ConfigurationError(
+            'SASL authentication required but no password available; '
+            'please check your configuration file.',
+        )
 
+    cap_info = bot.capabilities.get_capability_info('sasl')
+    cap_params = cap_info.params
 
-def setup(bot):
+    available_mechs = cap_params.split(',') if cap_params else []
+
+    if available_mechs and mech not in available_mechs:
+        # Raise an error if configured to use an unsupported SASL mechanism,
+        # but only if the server actually advertised supported mechanisms,
+        # i.e. this network supports SASL 3.2
+
+        # SASL 3.1 failure is handled (when possible)
+        # by the sasl_mechs() function
+
+        # See https://github.com/sopel-irc/sopel/issues/1780 for background
+        raise config.ConfigurationError(
+            'SASL mechanism "{mech}" is not advertised by this server; '
+            'available mechanisms are: {available}.'.format(
+                mech=mech,
+                available=', '.join(available_mechs),
+            )
+        )
+
+    bot.write(('AUTHENTICATE', mech))
+
+    # If we want to do SASL, we have to wait before we can send CAP END. So if
+    # we are, wait on 903 (SASL successful) to send it.
+    return plugin.CapabilityNegotiation.CONTINUE
+
+
+CAP_ECHO_MESSAGE = plugin.capability('echo-message')
+CAP_MULTI_PREFIX = plugin.capability('multi-prefix')
+CAP_AWAY_NOTIFY = plugin.capability('away-notify')
+CAP_CHGHOST = plugin.capability('chghost')
+CAP_CAP_NOTIFY = plugin.capability('cap-notify')
+CAP_SERVER_TIME = plugin.capability('server-time')
+CAP_USERHOST_IN_NAMES = plugin.capability('userhost-in-names')
+CAP_MESSAGE_TAGS = plugin.capability('message-tags')
+CAP_ACCOUNT_NOTIFY = plugin.capability(
+    'account-notify', handler=_handle_account_and_extjoin_capabilities)
+CAP_EXTENDED_JOIN = plugin.capability(
+    'extended-join', handler=_handle_account_and_extjoin_capabilities)
+CAP_ACCOUNT_TAG = plugin.capability(
+    'account-tag', handler=_handle_account_and_extjoin_capabilities)
+CAP_SASL = plugin.capability('sasl', handler=_handle_sasl_capability)
+
+
+def setup(bot: Sopel):
     """Set up the coretasks plugin.
 
     The setup phase is used to activate the throttle feature to prevent a flood
     of JOIN commands when there are too many channels to join.
     """
+    bot.memory['retry_join'] = SopelMemory()
     bot.memory['join_events_queue'] = collections.deque()
 
     # Manage JOIN flood protection
     if bot.settings.core.throttle_join:
         wait_interval = max(bot.settings.core.throttle_wait, 1)
-
-        @module.interval(wait_interval)
-        @plugin.label('throttle_join')
-        def processing_job(bot):
-            _join_event_processing(bot)
-
-        loader.clean_callable(processing_job, bot.settings)
-        processing_job.plugin_name = 'coretasks'
-
-        bot.register_jobs([processing_job])
+        job = jobs.Job(
+            [wait_interval],
+            plugin='coretasks',
+            label='throttle_join',
+            handler=_join_event_processing,
+            threaded=True,
+            doc=None,
+        )
+        bot.scheduler.register(job)
 
 
 def shutdown(bot):
     """Clean up coretasks-related values in the bot's memory."""
+    bot.memory['retry_join'] = SopelMemory()
     try:
         bot.memory['join_events_queue'].clear()
     except KeyError:
         pass
 
 
 def _join_event_processing(bot):
@@ -135,15 +244,15 @@
         auth_password = bot.config.core.nick_auth_password
         auth_target = bot.config.core.nick_auth_target
     else:
         return
 
     # nickserv-based auth method needs to check for current nick
     if auth_method == 'nickserv':
-        if bot.nick != bot.settings.core.nick:
+        if bot.nick != bot.make_identifier(bot.settings.core.nick):
             LOGGER.warning("Sending nickserv GHOST command.")
             bot.say(
                 'GHOST %s %s' % (bot.settings.core.nick, auth_password),
                 auth_target or 'NickServ')
         else:
             bot.say('IDENTIFY %s' % auth_password, auth_target or 'NickServ')
 
@@ -202,29 +311,29 @@
         trigger.nick,
         trigger.sender,
         trigger.args,
     )
     bot.change_current_nick(bot.nick + '_')
 
 
-@module.require_privmsg("This command only works as a private message.")
-@module.require_admin("This command requires admin privileges.")
-@module.commands('execute')
+@plugin.require_privmsg("This command only works as a private message.")
+@plugin.require_admin("This command requires admin privileges.")
+@plugin.commands('execute')
 def execute_perform(bot, trigger):
     """Execute commands specified to perform on IRC server connect.
 
     This allows a bot owner or admin to force the execution of commands
     that are automatically performed when the bot connects.
     """
     _execute_perform(bot)
 
 
-@module.event(events.RPL_WELCOME, events.RPL_LUSERCLIENT)
-@module.thread(False)
-@module.unblockable
+@plugin.event(events.RPL_WELCOME, events.RPL_LUSERCLIENT)
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def startup(bot, trigger):
     """Do tasks related to connecting to the network.
 
     ``001 RPL_WELCOME`` is from RFC2812 and is the first message that is sent
     after the connection has been registered on the network.
 
@@ -241,14 +350,19 @@
     3. join channels (or queue them to join later)
     4. check for security when the ``account-tag`` capability is enabled
     5. execute custom commands
     """
     if bot.connection_registered:
         return
 
+    LOGGER.info(
+        'Enabled client capabilities: %s',
+        ', '.join(bot.capabilities.enabled),
+    )
+
     # nick shenanigans are serious business, but fortunately RPL_WELCOME
     # includes the actual nick used by the server after truncation, removal
     # of invalid characters, etc. so we can check for such shenanigans
     if trigger.event == events.RPL_WELCOME:
         if bot.nick != trigger.args[0]:
             # setting modes below is just one of the things that won't work
             # as expected if the conditions for running this block are met
@@ -265,140 +379,187 @@
                 "cause unexpected behavior. Please modify the configuration "
                 "and restart the bot." % (bot.nick, trigger.args[0])
             )
             LOGGER.critical(debug_msg)
             bot.say(privmsg, bot.config.core.owner)
 
     # set flag
-    bot.connection_registered = True
+    bot._connection_registered.set()
 
     # handle auth method
     auth_after_register(bot)
 
     # set bot's MODE
     modes = bot.config.core.modes
     if modes:
         if not modes.startswith(('+', '-')):
             # Assume "+" by default.
             modes = '+' + modes
         bot.write(('MODE', bot.nick, modes))
 
-    # join channels
-    bot.memory['retry_join'] = SopelMemory()
-
-    channels = bot.config.core.channels
-    if not channels:
-        LOGGER.info("No initial channels to JOIN.")
-    elif bot.config.core.throttle_join:
-        throttle_rate = int(bot.config.core.throttle_join)
-        throttle_wait = max(bot.config.core.throttle_wait, 1)
-        channels_joined = 0
-
-        LOGGER.info(
-            "Joining %d channels (with JOIN throttle ON); "
-            "this may take a moment.",
-            len(channels))
-
-        for channel in channels:
-            channels_joined += 1
-            if not channels_joined % throttle_rate:
-                LOGGER.debug(
-                    "Waiting %ds before next JOIN batch.",
-                    throttle_wait)
-                time.sleep(throttle_wait)
-            bot.join(channel)
-    else:
-        LOGGER.info(
-            "Joining %d channels (with JOIN throttle OFF); "
-            "this may take a moment.",
-            len(channels))
-
-        for channel in bot.config.core.channels:
-            bot.join(channel)
-
     # warn for insecure auth method if necessary
-    if (not bot.config.core.owner_account and
-            'account-tag' in bot.enabled_capabilities and
-            '@' not in bot.config.core.owner):
+    if (
+        not bot.config.core.owner_account and
+        bot.capabilities.is_enabled('account-tag') and
+        '@' not in bot.config.core.owner
+    ):
         msg = (
             "This network supports using network services to identify you as "
             "my owner, rather than just matching your nickname. This is much "
             "more secure. If you'd like to do this, make sure you're logged in "
             "and reply with \"{}useserviceauth\""
         ).format(bot.config.core.help_prefix)
         bot.say(msg, bot.config.core.owner)
 
     # execute custom commands
     _execute_perform(bot)
 
 
-@module.event(events.RPL_ISUPPORT)
-@module.thread(False)
-@module.unblockable
-@module.rule('are supported by this server')
+@plugin.event(events.RPL_ISUPPORT)
+@plugin.thread(False)
+@plugin.unblockable
+@plugin.rule('are supported by this server')
 @plugin.priority('medium')
 def handle_isupport(bot, trigger):
     """Handle ``RPL_ISUPPORT`` events."""
-    # remember if NAMESX is known to be supported, before parsing RPL_ISUPPORT
+    # remember if certain actionable tokens are known to be supported,
+    # before parsing RPL_ISUPPORT
+    botmode_support = 'BOT' in bot.isupport
     namesx_support = 'NAMESX' in bot.isupport
+    uhnames_support = 'UHNAMES' in bot.isupport
+    casemapping_support = 'CASEMAPPING' in bot.isupport
+    chantypes_support = 'CHANTYPES' in bot.isupport
 
     # parse ISUPPORT message from server
     parameters = {}
     for arg in trigger.args:
         try:
             key, value = isupport.parse_parameter(arg)
             parameters[key] = value
         except ValueError:
             # ignore malformed parameter: log a warning and continue
             LOGGER.warning("Unable to parse ISUPPORT parameter: %r", arg)
 
     bot._isupport = bot._isupport.apply(**parameters)
 
+    # update bot's mode parser
+    if 'CHANMODES' in bot.isupport:
+        bot.modeparser.chanmodes = bot.isupport.CHANMODES
+
+    if 'PREFIX' in bot.isupport:
+        bot.modeparser.privileges = set(bot.isupport.PREFIX.keys())
+
+    # rebuild nick when CASEMAPPING and/or CHANTYPES are set
+    if any((
+        # was CASEMAPPING support status updated?
+        not casemapping_support and 'CASEMAPPING' in bot.isupport,
+        # was CHANTYPES support status updated?
+        not chantypes_support and 'CHANTYPES' in bot.isupport,
+    )):
+        # these parameters change how the bot makes Identifiers
+        # since bot.nick is an Identifier, it must be rebuilt
+        bot.rebuild_nick()
+
+    # was BOT mode support status updated?
+    if not botmode_support and 'BOT' in bot.isupport:
+        # yes it was! set our mode unless the config overrides it
+        botmode = bot.isupport['BOT']
+        modes_setting = bot.config.core.modes
+
+        if not modes_setting or botmode not in bot.config.core.modes:
+            bot.write(('MODE', bot.nick, '+' + botmode))
+
     # was NAMESX support status updated?
     if not namesx_support and 'NAMESX' in bot.isupport:
         # yes it was!
-        if 'multi-prefix' not in bot.server_capabilities:
-            # and the server doesn't have the multi-prefix capability
+        if not bot.capabilities.is_enabled('multi-prefix'):
+            # and the multi-prefix capability is not enabled
             # so we can ask the server to use the NAMESX feature
             bot.write(('PROTOCTL', 'NAMESX'))
 
+    # was UHNAMES support status updated?
+    if not uhnames_support and 'UHNAMES' in bot.isupport:
+        # yes it was!
+        if not bot.capabilities.is_enabled('userhost-in-names'):
+            # and the userhost-in-names capability is not enabled
+            # so we should ask for UHNAMES instead
+            bot.write(('PROTOCTL', 'UHNAMES'))
+
 
-@module.event(events.RPL_MYINFO)
-@module.thread(False)
-@module.unblockable
+@plugin.event(events.RPL_ENDOFMOTD, events.ERR_NOMOTD)
+@plugin.thread(False)
+@plugin.unblockable
+@plugin.priority('medium')
+def join_channels(bot, trigger):
+    # join channels
+    channels = bot.config.core.channels
+    if not channels:
+        LOGGER.info("No initial channels to JOIN.")
+
+    elif bot.config.core.throttle_join:
+        throttle_rate = int(bot.config.core.throttle_join)
+        throttle_wait = max(bot.config.core.throttle_wait, 1)
+        channels_joined = 0
+
+        LOGGER.info(
+            "Joining %d channels (with JOIN throttle ON); "
+            "this may take a moment.",
+            len(channels))
+
+        for channel in channels:
+            channels_joined += 1
+            if not channels_joined % throttle_rate:
+                LOGGER.debug(
+                    "Waiting %ds before next JOIN batch.",
+                    throttle_wait)
+                time.sleep(throttle_wait)
+            bot.join(channel)
+    else:
+        LOGGER.info(
+            "Joining %d channels (with JOIN throttle OFF); "
+            "this may take a moment.",
+            len(channels))
+
+        for channel in bot.config.core.channels:
+            bot.join(channel)
+
+
+@plugin.event(events.RPL_MYINFO)
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def parse_reply_myinfo(bot, trigger):
     """Handle ``RPL_MYINFO`` events."""
     # keep <client> <servername> <version> only
     # the trailing parameters (mode types) should be read from ISUPPORT
-    bot._myinfo = MyInfo(*trigger.args[0:3])
+    bot._myinfo = utils.MyInfo(*trigger.args[0:3])
 
     LOGGER.info(
         "Received RPL_MYINFO from server: %s, %s, %s",
         bot._myinfo.client,
         bot._myinfo.servername,
         bot._myinfo.version,
     )
 
 
-@module.require_privmsg()
-@module.require_owner()
-@module.commands('useserviceauth')
+@plugin.require_privmsg()
+@plugin.require_owner()
+@plugin.commands('useserviceauth')
 def enable_service_auth(bot, trigger):
     """Set owner's account from an authenticated owner.
 
     This command can be used to automatically configure ``core.owner_account``
     when the owner is known and has a registered account, but the bot doesn't
     have ``core.owner_account`` configured.
 
     This doesn't work if the ``account-tag`` capability is not available.
     """
     if bot.config.core.owner_account:
         return
-    if 'account-tag' not in bot.enabled_capabilities:
+    if not bot.capabilities.is_enabled('account-tag'):
         bot.say('This server does not fully support services auth, so this '
                 'command is not available.')
         return
     if not trigger.account:
         bot.say('You must be logged in to network services before using this '
                 'command.')
         return
@@ -409,15 +570,15 @@
     LOGGER.info(
         "User %s set %s as owner account.",
         trigger.nick,
         trigger.account,
     )
 
 
-@module.event(events.ERR_NOCHANMODES)
+@plugin.event(events.ERR_NOCHANMODES)
 @plugin.priority('medium')
 def retry_join(bot, trigger):
     """Give NickServ enough time to identify on a +R channel.
 
     Give NickServ enough time to identify, and retry rejoining an
     identified-only (+R) channel. Maximum of ten rejoin attempts.
     """
@@ -437,89 +598,118 @@
     attempt = bot.memory['retry_join'][channel] + 1
     LOGGER.info(
         "Trying to rejoin channel %r (attempt %d/10)",
         str(channel), attempt)
     bot.join(channel)
 
 
-@module.rule('(.*)')
-@module.event(events.RPL_NAMREPLY)
-@module.thread(False)
-@module.unblockable
+@plugin.rule('(.*)')
+@plugin.event(events.RPL_NAMREPLY)
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def handle_names(bot, trigger):
     """Handle NAMES responses.
 
     This function keeps track of users' privileges when Sopel joins channels.
     """
-    names = trigger.split()
-
     # TODO specific to one channel type. See issue 281.
     channels = re.search(r'(#\S*)', trigger.raw)
     if not channels:
         return
-    channel = Identifier(channels.group(1))
-    if channel not in bot.privileges:
-        bot.privileges[channel] = {}
+    channel = bot.make_identifier(channels.group(1))
     if channel not in bot.channels:
-        bot.channels[channel] = target.Channel(channel)
+        bot.channels[channel] = target.Channel(
+            channel,
+            identifier_factory=bot.make_identifier,
+        )
 
     # This could probably be made flexible in the future, but I don't think
     # it'd be worth it.
     # If this ever needs to be updated, remember to change the mode handling in
     # the WHO-handler functions below, too.
     mapping = {
-        "+": module.VOICE,
-        "%": module.HALFOP,
-        "@": module.OP,
-        "&": module.ADMIN,
-        "~": module.OWNER,
-        "!": module.OPER,
+        "+": plugin.VOICE,
+        "%": plugin.HALFOP,
+        "@": plugin.OP,
+        "&": plugin.ADMIN,
+        "~": plugin.OWNER,
+        "!": plugin.OPER,
     }
 
+    uhnames = 'UHNAMES' in bot.isupport
+    userhost_in_names = bot.capabilities.is_enabled('userhost-in-names')
+
+    names = trigger.split()
     for name in names:
+        username = hostname = None
+
+        if uhnames or userhost_in_names:
+            try:
+                name, mask = name.rsplit('!', 1)
+                username, hostname = mask.split('@', 1)
+            except ValueError:
+                # server advertised either UHNAMES or userhost-in-names, but
+                # isn't sending the hostmask with all listed nicks
+                # It's probably ZNC. https://github.com/znc/znc/issues/1224
+                LOGGER.debug(
+                    '%s is enabled, but still got RPL_NAMREPLY item without a hostmask. '
+                    'IRC server/bouncer is not spec compliant.',
+                    'UHNAMES' if uhnames else 'userhost-in-names')
+
         priv = 0
-        for prefix, value in iteritems(mapping):
+        for prefix, value in mapping.items():
             if prefix in name:
                 priv = priv | value
-        nick = Identifier(name.lstrip(''.join(mapping.keys())))
-        bot.privileges[channel][nick] = priv
+
+        nick = bot.make_identifier(name.lstrip(''.join(mapping.keys())))
         user = bot.users.get(nick)
         if user is None:
-            # It's not possible to set the username/hostname from info received
-            # in a NAMES reply, unfortunately.
+            # The username/hostname will be included in a NAMES reply only if
+            # userhost-in-names is available. We can use them if present.
             # Fortunately, the user should already exist in bot.users by the
             # time this code runs, so this is 99.9% ass-covering.
-            user = target.User(nick, None, None)
+            user = target.User(nick, username, hostname)
             bot.users[nick] = user
         bot.channels[channel].add_user(user, privs=priv)
 
 
-@module.rule('(.*)')
-@module.event('MODE')
-@module.thread(False)
-@module.unblockable
+@plugin.rule('(.*)')
+@plugin.event('MODE')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_modes(bot, trigger):
     """Track changes from received MODE commands."""
     _parse_modes(bot, trigger.args)
 
 
-@module.priority('high')
-@module.event(events.RPL_CHANNELMODEIS)
-@module.thread(False)
-@module.unblockable
+@plugin.priority('high')
+@plugin.event(events.RPL_CHANNELMODEIS)
+@plugin.thread(False)
+@plugin.unblockable
 def initial_modes(bot, trigger):
     """Populate channel modes from response to MODE request sent after JOIN."""
     _parse_modes(bot, trigger.args[1:], clear=True)
 
 
 def _parse_modes(bot, args, clear=False):
-    """Parse MODE message and apply changes to internal state."""
-    channel_name = Identifier(args[0])
+    """Parse MODE message and apply changes to internal state.
+
+    Sopel, by default, doesn't know how to parse other types than A, B, C, and
+    D, and only a preset of privileges.
+
+    .. seealso::
+
+        Parsing mode messages can be tricky and complicated to understand. In
+        any case it is better to read the IRC specifications about channel
+        modes at https://modern.ircdocs.horse/#channel-mode
+
+    """
+    channel_name = bot.make_identifier(args[0])
     if channel_name.is_nick():
         # We don't do anything with user modes
         LOGGER.debug("Ignoring user modes: %r", args)
         return
 
     channel = bot.channels[channel_name]
 
@@ -529,246 +719,215 @@
         args.pop()
     # If any args are still empty, that's something we may not be prepared for,
     # but let's continue anyway hoping they're trailing / not important.
     if len(args) < 2 or not all(args):
         LOGGER.debug(
             "The server sent a possibly malformed MODE message: %r", args)
 
-    modestring = args[1]
-    params = args[2:]
+    # parse the modestring with the parameters
+    modeinfo = bot.modeparser.parse(args[1], tuple(args[2:]))
 
-    mapping = {
-        "v": module.VOICE,
-        "h": module.HALFOP,
-        "o": module.OP,
-        "a": module.ADMIN,
-        "q": module.OWNER,
-        "y": module.OPER,
-        "Y": module.OPER,
-    }
+    # set, unset, or update channel's modes based on the mode type
+    # modeinfo.modes contains only the valid parsed modes
+    # coretask can handle type A, B, C, and D only
+    modes = {} if clear else copy.deepcopy(channel.modes)
+    for letter, mode, is_added, param in modeinfo.modes:
+        if letter == 'A':
+            # type A is a multi-value mode and always requires a parameter
+            if mode not in modes:
+                modes[mode] = set()
+            if is_added:
+                modes[mode].add(param)
+            elif param in modes[mode]:
+                modes[mode].remove(param)
+                # remove mode if empty
+                if not modes[mode]:
+                    modes.pop(mode)
+        elif letter == 'B':
+            # type B is a single-value mode and always requires a parameter
+            if is_added:
+                modes[mode] = param
+            elif mode in modes:
+                modes.pop(mode)
+        elif letter == 'C':
+            # type C is a single-value mode and requires a parameter when added
+            if is_added:
+                modes[mode] = param
+            elif mode in modes:
+                modes.pop(mode)
+        elif letter == 'D':
+            # type D is a flag (True or False) and doesn't have a parameter
+            if is_added:
+                modes[mode] = True
+            elif mode in modes:
+                modes.pop(mode)
 
-    modes = {}
-    if not clear:
-        # Work on a copy for some thread safety
-        modes.update(channel.modes)
-
-    # Process modes
-    sign = ""
-    param_idx = 0
-    chanmodes = bot.isupport.CHANMODES
-    for char in modestring:
-        # Are we setting or unsetting
-        if char in "+-":
-            sign = char
-            continue
-
-        if char in chanmodes["A"]:
-            # Type A (beI, etc) have a nick or address param to add/remove
-            if char not in modes:
-                modes[char] = set()
-            if sign == "+":
-                modes[char].add(params[param_idx])
-            elif params[param_idx] in modes[char]:
-                modes[char].remove(params[param_idx])
-            param_idx += 1
-        elif char in chanmodes["B"]:
-            # Type B (k, etc) always have a param
-            if sign == "+":
-                modes[char] = params[param_idx]
-            elif char in modes:
-                modes.pop(char)
-            param_idx += 1
-        elif char in chanmodes["C"]:
-            # Type C (l, etc) have a param only when setting
-            if sign == "+":
-                modes[char] = params[param_idx]
-                param_idx += 1
-            elif char in modes:
-                modes.pop(char)
-        elif char in chanmodes["D"]:
-            # Type D (aciLmMnOpqrRst, etc) have no params
-            if sign == "+":
-                modes[char] = True
-            elif char in modes:
-                modes.pop(char)
-        elif char in mapping and (
-            "PREFIX" not in bot.isupport or char in bot.isupport.PREFIX
-        ):
-            # User privs modes, always have a param
-            nick = Identifier(params[param_idx])
-            priv = channel.privileges.get(nick, 0)
-            # Log a warning if the two privilege-tracking data structures
-            # get out of sync. That should never happen.
-            # This is a good place to verify that bot.channels is doing
-            # what it's supposed to do before ultimately removing the old,
-            # deprecated bot.privileges structure completely.
-            ppriv = bot.privileges[channel_name].get(nick, 0)
-            if priv != ppriv:
-                LOGGER.warning(
-                    (
-                        "Privilege data error! Please share Sopel's "
-                        "raw log with the developers, if enabled. "
-                        "(Expected %s == %s for %r in %r)"
-                    ),
-                    priv,
-                    ppriv,
-                    nick,
-                    channel,
-                )
-            value = mapping.get(char)
-            if value is not None:
-                if sign == "+":
-                    priv = priv | value
-                else:
-                    priv = priv & ~value
-                bot.privileges[channel_name][nick] = priv
-                channel.privileges[nick] = priv
-            param_idx += 1
+    # atomic change of channel's modes
+    channel.modes = modes
+
+    # update user privileges in channel
+    # modeinfo.privileges contains only the valid parsed privileges
+    for privilege, is_added, param in modeinfo.privileges:
+        # User privs modes, always have a param
+        nick = bot.make_identifier(param)
+        priv = channel.privileges.get(nick, 0)
+        value = MODE_PREFIX_PRIVILEGES[privilege]
+        if is_added:
+            priv = priv | value
         else:
-            # Might be in a mode block past A/B/C/D, but we don't speak those.
-            # Send a WHO to ensure no user priv modes we're skipping are lost.
-            LOGGER.warning(
-                "Unknown MODE message, sending WHO. Message was: %r",
-                args,
-            )
-            _send_who(bot, channel_name)
-            return
+            priv = priv & ~value
+        channel.privileges[nick] = priv
 
-    if param_idx != len(params):
+    # log ignored modes (modes Sopel doesn't know how to handle)
+    if modeinfo.ignored_modes:
         LOGGER.warning(
-            "Too many arguments received for MODE: args=%r chanmodes=%r",
+            "Unknown MODE message, sending WHO. Message was: %r",
             args,
-            chanmodes,
         )
+        # send a WHO message to ensure we didn't miss anything
+        _send_who(bot, channel_name)
 
-    channel.modes = modes
+    # log leftover parameters (too many arguments)
+    if modeinfo.leftover_params:
+        LOGGER.warning(
+            "Too many arguments received for MODE: args=%r chanmodes=%r",
+            args,
+            bot.modeparser.chanmodes,
+        )
 
     LOGGER.info("Updated mode for channel: %s", channel.name)
     LOGGER.debug("Channel %r mode: %r", str(channel.name), channel.modes)
 
 
-@module.event('NICK')
-@module.thread(False)
-@module.unblockable
+@plugin.event('NICK')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_nicks(bot, trigger):
     """Track nickname changes and maintain our chanops list accordingly."""
     old = trigger.nick
-    new = Identifier(trigger)
+    new = bot.make_identifier(trigger)
 
-    # Give debug mssage, and PM the owner, if the bot's own nick changes.
+    # Give debug message, and PM the owner, if the bot's own nick changes.
     if old == bot.nick and new != bot.nick:
-        privmsg = (
-            "Hi, I'm your bot, %s. Something has made my nick change. This "
-            "can cause some problems for me, and make me do weird things. "
-            "You'll probably want to restart me, and figure out what made "
-            "that happen so you can stop it happening again. (Usually, it "
-            "means you tried to give me a nick that's protected by NickServ.)"
-        ) % bot.nick
-        debug_msg = (
-            "Nick changed by server. This can cause unexpected behavior. "
-            "Please restart the bot."
-        )
-        LOGGER.critical(debug_msg)
-        bot.say(privmsg, bot.config.core.owner)
-        return
+        # Is this the original nick being regained?
+        # e.g. by ZNC's keepnick module running in front of Sopel
+        if old != bot.config.core.nick and new == bot.config.core.nick:
+            LOGGER.info(
+                "Regained configured nick. Restarting is still recommended.")
+        else:
+            privmsg = (
+                "Hi, I'm your bot, %s. Something has made my nick change. This "
+                "can cause some problems for me, and make me do weird things. "
+                "You'll probably want to restart me, and figure out what made "
+                "that happen so you can stop it happening again. (Usually, it "
+                "means you tried to give me a nick that's protected by NickServ.)"
+            ) % bot.config.core.nick
+            debug_msg = (
+                "Nick changed by server. This can cause unexpected behavior. "
+                "Please restart the bot."
+            )
+            LOGGER.critical(debug_msg)
+            bot.say(privmsg, bot.config.core.owner)
 
-    for channel in bot.privileges:
-        channel = Identifier(channel)
-        if old in bot.privileges[channel]:
-            value = bot.privileges[channel].pop(old)
-            bot.privileges[channel][new] = value
+        # Always update bot.nick anyway so Sopel doesn't lose its self-identity.
+        # This should cut down the number of "weird things" that happen while
+        # the active nick doesn't match the config, but it's not a substitute
+        # for regaining the expected nickname.
+        LOGGER.info("Updating bot.nick property with server-changed nick.")
+        bot._nick = new
+        return
 
     for channel in bot.channels.values():
         channel.rename_user(old, new)
     if old in bot.users:
         bot.users[new] = bot.users.pop(old)
 
-    LOGGER.info("User named %r is now known as %r.", old, str(new))
+    LOGGER.info("User named %r is now known as %r.", str(old), str(new))
 
 
-@module.rule('(.*)')
-@module.event('PART')
-@module.thread(False)
-@module.unblockable
+@plugin.rule('(.*)')
+@plugin.event('PART')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_part(bot, trigger):
     """Track users leaving channels."""
     nick = trigger.nick
     channel = trigger.sender
     _remove_from_channel(bot, nick, channel)
     LOGGER.info("User %r left a channel: %s", str(nick), channel)
 
 
-@module.event('KICK')
-@module.thread(False)
-@module.unblockable
+@plugin.event('KICK')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_kick(bot, trigger):
     """Track users kicked from channels."""
-    nick = Identifier(trigger.args[1])
+    nick = bot.make_identifier(trigger.args[1])
     channel = trigger.sender
     _remove_from_channel(bot, nick, channel)
     LOGGER.info(
         "User %r got kicked by %r from a channel: %s",
         str(nick),
         str(trigger.nick),
         channel,
     )
 
 
 def _remove_from_channel(bot, nick, channel):
     if nick == bot.nick:
-        bot.privileges.pop(channel, None)
         bot.channels.pop(channel, None)
 
         lost_users = []
         for nick_, user in bot.users.items():
             user.channels.pop(channel, None)
             if not user.channels:
                 lost_users.append(nick_)
         for nick_ in lost_users:
             bot.users.pop(nick_, None)
     else:
-        bot.privileges[channel].pop(nick, None)
-
         user = bot.users.get(nick)
         if user and channel in user.channels:
             bot.channels[channel].clear_user(nick)
             if not user.channels:
                 bot.users.pop(nick, None)
 
 
-def _send_who(bot, channel):
+def _send_who(bot, mask):
     if 'WHOX' in bot.isupport:
         # WHOX syntax, see http://faerion.sourceforge.net/doc/irc/whox.var
-        # Needed for accounts in WHO replies. The `CORE_QUERYTYPE` parameter
+        # Needed for accounts in WHO replies. The `WHOX_QUERYTYPE` parameter
         # for WHO is used to identify the reply from the server and confirm
         # that it has the requested format. WHO replies with different
         # querytypes in the response were initiated elsewhere and will be
         # ignored.
-        bot.write(['WHO', channel, 'a%nuachtf,' + CORE_QUERYTYPE])
+        bot.write(['WHO', mask, '{},{}'.format(WHOX_QUERY, WHOX_QUERYTYPE)])
     else:
         # We might be on an old network, but we still care about keeping our
         # user list updated
-        bot.write(['WHO', channel])
-    bot.channels[Identifier(channel)].last_who = datetime.datetime.utcnow()
+        bot.write(['WHO', mask])
+
+    target_id = bot.make_identifier(mask)
+    if not target_id.is_nick():
+        bot.channels[target_id].last_who = datetime.now(timezone.utc)
 
 
-@module.interval(30)
+@plugin.interval(30)
 def _periodic_send_who(bot):
     """Periodically send a WHO request to keep user information up-to-date."""
-    if 'away-notify' in bot.enabled_capabilities:
+    if bot.capabilities.is_enabled('away-notify'):
         # WHO not needed to update 'away' status
         return
 
-    # Loops through the channels to find the one that has the longest time since the last WHO
-    # request, and issues a WHO request only if the last request for the channel was more than
+    # Loop through the channels to find the one that has the longest time since the last WHO
+    # request, and issue a WHO request only if the last request for the channel was more than
     # 120 seconds ago.
-    who_trigger_time = datetime.datetime.utcnow() - datetime.timedelta(seconds=120)
+    who_trigger_time = datetime.now(timezone.utc) - timedelta(seconds=120)
     selected_channel = None
     for channel_name, channel in bot.channels.items():
         if channel.last_who is None:
             # WHO was never sent yet to this channel: stop here
             selected_channel = channel_name
             break
         if channel.last_who < who_trigger_time:
@@ -778,248 +937,228 @@
 
     if selected_channel is not None:
         # selected_channel's last who is either none or the oldest valid
         LOGGER.debug("Sending WHO for channel: %s", selected_channel)
         _send_who(bot, selected_channel)
 
 
-@module.event('JOIN')
-@module.thread(False)
-@module.unblockable
+@plugin.event('JOIN')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_join(bot, trigger):
     """Track users joining channels.
 
     When a user joins a channel, the bot will send (or queue) a ``WHO`` command
     to know more about said user (privileges, modes, etc.).
     """
     channel = trigger.sender
+    new_channel = channel not in bot.channels
+    self_join = trigger.nick == bot.nick
+    new_user = trigger.nick not in bot.users
 
     # is it a new channel?
-    if channel not in bot.channels:
-        bot.privileges[channel] = {}
-        bot.channels[channel] = target.Channel(channel)
+    if new_channel:
+        bot.channels[channel] = target.Channel(
+            channel,
+            identifier_factory=bot.make_identifier,
+        )
 
     # did *we* just join?
-    if trigger.nick == bot.nick:
+    if self_join:
         LOGGER.info("Channel joined: %s", channel)
+        bot.channels[channel].join_time = trigger.time
         if bot.settings.core.throttle_join:
             LOGGER.debug("JOIN event added to queue for channel: %s", channel)
             bot.memory['join_events_queue'].append(channel)
         else:
             LOGGER.debug("Send MODE and direct WHO for channel: %s", channel)
             bot.write(["MODE", channel])
             _send_who(bot, channel)
     else:
         LOGGER.info(
             "Channel %r joined by user: %s",
             str(channel), trigger.nick)
 
     # set initial values
-    bot.privileges[channel][trigger.nick] = 0
-
-    user = bot.users.get(trigger.nick)
-    if user is None:
+    if new_user:
         user = target.User(trigger.nick, trigger.user, trigger.host)
         bot.users[trigger.nick] = user
+    else:
+        user = bot.users.get(trigger.nick)
     bot.channels[channel].add_user(user)
 
     if len(trigger.args) > 1 and trigger.args[1] != '*' and (
-            'account-notify' in bot.enabled_capabilities and
-            'extended-join' in bot.enabled_capabilities):
+        bot.capabilities.is_enabled('account-notify') and
+        bot.capabilities.is_enabled('extended-join')
+    ):
         user.account = trigger.args[1]
 
+    if new_user and not new_channel:
+        # send WHO to populate new user's realname etc.
+        _send_who(bot, trigger.nick)
 
-@module.event('QUIT')
-@module.thread(False)
-@module.unblockable
+
+@plugin.event('QUIT')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_quit(bot, trigger):
     """Track when users quit channels."""
-    for chanprivs in bot.privileges.values():
-        chanprivs.pop(trigger.nick, None)
     for channel in bot.channels.values():
         channel.clear_user(trigger.nick)
     bot.users.pop(trigger.nick, None)
 
     LOGGER.info("User quit: %s", trigger.nick)
 
-    if trigger.nick == bot.settings.core.nick and trigger.nick != bot.nick:
+    configured_nick = bot.make_identifier(bot.settings.core.nick)
+    if trigger.nick == configured_nick and trigger.nick != bot.nick:
         # old nick is now available, let's change nick again
         bot.change_current_nick(bot.settings.core.nick)
         auth_after_register(bot)
 
 
-@module.event('CAP')
-@module.thread(False)
-@module.unblockable
-@plugin.priority('medium')
-def receive_cap_list(bot, trigger):
-    """Handle client capability negotiation."""
-    cap = trigger.strip('-=~')
-    # Server is listing capabilities
-    if trigger.args[1] == 'LS':
-        receive_cap_ls_reply(bot, trigger)
-    # Server denied CAP REQ
-    elif trigger.args[1] == 'NAK':
-        entry = bot._cap_reqs.get(cap, None)
-        # If it was requested with bot.cap_req
-        if entry:
-            for req in entry:
-                # And that request was mandatory/prohibit, and a callback was
-                # provided
-                if req.prefix and req.failure:
-                    # Call it.
-                    req.failure(bot, req.prefix + cap)
-    # Server is removing a capability
-    elif trigger.args[1] == 'DEL':
-        entry = bot._cap_reqs.get(cap, None)
-        # If it was requested with bot.cap_req
-        if entry:
-            for req in entry:
-                # And that request wasn't prohibit, and a callback was
-                # provided
-                if req.prefix != '-' and req.failure:
-                    # Call it.
-                    req.failure(bot, req.prefix + cap)
-    # Server is adding new capability
-    elif trigger.args[1] == 'NEW':
-        entry = bot._cap_reqs.get(cap, None)
-        # If it was requested with bot.cap_req
-        if entry:
-            for req in entry:
-                # And that request wasn't prohibit
-                if req.prefix != '-':
-                    # Request it
-                    bot.write(('CAP', 'REQ', req.prefix + cap))
-    # Server is acknowledging a capability
-    elif trigger.args[1] == 'ACK':
-        caps = trigger.args[2].split()
-        for cap in caps:
-            cap.strip('-~= ')
-            bot.enabled_capabilities.add(cap)
-            entry = bot._cap_reqs.get(cap, [])
-            for req in entry:
-                if req.success:
-                    req.success(bot, req.prefix + trigger)
-            if cap == 'sasl':  # TODO why is this not done with bot.cap_req?
-                try:
-                    receive_cap_ack_sasl(bot)
-                except ConfigurationError as error:
-                    LOGGER.error(str(error))
-                    bot.quit('Wrong SASL configuration.')
-
-
-def receive_cap_ls_reply(bot, trigger):
-    if bot.server_capabilities:
-        # We've already seen the results, so someone sent CAP LS from a plugin.
-        # We're too late to do SASL, and we don't want to send CAP END before
-        # the plugin has done what it needs to, so just return
+def _receive_cap_ls_reply(bot: SopelWrapper, trigger: Trigger) -> None:
+    if not bot.capabilities.handle_ls(bot, trigger):
+        # multi-line, we must wait for more
         return
 
-    for cap in trigger.split():
-        c = cap.split('=')
-        if len(c) == 2:
-            batched_caps[c[0]] = c[1]
-        else:
-            batched_caps[c[0]] = None
+    if not bot.request_capabilities():
+        # Negotiation end because there is nothing to request
+        LOGGER.info('No capability negotiation.')
+        bot.write(('CAP', 'END'))
 
-    # Not the last in a multi-line reply. First two args are * and LS.
-    if trigger.args[2] == '*':
-        return
 
-    LOGGER.info(
-        "Client capability negotiation list: %s",
-        ', '.join(batched_caps.keys()),
-    )
-    bot.server_capabilities = batched_caps
+def _handle_cap_acknowledgement(
+    bot: SopelWrapper,
+    cap_req: tuple[str, ...],
+    results: list[tuple[bool, Optional[plugin.CapabilityNegotiation]]],
+    was_completed: bool,
+) -> None:
+    if any(
+        callback_result[1] == plugin.CapabilityNegotiation.ERROR
+        for callback_result in results
+    ):
+        # error: a plugin needs something and the bot cannot function properly
+        LOGGER.error(
+            'Capability negotiation failed for request: "%s"',
+            ' '.join(cap_req),
+        )
+        bot.write(('CAP', 'END'))  # close negotiation now
+        bot.quit('Error negotiating capabilities.')
 
-    # If some other plugin requests it, we don't need to add another request.
-    # If some other plugin prohibits it, we shouldn't request it.
-    core_caps = [
-        'echo-message',
-        'multi-prefix',
-        'away-notify',
-        'cap-notify',
-        'server-time',
-    ]
-    for cap in core_caps:
-        if cap not in bot._cap_reqs:
-            bot._cap_reqs[cap] = [CapReq('', 'coretasks')]
-
-    def acct_warn(bot, cap):
-        LOGGER.info("Server does not support %s, or it conflicts with a custom "
-                    "plugin. User account validation unavailable or limited.",
-                    cap[1:])
-        if bot.config.core.owner_account or bot.config.core.admin_accounts:
-            LOGGER.warning(
-                "Owner or admin accounts are configured, but %s is not "
-                "supported by the server. This may cause unexpected behavior.",
-                cap[1:])
-    auth_caps = ['account-notify', 'extended-join', 'account-tag']
-    for cap in auth_caps:
-        if cap not in bot._cap_reqs:
-            bot._cap_reqs[cap] = [CapReq('', 'coretasks', acct_warn)]
-
-    for cap, reqs in iteritems(bot._cap_reqs):
-        # At this point, we know mandatory and prohibited don't co-exist, but
-        # we need to call back for optionals if they're also prohibited
-        prefix = ''
-        for entry in reqs:
-            if prefix == '-' and entry.prefix != '-':
-                entry.failure(bot, entry.prefix + cap)
-                continue
-            if entry.prefix:
-                prefix = entry.prefix
-
-        # It's not required, or it's supported, so we can request it
-        if prefix != '=' or cap in bot.server_capabilities:
-            # REQs fail as a whole, so we send them one capability at a time
-            bot.write(('CAP', 'REQ', entry.prefix + cap))
-        # If it's required but not in server caps, we need to call all the
-        # callbacks
-        else:
-            for entry in reqs:
-                if entry.failure and entry.prefix == '=':
-                    entry.failure(bot, entry.prefix + cap)
+    if not was_completed and bot.cap_requests.is_complete:
+        # success: negotiation is complete and wasn't already
+        LOGGER.info('Capability negotiation ended successfuly.')
+        bot.write(('CAP', 'END'))  # close negotiation now
 
-    # If we want to do SASL, we have to wait before we can send CAP END. So if
-    # we are, wait on 903 (SASL successful) to send it.
-    if bot.config.core.auth_method == 'sasl' or bot.config.core.server_auth_method == 'sasl':
-        bot.write(('CAP', 'REQ', 'sasl'))
-    else:
-        bot.write(('CAP', 'END'))
-        LOGGER.info("End of client capability negotiation requests.")
 
+def _receive_cap_ack(bot: SopelWrapper, trigger: Trigger) -> None:
+    was_completed = bot.cap_requests.is_complete
+    cap_ack: tuple[str, ...] = bot.capabilities.handle_ack(bot, trigger)
 
-def receive_cap_ack_sasl(bot):
-    # Presumably we're only here if we said we actually *want* sasl, but still
-    # check anyway in case the server glitched.
-    password, mech = _get_sasl_pass_and_mech(bot)
-    if not password:
-        return
+    try:
+        result: Optional[
+            list[tuple[bool, Optional[plugin.CapabilityNegotiation]]]
+        ] = bot.cap_requests.acknowledge(bot, cap_ack)
+    except config.ConfigurationError as error:
+        LOGGER.error(
+            'Configuration error on ACK capability "%s": %s',
+            ', '.join(cap_ack),
+            error,
+        )
+        bot.write(('CAP', 'END'))  # close negotiation now
+        bot.quit('Configuration error.')
+        return None
+    except Exception as error:
+        LOGGER.exception(
+            'Error on ACK capability "%s": %s',
+            ', '.join(cap_ack),
+            error,
+        )
+        bot.write(('CAP', 'END'))  # close negotiation now
+        bot.quit('Error negotiating capabilities.')
+        return None
 
-    mech = mech or 'PLAIN'
-    available_mechs = bot.server_capabilities.get('sasl', '')
-    available_mechs = available_mechs.split(',') if available_mechs else []
+    if result is None:
+        # a plugin may have requested the capability without using the proper
+        # interface: ignore
+        return None
 
-    if available_mechs and mech not in available_mechs:
-        """
-        Raise an error if configured to use an unsupported SASL mechanism,
-        but only if the server actually advertised supported mechanisms,
-        i.e. this network supports SASL 3.2
+    _handle_cap_acknowledgement(bot, cap_ack, result, was_completed)
 
-        SASL 3.1 failure is handled (when possible) by the sasl_mechs() function
 
-        See https://github.com/sopel-irc/sopel/issues/1780 for background
-        """
-        raise ConfigurationError(
-            "SASL mechanism '{}' is not advertised by this server.".format(mech))
+def _receive_cap_nak(bot: SopelWrapper, trigger: Trigger) -> None:
+    was_completed = bot.cap_requests.is_complete
+    cap_ack = bot.capabilities.handle_nak(bot, trigger)
 
-    bot.write(('AUTHENTICATE', mech))
+    try:
+        result: Optional[
+            list[tuple[bool, Optional[plugin.CapabilityNegotiation]]]
+        ] = bot.cap_requests.deny(bot, cap_ack)
+    except config.ConfigurationError as error:
+        LOGGER.error(
+            'Configuration error on NAK capability "%s": %s',
+            ', '.join(cap_ack),
+            error,
+        )
+        bot.write(('CAP', 'END'))  # close negotiation now
+        bot.quit('Configuration error.')
+        return None
+    except Exception as error:
+        LOGGER.exception(
+            'Error on NAK capability "%s": %s',
+            ', '.join(cap_ack),
+            error,
+        )
+        bot.write(('CAP', 'END'))  # close negotiation now
+        bot.quit('Error negotiating capabilities.')
+        return None
+
+    if result is None:
+        # a plugin may have requested the capability without using the proper
+        # interface: ignore
+        return None
+
+    _handle_cap_acknowledgement(bot, cap_ack, result, was_completed)
+
+
+def _receive_cap_new(bot: SopelWrapper, trigger: Trigger) -> None:
+    cap_new = bot.capabilities.handle_new(bot, trigger)
+    LOGGER.info('Capability is now available: %s', ', '.join(cap_new))
+    # TODO: try to request what wasn't requested before
+
+
+def _receive_cap_del(bot: SopelWrapper, trigger: Trigger) -> None:
+    cap_del = bot.capabilities.handle_del(bot, trigger)
+    LOGGER.info('Capability is now unavailable: %s', ', '.join(cap_del))
+    # TODO: what to do when a CAP is removed? NAK callbacks?
+
+
+CAP_HANDLERS: dict[str, Callable[[SopelWrapper, Trigger], None]] = {
+    'LS': _receive_cap_ls_reply,  # Server is listing capabilities
+    'ACK': _receive_cap_ack,  # Server is acknowledging a capability
+    'NAK': _receive_cap_nak,  # Server is denying a capability
+    'NEW': _receive_cap_new,  # Server is adding new capability
+    'DEL': _receive_cap_del,  # Server is removing a capability
+}
+
+
+@plugin.event('CAP')
+@plugin.thread(False)
+@plugin.unblockable
+@plugin.priority('medium')
+def receive_cap_list(bot: SopelWrapper, trigger: Trigger) -> None:
+    """Handle client capability negotiation."""
+    subcommand = trigger.args[1]
+    if subcommand in CAP_HANDLERS:
+        handler = CAP_HANDLERS[subcommand]
+        handler(bot, trigger)
+    else:
+        LOGGER.info('Unknown CAP subcommand received: %s', subcommand)
 
 
 def send_authenticate(bot, token):
     """Send ``AUTHENTICATE`` command to server with the given ``token``.
 
     :param bot: instance of IRC bot that must authenticate
     :param str token: authentication token
@@ -1045,98 +1184,122 @@
         bot.write(('AUTHENTICATE', chunk))
 
     # send empty (+) AUTHENTICATE when payload's length is a multiple of 400
     if len(payload) % chunk_size == 0:
         bot.write(('AUTHENTICATE', '+'))
 
 
-@module.event('AUTHENTICATE')
+@plugin.event('AUTHENTICATE')
 @plugin.thread(False)
-@module.unblockable
+@plugin.unblockable
 @plugin.priority('medium')
 def auth_proceed(bot, trigger):
     """Handle client-initiated SASL auth.
 
     If the chosen mechanism is client-first, the server sends an empty
     response (``AUTHENTICATE +``). In that case, Sopel will handle SASL auth
     that uses a token.
 
     .. important::
 
         If ``core.auth_method`` is set, then ``core.server_auth_method`` will
         be ignored. If none is set, then this function does nothing.
 
     """
-    if trigger.args[0] != '+':
-        # How did we get here? I am not good with computer.
-        LOGGER.warning("Aborting SASL: unexpected server reply '%s'" % trigger)
-        # Send `authenticate-abort` command
-        # See https://ircv3.net/specs/extensions/sasl-3.1#the-authenticate-command
-        bot.write(('AUTHENTICATE', '*'))
+    if bot.config.core.auth_method == 'sasl':
+        mech = bot.config.core.auth_target or 'PLAIN'
+    elif bot.config.core.server_auth_method == 'sasl':
+        mech = bot.config.core.server_auth_sasl_mech or 'PLAIN'
+    else:
+        return
+
+    if mech == 'EXTERNAL':
+        if trigger.args[0] != '+':
+            # not an expected response from the server; abort SASL
+            token = '*'
+        else:
+            token = '+'
+
+        bot.write(('AUTHENTICATE', token))
         return
-    # Is this right?
+
     if bot.config.core.auth_method == 'sasl':
         sasl_username = bot.config.core.auth_username
         sasl_password = bot.config.core.auth_password
     elif bot.config.core.server_auth_method == 'sasl':
         sasl_username = bot.config.core.server_auth_username
         sasl_password = bot.config.core.server_auth_password
     else:
+        # How did we get here? I am not good with computer
         return
+
     sasl_username = sasl_username or bot.nick
-    sasl_token = _make_sasl_plain_token(sasl_username, sasl_password)
-    LOGGER.info("Sending SASL Auth token.")
-    send_authenticate(bot, sasl_token)
+
+    if mech == 'PLAIN':
+        if trigger.args[0] == '+':
+            sasl_token = _make_sasl_plain_token(sasl_username, sasl_password)
+            LOGGER.info("Sending SASL Auth token.")
+            send_authenticate(bot, sasl_token)
+            return
+        else:
+            # Not an expected response from the server
+            LOGGER.warning(
+                'Aborting SASL: unexpected server reply "%s"', trigger,
+            )
+            # Send `authenticate-abort` command
+            # See https://ircv3.net/specs/extensions/sasl-3.1#the-authenticate-command
+            bot.write(('AUTHENTICATE', '*'))
+            return
+
+    # TODO: Implement SCRAM challenges
 
 
 def _make_sasl_plain_token(account, password):
     return '\x00'.join((account, account, password))
 
 
-@module.event(events.RPL_SASLSUCCESS)
+@plugin.event(events.RPL_SASLSUCCESS)
 @plugin.thread(False)
-@module.unblockable
+@plugin.unblockable
 @plugin.priority('medium')
-def sasl_success(bot, trigger):
-    """End CAP request on successful SASL auth.
-
-    If SASL is configured, then the bot won't send ``CAP END`` once it gets
-    all the capability responses; it will wait for SASL auth result.
-
-    In this case, the SASL auth is a success, so we can close the negotiation.
-    """
+def sasl_success(bot: SopelWrapper, trigger: Trigger):
+    """Resume capability negotiation on successful SASL auth."""
     LOGGER.info("Successful SASL Auth.")
-    bot.write(('CAP', 'END'))
-    LOGGER.info("End of client capability negotiation requests.")
+    bot.resume_capability_negotiation(CAP_SASL.cap_req, 'coretasks')
 
 
 @plugin.event(events.ERR_SASLFAIL)
 @plugin.event(events.ERR_SASLTOOLONG)
 @plugin.event(events.ERR_SASLABORTED)
 @plugin.event(events.ERR_NICKLOCKED)
 @plugin.thread(False)
 @plugin.unblockable
 @plugin.priority('medium')
 def sasl_fail(bot, trigger):
     """SASL Auth Failed: log the error and quit."""
     LOGGER.error(
         "SASL Auth Failed; check your configuration: %s",
         str(trigger))
+    # negotiation done
+    bot.resume_capability_negotiation(CAP_SASL.cap_req, 'coretasks')
+    # quit
     bot.quit('SASL Auth Failed')
 
 
-@module.event(events.RPL_SASLMECHS)
+@plugin.event(events.RPL_SASLMECHS)
 @plugin.thread(False)
-@module.unblockable
+@plugin.unblockable
 @plugin.priority('low')
 def sasl_mechs(bot, trigger):
     # Presumably we're only here if we said we actually *want* sasl, but still
     # check anyway in case the server glitched.
     password, mech = _get_sasl_pass_and_mech(bot)
     if not password:
+        # negotiation done
+        bot.resume_capability_negotiation(CAP_SASL.cap_req, 'coretasks')
         return
 
     supported_mechs = trigger.args[1].split(',')
     if mech not in supported_mechs:
         """
         How we get here:
 
@@ -1146,259 +1309,318 @@
         3. The server doesn't support the mechanism Sopel used, and is a good
            IRC citizen, so it sends this optional numeric, 908 RPL_SASLMECHS
 
         Note that misconfigured SASL 3.1 will just silently fail when connected
         to an IRC server NOT implementing the optional 908 reply.
 
         A network with SASL 3.2 should theoretically never get this far because
-        Sopel should catch the unadvertised mechanism in receive_cap_ack_sasl().
+        Sopel should catch the unadvertised mechanism in CAP_SASL.
 
         See https://github.com/sopel-irc/sopel/issues/1780 for background
         """
         LOGGER.error(
             "Configured SASL mechanism '%s' is not advertised by this server. "
             "Advertised values: %s",
             mech,
             ', '.join(supported_mechs),
         )
+        bot.resume_capability_negotiation(CAP_SASL.cap_req, 'coretasks')
         bot.quit('Wrong SASL configuration.')
     else:
         LOGGER.info(
             "Selected SASL mechanism is %s, advertised: %s",
             mech,
             ', '.join(supported_mechs),
         )
 
 
 def _get_sasl_pass_and_mech(bot):
     password = None
     mech = None
+
     if bot.config.core.auth_method == 'sasl':
         password = bot.config.core.auth_password
         mech = bot.config.core.auth_target
     elif bot.config.core.server_auth_method == 'sasl':
         password = bot.config.core.server_auth_password
         mech = bot.config.core.server_auth_sasl_mech
+
+    mech = 'PLAIN' if mech is None else mech.upper()
+
     return password, mech
 
 
 # Live blocklist editing
 
 
-@module.commands('blocks')
-@module.thread(False)
-@module.unblockable
-@module.priority('low')
-@module.require_admin
+@plugin.commands('blocks')
+@plugin.example(r'.blocks del nick falsep0sitive', user_help=True)
+@plugin.example(r'.blocks add host some\.malicious\.network', user_help=True)
+@plugin.example(r'.blocks add nick sp(a|4)mb(o|0)t\d*', user_help=True)
+@plugin.thread(False)
+@plugin.unblockable
+@plugin.priority('low')
+@plugin.require_admin
 def blocks(bot, trigger):
-    """
-    Manage Sopel's blocking features.\
-    See [ignore system documentation]({% link _usage/ignoring-people.md %}).
+    """Manage Sopel's blocking features.
+
+    Full argspec: `list [nick|host]` or `[add|del] [nick|host] pattern`
     """
     STRINGS = {
         "success_del": "Successfully deleted block: %s",
         "success_add": "Successfully added block: %s",
         "no_nick": "No matching nick block found for: %s",
-        "no_host": "No matching hostmask block found for: %s",
-        "invalid": "Invalid format for %s a block. Try: .blocks add (nick|hostmask) sopel",
+        "no_host": "No matching host block found for: %s",
+        "invalid": "Invalid format for %s a block. Try: .blocks add (nick|host) sopel",
         "invalid_display": "Invalid input for displaying blocks.",
         "nonelisted": "No %s listed in the blocklist.",
         'huh': "I could not figure out what you wanted to do.",
     }
 
-    masks = set(s for s in bot.config.core.host_blocks if s != '')
-    nicks = set(Identifier(nick)
+    hosts = set(s for s in bot.config.core.host_blocks if s != '')
+    nicks = set(bot.make_identifier(nick)
                 for nick in bot.config.core.nick_blocks
                 if nick != '')
     text = trigger.group().split()
 
     if len(text) == 3 and text[1] == "list":
-        if text[2] == "hostmask":
-            if len(masks) > 0:
-                blocked = ', '.join(unicode(mask) for mask in masks)
-                bot.say("Blocked hostmasks: {}".format(blocked))
+        if text[2] == "host":
+            if len(hosts) > 0:
+                blocked = ', '.join(str(host) for host in hosts)
+                bot.say("Blocked hosts: {}".format(blocked))
             else:
-                bot.reply(STRINGS['nonelisted'] % ('hostmasks'))
+                bot.reply(STRINGS['nonelisted'] % ('hosts'))
         elif text[2] == "nick":
             if len(nicks) > 0:
-                blocked = ', '.join(unicode(nick) for nick in nicks)
+                blocked = ', '.join(str(nick) for nick in nicks)
                 bot.say("Blocked nicks: {}".format(blocked))
             else:
                 bot.reply(STRINGS['nonelisted'] % ('nicks'))
         else:
             bot.reply(STRINGS['invalid_display'])
 
     elif len(text) == 4 and text[1] == "add":
         if text[2] == "nick":
             nicks.add(text[3])
             bot.config.core.nick_blocks = nicks
             bot.config.save()
-        elif text[2] == "hostmask":
-            masks.add(text[3].lower())
-            bot.config.core.host_blocks = list(masks)
+        elif text[2] == "host":
+            hosts.add(text[3].lower())
+            bot.config.core.host_blocks = list(hosts)
+            bot.config.save()
         else:
             bot.reply(STRINGS['invalid'] % ("adding"))
             return
 
         bot.reply(STRINGS['success_add'] % (text[3]))
 
     elif len(text) == 4 and text[1] == "del":
         if text[2] == "nick":
-            if Identifier(text[3]) not in nicks:
+            nick = bot.make_identifier(text[3])
+            if nick not in nicks:
                 bot.reply(STRINGS['no_nick'] % (text[3]))
                 return
-            nicks.remove(Identifier(text[3]))
-            bot.config.core.nick_blocks = [unicode(n) for n in nicks]
+            nicks.remove(nick)
+            bot.config.core.nick_blocks = [str(n) for n in nicks]
             bot.config.save()
             bot.reply(STRINGS['success_del'] % (text[3]))
-        elif text[2] == "hostmask":
-            mask = text[3].lower()
-            if mask not in masks:
+        elif text[2] == "host":
+            host = text[3].lower()
+            if host not in hosts:
                 bot.reply(STRINGS['no_host'] % (text[3]))
                 return
-            masks.remove(mask)
-            bot.config.core.host_blocks = [unicode(m) for m in masks]
+            hosts.remove(host)
+            bot.config.core.host_blocks = [str(m) for m in hosts]
             bot.config.save()
             bot.reply(STRINGS['success_del'] % (text[3]))
         else:
             bot.reply(STRINGS['invalid'] % ("deleting"))
             return
     else:
         bot.reply(STRINGS['huh'])
 
 
-@module.event('ACCOUNT')
+@plugin.event('CHGHOST')
+@plugin.thread(False)
+@plugin.unblockable
+@plugin.priority('medium')
+def recv_chghost(bot, trigger):
+    """Track user/host changes."""
+    if trigger.nick not in bot.users:
+        bot.users[trigger.nick] = target.User(
+            trigger.nick, trigger.user, trigger.host)
+
+    try:
+        new_user, new_host = trigger.args
+    except ValueError:
+        LOGGER.warning(
+            "Ignoring CHGHOST command with %s arguments: %r",
+            'extra' if len(trigger.args) > 2 else 'insufficient',
+            trigger.args)
+        return
+
+    bot.users[trigger.nick].user = new_user
+    bot.users[trigger.nick].host = new_host
+    LOGGER.info(
+        "Update user@host for nick %r: %s@%s",
+        str(trigger.nick), new_user, new_host)
+
+
+@plugin.event('ACCOUNT')
 @plugin.thread(False)
 @plugin.unblockable
 @plugin.priority('medium')
 def account_notify(bot, trigger):
     """Track users' accounts."""
     if trigger.nick not in bot.users:
         bot.users[trigger.nick] = target.User(
             trigger.nick, trigger.user, trigger.host)
     account = trigger.args[0]
     if account == '*':
         account = None
     bot.users[trigger.nick].account = account
-    LOGGER.info("Update account for nick %r: %s", trigger.nick, account)
+    LOGGER.info("Update account for nick %r: %s", str(trigger.nick), account)
 
 
-@module.event(events.RPL_WHOSPCRPL)
+@plugin.event(events.RPL_WHOSPCRPL)
 @plugin.thread(False)
-@module.unblockable
+@plugin.unblockable
 @plugin.priority('medium')
 def recv_whox(bot, trigger):
     """Track ``WHO`` responses when ``WHOX`` is enabled."""
-    if len(trigger.args) < 2 or trigger.args[1] != CORE_QUERYTYPE:
+    if len(trigger.args) < 2 or trigger.args[1] != WHOX_QUERYTYPE:
         # Ignored, some plugin probably called WHO
         LOGGER.debug("Ignoring WHO reply for channel '%s'; not queried by coretasks", trigger.args[1])
         return
-    if len(trigger.args) != 8:
+    if len(trigger.args) != len(WHOX_QUERY):
         LOGGER.warning(
             "While populating `bot.accounts` a WHO response was malformed.")
         return
-    _, _, channel, user, host, nick, status, account = trigger.args
+    _, _, channel, user, host, nick, status, account, realname = trigger.args
+    botmode = bot.isupport.get('BOT')
     away = 'G' in status
+    is_bot = (botmode in status) if botmode else None
     modes = ''.join([c for c in status if c in '~&@%+!'])
-    _record_who(bot, channel, user, host, nick, account, away, modes)
+    _record_who(bot, channel, user, host, nick, realname, account, away, is_bot, modes)
 
 
-def _record_who(bot, channel, user, host, nick, account=None, away=None, modes=None):
-    nick = Identifier(nick)
-    channel = Identifier(channel)
+def _record_who(
+    bot: Sopel,
+    channel: Identifier,
+    user: str,
+    host: str,
+    nick: str,
+    realname: Optional[str] = None,
+    account: Optional[str] = None,
+    away: Optional[bool] = None,
+    is_bot: Optional[bool] = None,
+    modes: Optional[str] = None,
+):
+    nick = bot.make_identifier(nick)
+    channel = bot.make_identifier(channel)
     if nick not in bot.users:
         usr = target.User(nick, user, host)
         bot.users[nick] = usr
     else:
         usr = bot.users[nick]
         # check for & fill in sparse User added by handle_names()
         if usr.host is None and host:
             usr.host = host
         if usr.user is None and user:
             usr.user = user
+    if realname:
+        usr.realname = realname
     if account == '0':
         usr.account = None
     else:
         usr.account = account
     if away is not None:
         usr.away = away
+    if is_bot is not None:
+        usr.is_bot = is_bot
     priv = 0
     if modes:
         mapping = {
-            "+": module.VOICE,
-            "%": module.HALFOP,
-            "@": module.OP,
-            "&": module.ADMIN,
-            "~": module.OWNER,
-            "!": module.OPER,
+            "+": plugin.VOICE,
+            "%": plugin.HALFOP,
+            "@": plugin.OP,
+            "&": plugin.ADMIN,
+            "~": plugin.OWNER,
+            "!": plugin.OPER,
         }
         for c in modes:
             priv = priv | mapping[c]
     if channel not in bot.channels:
-        bot.channels[channel] = target.Channel(channel)
+        bot.channels[channel] = target.Channel(
+            channel,
+            identifier_factory=bot.make_identifier,
+        )
+
     bot.channels[channel].add_user(usr, privs=priv)
-    if channel not in bot.privileges:
-        bot.privileges[channel] = {}
-    bot.privileges[channel][nick] = priv
 
 
-@module.event(events.RPL_WHOREPLY)
+@plugin.event(events.RPL_WHOREPLY)
 @plugin.thread(False)
-@module.unblockable
+@plugin.unblockable
 @plugin.priority('medium')
 def recv_who(bot, trigger):
     """Track ``WHO`` responses when ``WHOX`` is not enabled."""
     channel, user, host, _, nick, status = trigger.args[1:7]
+    botmode = bot.isupport.get('BOT')
+    realname = trigger.args[-1].partition(' ')[-1]
     away = 'G' in status
+    is_bot = (botmode in status) if botmode else None
     modes = ''.join([c for c in status if c in '~&@%+!'])
-    _record_who(bot, channel, user, host, nick, away=away, modes=modes)
+    _record_who(
+        bot, channel, user, host, nick, realname,
+        away=away, is_bot=is_bot, modes=modes,
+    )
 
 
-@module.event('AWAY')
-@module.thread(False)
-@module.unblockable
+@plugin.event('AWAY')
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_notify(bot, trigger):
     """Track users going away or coming back."""
     if trigger.nick not in bot.users:
         bot.users[trigger.nick] = target.User(
             trigger.nick, trigger.user, trigger.host)
     user = bot.users[trigger.nick]
     user.away = bool(trigger.args)
     state_change = 'went away' if user.away else 'came back'
     LOGGER.info("User %s: %s", state_change, trigger.nick)
 
 
-@module.event('TOPIC')
-@module.event(events.RPL_TOPIC)
-@module.thread(False)
-@module.unblockable
+@plugin.event('TOPIC')
+@plugin.event(events.RPL_TOPIC)
+@plugin.thread(False)
+@plugin.unblockable
 @plugin.priority('medium')
 def track_topic(bot, trigger):
     """Track channels' topics."""
     if trigger.event != 'TOPIC':
         channel = trigger.args[1]
     else:
         channel = trigger.args[0]
     if channel not in bot.channels:
         return
     bot.channels[channel].topic = trigger.args[-1]
     LOGGER.info("Channel's topic updated: %s", channel)
 
 
-@module.rule(r'(?u).*(.+://\S+).*')
+@plugin.rule(r'(?u).*(.+://\S+).*')
 def handle_url_callbacks(bot, trigger):
     """Dispatch callbacks on URLs
 
     For each URL found in the trigger, trigger the URL callback registered by
     the ``@url`` decorator.
     """
-    schemes = bot.config.core.auto_url_schemes
     # find URLs in the trigger
-    for url in web.search_urls(trigger, schemes=schemes):
+    for url in trigger.urls:
         # find callbacks for said URL
         for function, match in bot.search_url_callbacks(url):
             # trigger callback defined by the `@url` decorator
             if hasattr(function, 'url_regex'):
                 # bake the `match` argument in before passing the callback on
                 @functools.wraps(function)
                 def decorated(bot, trigger):
```

### Comparing `sopel-7.1.9/sopel/db.py` & `sopel-8.0.0/sopel/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-# coding=utf-8
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""Sopel database module: management and tools around Sopel's datamodel.
+
+This module defines a datamodel, using `SQLAlchemy ORM's mapping`__:
+
+* :class:`NickIDs` and :class:`Nicknames` are used to track users
+* :class:`NickValues` is used to store arbitrary values for users
+* :class:`ChannelValues` is used to store arbitrary values for channels
+* :class:`PluginValues` is used to store arbitrary values for plugins
+
+These models are made available through the :class:`SopelDB` class and its
+convenience methods, such as :meth:`~SopelDB.get_nick_value` or
+:meth:`~SopelDB.get_channel_value`.
+
+.. __: https://docs.sqlalchemy.org/en/14/orm/tutorial.html#declare-a-mapping
+"""
+from __future__ import annotations
 
 import errno
 import json
 import logging
 import os.path
-import sys
 import traceback
+import typing
 
 from sqlalchemy import Column, create_engine, ForeignKey, Integer, String
-from sqlalchemy.engine.url import URL
-from sqlalchemy.exc import OperationalError, SQLAlchemyError
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import scoped_session, sessionmaker
-
-from sopel.tools import Identifier
-
-if sys.version_info.major >= 3:
-    unicode = str
-    basestring = str
+from sqlalchemy.engine.url import make_url, URL
+from sqlalchemy.exc import OperationalError
+from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker
+from sqlalchemy.sql import delete, func, select, update
+
+from sopel.lifecycle import deprecated
+from sopel.tools.identifiers import Identifier, IdentifierFactory
+
+if typing.TYPE_CHECKING:
+    from collections.abc import Iterable
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _deserialize(value):
     if value is None:
         return None
     # sqlite likes to return ints for strings that look like ints, even though
     # the column type is string. That's how you do dynamic typing wrong.
-    value = unicode(value)
+    value = str(value)
     # Just in case someone's mucking with the DB in a way we can't account for,
     # ignore json parsing errors
     try:
         value = json.loads(value)
     except ValueError:
         pass
     return value
@@ -83,63 +97,88 @@
     __tablename__ = 'plugin_values'
     __table_args__ = MYSQL_TABLE_ARGS
     plugin = Column(String(255), primary_key=True)
     key = Column(String(255), primary_key=True)
     value = Column(String(255))
 
 
-class SopelDB(object):
+class SopelDB:
     """Database object class.
 
     :param config: Sopel's configuration settings
     :type config: :class:`sopel.config.Config`
+    :param identifier_factory: factory for
+                               :class:`~sopel.tools.identifiers.Identifier`
+    :type: Callable[[:class:`str`], :class:`str`]
 
     This defines a simplified interface for basic, common operations on the
-    bot's database. Direct access to the database is also available, to serve
-    more complex plugins' needs.
+    bot's database. Direct access to the database is also available through
+    its :attr:`engine` attribute, to serve more complex plugins' needs.
 
     When configured to use SQLite with a relative filename, the file is assumed
     to be in the directory named by the core setting ``homedir``.
 
     .. versionadded:: 5.0
 
     .. versionchanged:: 7.0
 
         Switched from direct SQLite access to :ref:`SQLAlchemy
         <sqlalchemy:overview>`, allowing users more flexibility around what type
         of database they use (especially on high-load Sopel instances, which may
         run up against SQLite's concurrent-access limitations).
 
-    """
+    .. versionchanged:: 8.0
+
+        An Identifier factory can be provided that will be used to instantiate
+        :class:`~sopel.tools.identifiers.Identifier` when dealing with Nick or
+        Channel names.
+
+    .. seealso::
 
-    def __init__(self, config):
-        # MySQL - mysql://username:password@localhost/db
-        # SQLite - sqlite:////home/sopel/.sopel/default.db
-        self.type = config.core.db_type
+        For any advanced usage of the ORM, refer to the
+        `SQLAlchemy documentation`__.
 
-        # Handle SQLite explicitly as a default
-        if self.type == 'sqlite':
+    .. __: https://docs.sqlalchemy.org/en/14/
+    """
+
+    def __init__(
+        self,
+        config,
+        identifier_factory: IdentifierFactory = Identifier,
+    ) -> None:
+        self.make_identifier: IdentifierFactory = identifier_factory
+
+        if config.core.db_url is not None:
+            self.url = make_url(config.core.db_url)
+
+            # TODO: there's no way to get `config.core.db_type.choices`, but
+            # it would be nice to validate this type name somehow. Shouldn't
+            # affect anything, since the only thing it's ever used for is
+            # checking whether the configured database is 'sqlite'.
+            self.type = self.url.drivername.split('+', 1)[0]
+        elif config.core.db_type == 'sqlite':
+            self.type = 'sqlite'
             path = config.core.db_filename
             if path is None:
                 path = os.path.join(config.core.homedir, config.basename + '.db')
             path = os.path.expanduser(path)
             if not os.path.isabs(path):
                 path = os.path.normpath(os.path.join(config.core.homedir, path))
             if not os.path.isdir(os.path.dirname(path)):
                 raise OSError(
                     errno.ENOENT,
                     'Cannot create database file. '
                     'No such directory: "{}". Check that configuration setting '
                     'core.db_filename is valid'.format(os.path.dirname(path)),
                     path
                 )
-            self.filename = path
-            self.url = 'sqlite:///%s' % path
-        # Otherwise, handle all other database engines
+            self.url = make_url('sqlite:///' + path)
         else:
+            self.type = config.core.db_type
+
             query = {}
             if self.type == 'mysql':
                 drivername = config.core.db_driver or 'mysql'
                 query = {'charset': 'utf8mb4'}
             elif self.type == 'postgres':
                 drivername = config.core.db_driver or 'postgresql'
             elif self.type == 'oracle':
@@ -149,42 +188,66 @@
             elif self.type == 'firebird':
                 drivername = config.core.db_driver or 'firebird+fdb'
             elif self.type == 'sybase':
                 drivername = config.core.db_driver or 'sybase+pysybase'
             else:
                 raise Exception('Unknown db_type')
 
-            db_user = config.core.db_user
-            db_pass = config.core.db_pass
-            db_host = config.core.db_host
+            db_user = config.core.db_user  # Sometimes empty
+            db_pass = config.core.db_pass  # Sometimes empty
+            db_host = config.core.db_host  # Sometimes empty
             db_port = config.core.db_port  # Optional
-            db_name = config.core.db_name  # Optional, depending on DB
+            db_name = config.core.db_name  # Sometimes optional
 
             # Ensure we have all our variables defined
             if db_user is None or db_pass is None or db_host is None:
                 raise Exception('Please make sure the following core '
                                 'configuration values are defined: '
                                 'db_user, db_pass, db_host')
             self.url = URL(drivername=drivername, username=db_user,
                            password=db_pass, host=db_host, port=db_port,
                            database=db_name, query=query)
 
         self.engine = create_engine(self.url, pool_recycle=3600)
+        """SQLAlchemy Engine used to connect to Sopel's database.
+
+        .. seealso::
+
+            Read `SQLAlchemy engine`__'s documentation to know how to use it.
+
+        .. __: https://docs.sqlalchemy.org/en/14/core/connections.html
+
+        .. important::
+
+            Introduced in Sopel 7, Sopel uses SQLAlchemy 1.4+. This version of
+            SQLAlchemy deprecates various behaviors and methods, to prepare the
+            migration to its future 2.0 version, and the new 2.x style.
+
+            Sopel doesn't enforce the new 2.x style yet. This will be modified
+            in Sopel 9 by using the ``future=True`` flag on the engine.
+
+            You can read more about the `migration guide from 1.x to 2.x`__, as
+            Sopel will ensure in a future version that it is compatible with
+            the new style.
+
+        .. __: https://docs.sqlalchemy.org/en/14/changelog/migration_20.html
+        """
 
         # Catch any errors connecting to database
         try:
             self.engine.connect()
         except OperationalError:
             print("OperationalError: Unable to connect to database.")
             raise
 
         # Create our tables
         BASE.metadata.create_all(self.engine)
 
-        self.ssession = scoped_session(sessionmaker(bind=self.engine))
+        self.ssession = scoped_session(
+            sessionmaker(bind=self.engine, future=True))
 
     def connect(self):
         """Get a direct database connection.
 
         :return: a proxied DBAPI connection object; see
                  :meth:`sqlalchemy.engine.Engine.raw_connection()`
 
@@ -230,136 +293,166 @@
            If your plugin needs to remain compatible with Sopel versions prior
            to 7.0, you can use :meth:`connect` to get a raw connection. See
            its documentation for relevant warnings and compatibility caveats.
 
         """
         return self.ssession()
 
+    @deprecated('Use SopelDB.engine directly', version='8.0', removed_in='9.0')
     def execute(self, *args, **kwargs):
         """Execute an arbitrary SQL query against the database.
 
         :return: the query results
-        :rtype: :class:`sqlalchemy.engine.ResultProxy`
+        :rtype: :class:`sqlalchemy.engine.Result`
+
+        The ``Result`` object returned is a wrapper around a ``Cursor`` object
+        as specified by :pep:`249`.
+
+        .. deprecated:: 8.0
+
+            This method will be removed in Sopel 9, following the deprecation
+            of SQLAlchemy's :meth:`sqlalchemy.engine.Engine.execute`.
+
+            To perform a raw SQL query, use the :class:`~SopelDB.engine`
+            attribute as per the migration guide from SQLAlchemy::
+
+                from sqlalchemy.sql import text
+
+                def my_command(bot, trigger):
+                    raw_sql = ' ... '  # your raw SQL
+                    # get a connection as a context manager
+                    with bot.db.engine.connect() as conn:
+                        res = conn.execute(text(raw_sql))
+                        data = res.fetchall()
+
+                    # do something with your data here
+
+        .. seealso::
 
-        The ``ResultProxy`` object returned is a wrapper around a ``Cursor``
-        object as specified by PEP 249.
+            Read the `migration guide from 1.x style to 2.x style`__ by
+            SQLAlchemy to learn more about using SQLALchemy's engine and
+            connection.
+
+        .. __: https://docs.sqlalchemy.org/en/14/changelog/migration_20.html
         """
         return self.engine.execute(*args, **kwargs)
 
-    def get_uri(self):
+    def get_uri(self) -> URL:
         """Return a direct URL for the database.
 
         :return: the database connection URI
         :rtype: str
 
         This can be used to connect from a plugin using another SQLAlchemy
         instance, for example, without sharing the bot's connection.
         """
         return self.url
 
     # NICK FUNCTIONS
 
-    def get_nick_id(self, nick, create=True):
+    def get_nick_id(self, nick: str, create: bool = False) -> int:
         """Return the internal identifier for a given nick.
 
         :param nick: the nickname for which to fetch an ID
-        :type nick: :class:`~sopel.tools.Identifier`
-        :param bool create: whether to create an ID if one does not exist
+        :param create: whether to create an ID if one does not exist
+                       (set to ``False`` by default)
         :raise ValueError: if no ID exists for the given ``nick`` and ``create``
                            is set to ``False``
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         The nick ID is shared across all of a user's aliases, assuming their
         nicks have been grouped together.
 
+        .. versionchanged:: 8.0
+
+            The ``create`` parameter is now ``False`` by default.
+
         .. seealso::
 
             Alias/group management functions: :meth:`alias_nick`,
             :meth:`unalias_nick`, :meth:`merge_nick_groups`, and
-            :meth:`delete_nick_group`.
+            :meth:`forget_nick_group`.
 
         """
-        session = self.ssession()
-        slug = nick.lower()
-        try:
-            nickname = session.query(Nicknames) \
-                .filter(Nicknames.slug == slug) \
-                .one_or_none()
+        slug = self.make_identifier(nick).lower()
+        with self.session() as session:
+            nickname = session.execute(
+                select(Nicknames).where(Nicknames.slug == slug)
+            ).scalar_one_or_none()
 
             if nickname is None:
                 # see if it needs case-mapping migration
-                nickname = session.query(Nicknames) \
-                    .filter(Nicknames.slug == Identifier._lower_swapped(nick)) \
-                    .one_or_none()
+                nickname = session.execute(
+                    select(Nicknames)
+                    .where(Nicknames.slug == Identifier._lower_swapped(nick))
+                ).scalar_one_or_none()
+
                 if nickname is not None:
                     # it does!
                     nickname.slug = slug
                     session.commit()
 
             if nickname is None:  # "is /* still */ None", if Python had inline comments
                 if not create:
                     raise ValueError('No ID exists for the given nick')
                 # Generate a new ID
                 nick_id = NickIDs()
                 session.add(nick_id)
                 session.commit()
 
                 # Create a new Nickname
-                nickname = Nicknames(nick_id=nick_id.nick_id, slug=slug, canonical=nick)
+                nickname = Nicknames(
+                    nick_id=nick_id.nick_id,
+                    slug=slug,
+                    canonical=nick,
+                )
                 session.add(nickname)
                 session.commit()
             return nickname.nick_id
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def alias_nick(self, nick, alias):
+    def alias_nick(self, nick: str, alias: str) -> None:
         """Create an alias for a nick.
 
-        :param str nick: an existing nickname
-        :param str alias: an alias by which ``nick`` should also be known
+        :param nick: an existing nickname
+        :param alias: an alias by which ``nick`` should also be known
         :raise ValueError: if the ``alias`` already exists
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. seealso::
 
             To merge two *existing* nick groups, use :meth:`merge_nick_groups`.
 
             To remove an alias created with this function, use
             :meth:`unalias_nick`.
 
         """
-        nick = Identifier(nick)
-        alias = Identifier(alias)
-        nick_id = self.get_nick_id(nick)
-        session = self.ssession()
-        try:
-            result = session.query(Nicknames) \
-                .filter(Nicknames.slug == alias.lower()) \
-                .filter(Nicknames.canonical == alias) \
-                .one_or_none()
+        slug = self.make_identifier(alias).lower()
+        nick_id = self.get_nick_id(nick, create=True)
+        with self.session() as session:
+            result = session.execute(
+                select(Nicknames)
+                .where(Nicknames.slug == slug)
+                .where(Nicknames.canonical == alias)
+            ).scalar_one_or_none()
             if result:
                 raise ValueError('Alias already exists.')
-            nickname = Nicknames(nick_id=nick_id, slug=alias.lower(), canonical=alias)
+            nickname = Nicknames(
+                nick_id=nick_id,
+                slug=slug,
+                canonical=alias,
+            )
             session.add(nickname)
             session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def set_nick_value(self, nick, key, value):
+    def set_nick_value(self, nick: str, key: str, value: typing.Any) -> None:
         """Set or update a value in the key-value store for ``nick``.
 
-        :param str nick: the nickname with which to associate the ``value``
-        :param str key: the name by which this ``value`` may be accessed later
-        :param mixed value: the value to set for this ``key`` under ``nick``
+        :param nick: the nickname with which to associate the ``value``
+        :param key: the name by which this ``value`` may be accessed later
+        :param value: the value to set for this ``key`` under ``nick``
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         The ``value`` can be any of a range of types; it need not be a string.
         It will be serialized to JSON before being stored and decoded
         transparently upon retrieval.
 
         .. seealso::
@@ -367,78 +460,81 @@
             To retrieve a value set with this method, use
             :meth:`get_nick_value`.
 
             To delete a value set with this method, use
             :meth:`delete_nick_value`.
 
         """
-        nick = Identifier(nick)
         value = json.dumps(value, ensure_ascii=False)
-        nick_id = self.get_nick_id(nick)
-        session = self.ssession()
-        try:
-            result = session.query(NickValues) \
-                .filter(NickValues.nick_id == nick_id) \
-                .filter(NickValues.key == key) \
-                .one_or_none()
+        nick_id = self.get_nick_id(nick, create=True)
+        with self.session() as session:
+            result = session.execute(
+                select(NickValues)
+                .where(NickValues.nick_id == nick_id)
+                .where(NickValues.key == key)
+            ).scalar_one_or_none()
+
             # NickValue exists, update
             if result:
                 result.value = value
                 session.commit()
             # DNE - Insert
             else:
-                new_nickvalue = NickValues(nick_id=nick_id, key=key, value=value)
+                new_nickvalue = NickValues(
+                    nick_id=nick_id,
+                    key=key,
+                    value=value,
+                )
                 session.add(new_nickvalue)
                 session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def delete_nick_value(self, nick, key):
+    def delete_nick_value(self, nick: str, key: str) -> None:
         """Delete a value from the key-value store for ``nick``.
 
-        :param str nick: the nickname whose values to modify
-        :param str key: the name of the value to delete
+        :param nick: the nickname whose values to modify
+        :param key: the name of the value to delete
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. seealso::
 
             To set a value in the first place, use :meth:`set_nick_value`.
 
             To retrieve a value instead of deleting it, use
             :meth:`get_nick_value`.
 
         """
-        nick = Identifier(nick)
-        nick_id = self.get_nick_id(nick)
-        session = self.ssession()
         try:
-            result = session.query(NickValues) \
-                .filter(NickValues.nick_id == nick_id) \
-                .filter(NickValues.key == key) \
-                .one_or_none()
+            nick_id = self.get_nick_id(nick)
+        except ValueError:
+            # there's nothing to do if the nick doesn't exist
+            return
+
+        with self.session() as session:
+            result = session.execute(
+                select(NickValues)
+                .where(NickValues.nick_id == nick_id)
+                .where(NickValues.key == key)
+            ).scalar_one_or_none()
             # NickValue exists, delete
             if result:
                 session.delete(result)
                 session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def get_nick_value(self, nick, key, default=None):
+    def get_nick_value(
+        self,
+        nick: str,
+        key: str,
+        default: typing.Optional[typing.Any] = None
+    ) -> typing.Optional[typing.Any]:
         """Get a value from the key-value store for ``nick``.
 
-        :param str nick: the nickname whose values to access
-        :param str key: the name by which the desired value was saved
-        :param mixed default: value to return if ``key`` does not have a value
-                              set (optional)
+        :param nick: the nickname whose values to access
+        :param key: the name by which the desired value was saved
+        :param default: value to return if ``key`` does not have a value set
+                        (optional)
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. versionadded:: 7.0
 
             The ``default`` parameter.
 
         .. seealso::
@@ -446,94 +542,101 @@
             To set a value for later retrieval with this method, use
             :meth:`set_nick_value`.
 
             To delete a value instead of retrieving it, use
             :meth:`delete_nick_value`.
 
         """
-        nick = Identifier(nick)
-        session = self.ssession()
-        try:
-            result = session.query(NickValues) \
-                .filter(Nicknames.nick_id == NickValues.nick_id) \
-                .filter(Nicknames.slug == nick.lower()) \
-                .filter(NickValues.key == key) \
-                .one_or_none()
+        slug = self.make_identifier(nick).lower()
+        with self.session() as session:
+            result = session.execute(
+                select(NickValues)
+                .where(Nicknames.nick_id == NickValues.nick_id)
+                .where(Nicknames.slug == slug)
+                .where(NickValues.key == key)
+            ).scalar_one_or_none()
+
             if result is not None:
                 result = result.value
             elif default is not None:
                 result = default
+
             return _deserialize(result)
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def unalias_nick(self, alias):
+    def unalias_nick(self, alias: str) -> None:
         """Remove an alias.
 
-        :param str alias: an alias with at least one other nick in its group
-        :raise ValueError: if there is not at least one other nick in the group
+        :param alias: an alias with at least one other nick in its group
+        :raise ValueError: if there is not at least one other nick in the
+                           group, or the ``alias`` is not known
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. seealso::
 
-            To delete an entire group, use :meth:`delete_nick_group`.
+            To delete an entire group, use :meth:`forget_nick_group`.
 
             To *add* an alias for a nick, use :meth:`alias_nick`.
 
         """
-        alias = Identifier(alias)
-        nick_id = self.get_nick_id(alias, False)
-        session = self.ssession()
-        try:
-            count = session.query(Nicknames) \
-                .filter(Nicknames.nick_id == nick_id) \
-                .count()
+        slug = self.make_identifier(alias).lower()
+        nick_id = self.get_nick_id(alias)
+        with self.session() as session:
+            count = session.scalar(
+                select(func.count()).select_from(Nicknames)
+                .where(Nicknames.nick_id == nick_id)
+            )
             if count <= 1:
                 raise ValueError('Given alias is the only entry in its group.')
-            session.query(Nicknames).filter(Nicknames.slug == alias.lower()).delete()
+            session.execute(
+                delete(Nicknames)
+                .where(Nicknames.slug == slug)
+                .execution_options(synchronize_session="fetch")
+            )
             session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def delete_nick_group(self, nick):
+    def forget_nick_group(self, nick: str) -> None:
         """Remove a nickname, all of its aliases, and all of its stored values.
 
-        :param str nick: one of the nicknames in the group to be deleted
+        :param nick: one of the nicknames in the group to be deleted
+        :raise ValueError: if the ``nick`` does not exist in the database
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. important::
 
             This is otherwise known as The Nuclear Option. Be *very* sure that
             you want to do this.
 
         """
-        nick = Identifier(nick)
-        nick_id = self.get_nick_id(nick, False)
-        session = self.ssession()
-        try:
-            session.query(Nicknames).filter(Nicknames.nick_id == nick_id).delete()
-            session.query(NickValues).filter(NickValues.nick_id == nick_id).delete()
+        nick_id = self.get_nick_id(nick)
+        with self.session() as session:
+            session.execute(
+                delete(Nicknames)
+                .where(Nicknames.nick_id == nick_id)
+                .execution_options(synchronize_session="fetch")
+            )
+            session.execute(
+                delete(NickValues)
+                .where(NickValues.nick_id == nick_id)
+                .execution_options(synchronize_session="fetch")
+            )
             session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def merge_nick_groups(self, first_nick, second_nick):
+    @deprecated(
+        version='8.0',
+        removed_in='9.0',
+        reason="Renamed to `forget_nick_group`",
+    )
+    def delete_nick_group(self, nick: str) -> None:  # pragma: nocover
+        self.forget_nick_group(nick)
+
+    def merge_nick_groups(self, first_nick: str, second_nick: str):
         """Merge two nick groups.
 
-        :param str first_nick: one nick in the first group to merge
-        :param str second_nick: one nick in the second group to merge
+        :param first_nick: one nick in the first group to merge
+        :param second_nick: one nick in the second group to merge
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         Takes two nicks, which may or may not be registered. Unregistered nicks
         will be registered. Keys which are set for only one of the given nicks
         will be preserved. Where both nicks have values for a given key, the
         value set for the ``first_nick`` will be used.
 
@@ -541,85 +644,85 @@
         than one nickname can be created with this function, or by using
         :meth:`alias_nick` to add aliases.
 
         Note that merging of data only applies to the native key-value store.
         Plugins which define their own tables relying on the nick table will
         need to handle their own merging separately.
         """
-        first_id = self.get_nick_id(Identifier(first_nick))
-        second_id = self.get_nick_id(Identifier(second_nick))
-        session = self.ssession()
-        try:
+        first_id = self.get_nick_id(first_nick, create=True)
+        second_id = self.get_nick_id(second_nick, create=True)
+        with self.session() as session:
             # Get second_id's values
-            res = session.query(NickValues).filter(NickValues.nick_id == second_id).all()
+            results = session.execute(
+                select(NickValues).where(NickValues.nick_id == second_id)
+            ).scalars()
+
             # Update first_id with second_id values if first_id doesn't have that key
-            for row in res:
-                first_res = session.query(NickValues) \
-                    .filter(NickValues.nick_id == first_id) \
-                    .filter(NickValues.key == row.key) \
-                    .one_or_none()
+            for row in results:
+                first_res = session.execute(
+                    select(NickValues)
+                    .where(NickValues.nick_id == first_id)
+                    .where(NickValues.key == row.key)
+                ).scalar_one_or_none()
+
                 if not first_res:
-                    self.set_nick_value(first_nick, row.key, _deserialize(row.value))
-            session.query(NickValues).filter(NickValues.nick_id == second_id).delete()
-            session.query(Nicknames) \
-                .filter(Nicknames.nick_id == second_id) \
-                .update({'nick_id': first_id})
+                    self.set_nick_value(
+                        first_nick, row.key, _deserialize(row.value))
+
+            session.execute(
+                delete(NickValues)
+                .where(NickValues.nick_id == second_id)
+                .execution_options(synchronize_session="fetch")
+            )
+            session.execute(
+                update(Nicknames)
+                .where(Nicknames.nick_id == second_id)
+                .values(nick_id=first_id)
+                .execution_options(synchronize_session="fetch")
+            )
             session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
     # CHANNEL FUNCTIONS
 
-    def get_channel_slug(self, chan):
+    def get_channel_slug(self, chan: str) -> str:
         """Return the case-normalized representation of ``channel``.
 
-        :param str channel: the channel name to normalize, with prefix
-                            (required)
-        :return str: the case-normalized channel name (or "slug"
-                     representation)
+        :param channel: the channel name to normalize, with prefix (required)
+        :return: the case-normalized channel name (or "slug" representation)
 
         This is useful to make sure that a channel name is stored consistently
         in both the bot's own database and third-party plugins'
         databases/files, without regard for variation in case between
         different clients and/or servers on the network.
         """
-        chan = Identifier(chan)
-        slug = chan.lower()
-        session = self.ssession()
-        try:
-            count = session.query(ChannelValues) \
-                .filter(ChannelValues.channel == slug) \
-                .count()
+        slug = self.make_identifier(chan).lower()
 
-            if count == 0:
-                # see if it needs case-mapping migration
-                old_rows = session.query(ChannelValues) \
-                    .filter(ChannelValues.channel == Identifier._lower_swapped(chan))
-                old_count = old_rows.count()
-                if old_count > 0:
-                    # it does!
-                    old_rows.update({ChannelValues.channel: slug})
-                    session.commit()
+        with self.session() as session:
+            # Always migrate from old casemapping
+            session.execute(
+                update(ChannelValues)
+                .where(ChannelValues.channel == Identifier._lower_swapped(chan))
+                .values(channel=slug)
+                .execution_options(synchronize_session="fetch")
+            )
+            session.commit()
 
-            return slug
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
+        return slug
 
-    def set_channel_value(self, channel, key, value):
+    def set_channel_value(
+        self,
+        channel: str,
+        key: str,
+        value: typing.Any,
+    ) -> None:
         """Set or update a value in the key-value store for ``channel``.
 
-        :param str channel: the channel with which to associate the ``value``
-        :param str key: the name by which this ``value`` may be accessed later
-        :param mixed value: the value to set for this ``key`` under ``channel``
+        :param channel: the channel with which to associate the ``value``
+        :param key: the name by which this ``value`` may be accessed later
+        :param value: the value to set for this ``key`` under ``channel``
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         The ``value`` can be any of a range of types; it need not be a string.
         It will be serialized to JSON before being stored and decoded
         transparently upon retrieval.
 
         .. seealso::
@@ -629,74 +732,73 @@
 
             To delete a value set with this method, use
             :meth:`delete_channel_value`.
 
         """
         channel = self.get_channel_slug(channel)
         value = json.dumps(value, ensure_ascii=False)
-        session = self.ssession()
-        try:
-            result = session.query(ChannelValues) \
-                .filter(ChannelValues.channel == channel)\
-                .filter(ChannelValues.key == key) \
-                .one_or_none()
+        with self.session() as session:
+            result = session.execute(
+                select(ChannelValues)
+                .where(ChannelValues.channel == channel)
+                .where(ChannelValues.key == key)
+            ).scalar_one_or_none()
+
             # ChannelValue exists, update
             if result:
                 result.value = value
                 session.commit()
             # DNE - Insert
             else:
-                new_channelvalue = ChannelValues(channel=channel, key=key, value=value)
+                new_channelvalue = ChannelValues(
+                    channel=channel,
+                    key=key,
+                    value=value,
+                )
                 session.add(new_channelvalue)
                 session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def delete_channel_value(self, channel, key):
+    def delete_channel_value(self, channel: str, key: str) -> None:
         """Delete a value from the key-value store for ``channel``.
 
-        :param str channel: the channel whose values to modify
-        :param str key: the name of the value to delete
+        :param channel: the channel whose values to modify
+        :param key: the name of the value to delete
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. seealso::
 
             To set a value in the first place, use :meth:`set_channel_value`.
 
             To retrieve a value instead of deleting it, use
             :meth:`get_channel_value`.
 
         """
         channel = self.get_channel_slug(channel)
-        session = self.ssession()
-        try:
-            result = session.query(ChannelValues) \
-                .filter(ChannelValues.channel == channel)\
-                .filter(ChannelValues.key == key) \
-                .one_or_none()
-            # ChannelValue exists, delete
-            if result:
-                session.delete(result)
-                session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
+        with self.session() as session:
+            session.execute(
+                delete(ChannelValues)
+                .where(
+                    ChannelValues.channel == channel,
+                    ChannelValues.key == key
+                ).execution_options(synchronize_session="fetch")
+            )
+            session.commit()
 
-    def get_channel_value(self, channel, key, default=None):
+    def get_channel_value(
+        self,
+        channel: str,
+        key: str,
+        default: typing.Optional[typing.Any] = None,
+    ):
         """Get a value from the key-value store for ``channel``.
 
-        :param str channel: the channel whose values to access
-        :param str key: the name by which the desired value was saved
-        :param mixed default: value to return if ``key`` does not have a value
-                              set (optional)
+        :param channel: the channel whose values to access
+        :param key: the name by which the desired value was saved
+        :param default: value to return if ``key`` does not have a value set
+                        (optional)
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. versionadded:: 7.0
 
             The ``default`` parameter.
 
         .. seealso::
@@ -705,39 +807,58 @@
             :meth:`set_channel_value`.
 
             To delete a value instead of retrieving it, use
             :meth:`delete_channel_value`.
 
         """
         channel = self.get_channel_slug(channel)
-        session = self.ssession()
-        try:
-            result = session.query(ChannelValues) \
-                .filter(ChannelValues.channel == channel)\
-                .filter(ChannelValues.key == key) \
-                .one_or_none()
+        with self.session() as session:
+            result = session.execute(
+                select(ChannelValues)
+                .where(ChannelValues.channel == channel)
+                .where(ChannelValues.key == key)
+            ).scalar_one_or_none()
             if result is not None:
                 result = result.value
             elif default is not None:
                 result = default
             return _deserialize(result)
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
+
+    def forget_channel(self, channel: str) -> None:
+        """Remove all of a channel's stored values.
+
+        :param channel: the name of the channel for which to delete values
+        :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
+
+        .. important::
+
+            This is a Nuclear Option. Be *very* sure that you want to do it.
+
+        """
+        channel = self.get_channel_slug(channel)
+        with self.session() as session:
+            session.execute(
+                delete(ChannelValues)
+                .where(ChannelValues.channel == channel)
+            )
+            session.commit()
 
     # PLUGIN FUNCTIONS
 
-    def set_plugin_value(self, plugin, key, value):
+    def set_plugin_value(
+        self,
+        plugin: str,
+        key: str,
+        value: typing.Any,
+    ) -> None:
         """Set or update a value in the key-value store for ``plugin``.
 
-        :param str plugin: the plugin name with which to associate the ``value``
-        :param str key: the name by which this ``value`` may be accessed later
-        :param mixed value: the value to set for this ``key`` under ``plugin``
+        :param plugin: the plugin name with which to associate the ``value``
+        :param key: the name by which this ``value`` may be accessed later
+        :param value: the value to set for this ``key`` under ``plugin``
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         The ``value`` can be any of a range of types; it need not be a string.
         It will be serialized to JSON before being stored and decoded
         transparently upon retrieval.
 
         .. seealso::
@@ -747,74 +868,69 @@
 
             To delete a value set with this method, use
             :meth:`delete_plugin_value`.
 
         """
         plugin = plugin.lower()
         value = json.dumps(value, ensure_ascii=False)
-        session = self.ssession()
-        try:
-            result = session.query(PluginValues) \
-                .filter(PluginValues.plugin == plugin)\
-                .filter(PluginValues.key == key) \
-                .one_or_none()
+        with self.session() as session:
+            result = session.execute(
+                select(PluginValues)
+                .where(PluginValues.plugin == plugin)
+                .where(PluginValues.key == key)
+            ).scalar_one_or_none()
             # PluginValue exists, update
             if result:
                 result.value = value
                 session.commit()
             # DNE - Insert
             else:
                 new_pluginvalue = PluginValues(plugin=plugin, key=key, value=value)
                 session.add(new_pluginvalue)
                 session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def delete_plugin_value(self, plugin, key):
+    def delete_plugin_value(self, plugin: str, key: str) -> None:
         """Delete a value from the key-value store for ``plugin``.
 
-        :param str plugin: the plugin name whose values to modify
-        :param str key: the name of the value to delete
+        :param plugin: the plugin name whose values to modify
+        :param key: the name of the value to delete
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. seealso::
 
             To set a value in the first place, use :meth:`set_plugin_value`.
 
             To retrieve a value instead of deleting it, use
             :meth:`get_plugin_value`.
 
         """
         plugin = plugin.lower()
-        session = self.ssession()
-        try:
-            result = session.query(PluginValues) \
-                .filter(PluginValues.plugin == plugin)\
-                .filter(PluginValues.key == key) \
-                .one_or_none()
+        with self.session() as session:
+            result = session.execute(
+                select(PluginValues)
+                .where(PluginValues.plugin == plugin)
+                .where(PluginValues.key == key)
+            ).scalar_one_or_none()
             # PluginValue exists, update
             if result:
                 session.delete(result)
                 session.commit()
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
 
-    def get_plugin_value(self, plugin, key, default=None):
+    def get_plugin_value(
+        self,
+        plugin: str,
+        key: str,
+        default: typing.Optional[typing.Any] = None,
+    ) -> typing.Optional[typing.Any]:
         """Get a value from the key-value store for ``plugin``.
 
-        :param str plugin: the plugin name whose values to access
-        :param str key: the name by which the desired value was saved
-        :param mixed default: value to return if ``key`` does not have a value
-                              set (optional)
+        :param plugin: the plugin name whose values to access
+        :param key: the name by which the desired value was saved
+        :param default: value to return if ``key`` does not have a value set
+                        (optional)
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. versionadded:: 7.0
 
             The ``default`` parameter.
 
         .. seealso::
@@ -823,40 +939,59 @@
             :meth:`set_plugin_value`.
 
             To delete a value instead of retrieving it, use
             :meth:`delete_plugin_value`.
 
         """
         plugin = plugin.lower()
-        session = self.ssession()
-        try:
-            result = session.query(PluginValues) \
-                .filter(PluginValues.plugin == plugin)\
-                .filter(PluginValues.key == key) \
-                .one_or_none()
+        with self.session() as session:
+            result = session.execute(
+                select(PluginValues)
+                .where(PluginValues.plugin == plugin)
+                .where(PluginValues.key == key)
+            ).scalar_one_or_none()
+
             if result is not None:
                 result = result.value
             elif default is not None:
                 result = default
             return _deserialize(result)
-        except SQLAlchemyError:
-            session.rollback()
-            raise
-        finally:
-            self.ssession.remove()
+
+    def forget_plugin(self, plugin: str) -> None:
+        """Remove all of a plugin's stored values.
+
+        :param plugin: the name of the plugin for which to delete values
+        :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
+
+        .. important::
+
+            This is a Nuclear Option. Be *very* sure that you want to do it.
+
+        """
+        plugin = plugin.lower()
+        with self.session() as session:
+            session.execute(
+                delete(PluginValues).where(PluginValues.plugin == plugin)
+            )
+            session.commit()
 
     # NICK AND CHANNEL FUNCTIONS
 
-    def get_nick_or_channel_value(self, name, key, default=None):
+    def get_nick_or_channel_value(
+        self,
+        name: str,
+        key: str,
+        default=None
+    ) -> typing.Optional[typing.Any]:
         """Get a value from the key-value store for ``name``.
 
-        :param str name: nick or channel whose values to access
-        :param str key: the name by which the desired value was saved
-        :param mixed default: value to return if ``key`` does not have a value
-                              set (optional)
+        :param name: nick or channel whose values to access
+        :param key: the name by which the desired value was saved
+        :param default: value to return if ``key`` does not have a value set
+                        (optional)
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         .. versionadded:: 7.0
 
             The ``default`` parameter.
 
         This is useful for common logic that is shared between both users and
@@ -867,25 +1002,33 @@
 
             To get a value for a nick specifically, use :meth:`get_nick_value`.
 
             To get a value for a channel specifically, use
             :meth:`get_channel_value`.
 
         """
-        name = Identifier(name)
-        if name.is_nick():
-            return self.get_nick_value(name, key, default)
+        if not isinstance(name, Identifier):
+            identifier = self.make_identifier(name)
+        else:
+            identifier = typing.cast('Identifier', name)
+
+        if identifier.is_nick():
+            return self.get_nick_value(identifier, key, default)
         else:
-            return self.get_channel_value(name, key, default)
+            return self.get_channel_value(identifier, key, default)
 
-    def get_preferred_value(self, names, key):
+    def get_preferred_value(
+        self,
+        names: Iterable[str],
+        key: str,
+    ) -> typing.Optional[typing.Any]:
         """Get a value for the first name which has it set.
 
-        :param list names: a list of channel names and/or nicknames
-        :param str key: the name by which the desired value was saved
+        :param names: a list of channel names and/or nicknames
+        :param key: the name by which the desired value was saved
         :return: the value for ``key`` from the first ``name`` which has it set,
                  or ``None`` if none of the ``names`` has it set
         :raise ~sqlalchemy.exc.SQLAlchemyError: if there is a database error
 
         This is useful for logic that needs to customize its output based on
         settings stored in the database. For example, it can be used to fall
         back from the triggering user's setting to the current channel's setting
@@ -898,7 +1041,10 @@
             might have ``None`` as a valid value, to avoid ambiguous logic.
 
         """
         for name in names:
             value = self.get_nick_or_channel_value(name, key)
             if value is not None:
                 return value
+
+        # Explicit return for type check
+        return None
```

### Comparing `sopel-7.1.9/sopel/formatting.py` & `sopel-8.0.0/sopel/formatting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-# coding=utf-8
 """The formatting module includes functions to apply IRC formatting to text.
 
 *Availability: 4.5+*
 """
 # Copyright 2014, Elsie Powell, embolalia.com
 # Copyright 2019, dgw, technobabbl.es
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+from enum import Enum
 import re
 import string
-import sys
 
 
 __all__ = [
     # control chars
     'CONTROL_NORMAL',
     'CONTROL_COLOR',
     'CONTROL_HEX_COLOR',
     'CONTROL_BOLD',
     'CONTROL_ITALIC',
     'CONTROL_UNDERLINE',
     'CONTROL_STRIKETHROUGH',
     'CONTROL_MONOSPACE',
     'CONTROL_REVERSE',
+    # convenience lists
+    'CONTROL_FORMATTING',
+    'CONTROL_NON_PRINTING',
     # utility functions
     'color',
     'hex_color',
     'bold',
     'italic',
     'underline',
     'strikethrough',
     'monospace',
     'reverse',
     'plain',
-    # utility class
+    # utility enum
     'colors',
 ]
 
-if sys.version_info.major >= 3:
-    unicode = str
-
 # Color names are as specified at http://www.mirc.com/colors.html
 
 CONTROL_NORMAL = '\x0f'
 """The control code to reset formatting."""
 CONTROL_COLOR = '\x03'
 """The control code to start or end color formatting."""
 CONTROL_HEX_COLOR = '\x04'
@@ -124,60 +123,63 @@
 PLAIN_PATTERN = '|'.join([
     '(' + COLOR_PATTERN + ')',
     '(' + HEX_COLOR_PATTERN + ')',
 ])
 PLAIN_REGEX = re.compile(PLAIN_PATTERN)
 
 
-# TODO when we can move to 3.3+ completely, make this an Enum.
-class colors:
+class colors(str, Enum):
+    """Mapping of color names to mIRC code values."""
+    # Mostly aligned with https://modern.ircdocs.horse/formatting.html#colors
+    # which are likely based on mIRC's color names (https://www.mirc.com/colors.html)
     WHITE = '00'
     BLACK = '01'
     BLUE = '02'
-    NAVY = BLUE
     GREEN = '03'
-    RED = '04'
+    LIGHT_RED = '04'
     BROWN = '05'
-    MAROON = BROWN
     PURPLE = '06'
     ORANGE = '07'
-    OLIVE = ORANGE
     YELLOW = '08'
     LIGHT_GREEN = '09'
-    LIME = LIGHT_GREEN
-    TEAL = '10'
+    TEAL = '10'  # TODO: should be called 'CYAN'
     LIGHT_CYAN = '11'
-    CYAN = LIGHT_CYAN
     LIGHT_BLUE = '12'
-    ROYAL = LIGHT_BLUE
     PINK = '13'
-    LIGHT_PURPLE = PINK
-    FUCHSIA = PINK
     GREY = '14'
     LIGHT_GREY = '15'
-    SILVER = LIGHT_GREY
 
     # Create aliases.
+    NAVY = BLUE
+    RED = LIGHT_RED
+    MAROON = BROWN
+    OLIVE = ORANGE  # TODO: held over from antiquity; does anyone actually think this?
+    LIME = LIGHT_GREEN
+    CYAN = LIGHT_CYAN  # TODO: should be what is called 'TEAL' above
+    ROYAL = LIGHT_BLUE
+    LIGHT_PURPLE = PINK
+    FUCHSIA = PINK
     GRAY = GREY
     LIGHT_GRAY = LIGHT_GREY
+    SILVER = LIGHT_GREY
 
 
 def _get_color(color):
     if color is None:
         return None
 
     # You can pass an int or string of the code
     try:
         color = int(color)
     except ValueError:
         pass
     if isinstance(color, int):
         if color > 99:
             raise ValueError('Can not specify a color above 99.')
-        return unicode(color).rjust(2, '0')
+        return str(color).rjust(2, '0')
 
     # You can also pass the name of the color
     color_name = color.upper()
     color_dict = colors.__dict__
     try:
         return color_dict[color_name]
     except KeyError:
@@ -186,20 +188,23 @@
 
 def color(text, fg=None, bg=None):
     """Return the text, with the given colors applied in IRC formatting.
 
     :param str text: the text to format
     :param mixed fg: the foreground color
     :param mixed bg: the background color
+    :raises TypeError: if ``text`` is not a string
+    :raises ValueError: if ``fg`` or ``bg`` is an unrecognized color value
+    :rtype: str
 
     The color can be a string of the color name, or an integer in the range
     0-99. The known color names can be found in the :class:`colors` class of
     this module.
     """
-    if not fg and not bg:
+    if fg is None and bg is None:
         return text
 
     fg = _get_color(fg)
     bg = _get_color(bg)
 
     if not bg:
         text = ''.join([CONTROL_COLOR, fg, text, CONTROL_COLOR])
@@ -229,22 +234,25 @@
 
 def hex_color(text, fg=None, bg=None):
     """Return the text, with the given colors applied in IRC formatting.
 
     :param str text: the text to format
     :param str fg: the foreground color
     :param str bg: the background color
+    :raises TypeError: if ``text`` is not a string
+    :raises ValueError: if ``fg`` or ``bg`` is an unrecognized color value
+    :rtype: str
 
     The color can be provided with a string of either 3 or 6 hexadecimal digits.
     As in CSS, 3-digit colors will be interpreted as if they were 6-digit colors
     with each digit repeated (e.g. color ``c90`` is identical to ``cc9900``). Do
     not include the leading ``#`` symbol.
 
     .. note::
-        This is a relatively new IRC formatting convention. Use only when you
+        This is a relatively new IRC formatting convention. Use it only when you
         can afford to have its meaning lost, as not many clients support it yet.
     """
     if not fg and not bg:
         return text
 
     fg = _get_hex_color(fg)
     bg = _get_hex_color(bg)
@@ -256,72 +264,85 @@
     return text
 
 
 def bold(text):
     """Return the text, with bold IRC formatting.
 
     :param str text: the text to format
+    :raises TypeError: if ``text`` is not a string
+    :rtype: str
     """
     return ''.join([CONTROL_BOLD, text, CONTROL_BOLD])
 
 
 def italic(text):
     """Return the text, with italic IRC formatting.
 
     :param str text: the text to format
+    :raises TypeError: if ``text`` is not a string
+    :rtype: str
     """
     return ''.join([CONTROL_ITALIC, text, CONTROL_ITALIC])
 
 
 def underline(text):
     """Return the text, with underline IRC formatting.
 
     :param str text: the text to format
+    :raises TypeError: if ``text`` is not a string
+    :rtype: str
     """
     return ''.join([CONTROL_UNDERLINE, text, CONTROL_UNDERLINE])
 
 
 def strikethrough(text):
     """Return the text, with strikethrough IRC formatting.
 
     :param str text: the text to format
+    :raises TypeError: if ``text`` is not a string
+    :rtype: str
 
     .. note::
-        This is a relatively new IRC formatting convention. Use only when you
+        This is a relatively new IRC formatting convention. Use it only when you
         can afford to have its meaning lost, as not many clients support it yet.
     """
     return ''.join([CONTROL_STRIKETHROUGH, text, CONTROL_STRIKETHROUGH])
 
 
 def monospace(text):
     """Return the text, with monospace IRC formatting.
 
     :param str text: the text to format
+    :raises TypeError: if ``text`` is not a string
+    :rtype: str
 
     .. note::
-        This is a relatively new IRC formatting convention. Use only when you
+        This is a relatively new IRC formatting convention. Use it only when you
         can afford to have its meaning lost, as not many clients support it yet.
     """
     return ''.join([CONTROL_MONOSPACE, text, CONTROL_MONOSPACE])
 
 
 def reverse(text):
     """Return the text, with reverse-color IRC formatting.
 
     :param str text: the text to format
+    :raises TypeError: if ``text`` is not a string
+    :rtype: str
 
     .. note::
         This code isn't super well supported, and its behavior even in clients
         that understand it (e.g. mIRC) can be unpredictable. Use it carefully.
     """
     return ''.join([CONTROL_REVERSE, text, CONTROL_REVERSE])
 
 
 def plain(text):
     """Return the text without any IRC formatting.
 
     :param str text: text with potential IRC formatting control code(s)
+    :raises TypeError: if ``text`` is not a string
     :rtype: str
     """
     if '\x03' in text or '\x04' in text:
         text = PLAIN_REGEX.sub('', text)
     return ''.join(c for c in text if ord(c) >= 0x20 and c != '\x7F')
```

### Comparing `sopel-7.1.9/sopel/irc/__init__.py` & `sopel-8.0.0/sopel/irc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,397 @@
-# coding=utf-8
 """:mod:`sopel.irc` is the core IRC module for Sopel.
 
 This sub-package contains everything that is related to the IRC protocol
 (connection, commands, abstract client, etc.) and that can be used to implement
 the Sopel bot.
 
 In particular, it defines the interface for the IRC backend
 (:class:`~sopel.irc.abstract_backends.AbstractIRCBackend`), and the
-interface for the bot itself (:class:`~sopel.irc.AbstractBot`). This is all
-internal code that isn't supposed to be used directly by a plugin developer,
-who should worry about :class:`sopel.bot.Sopel` only.
+interface for the bot itself (:class:`~sopel.irc.AbstractBot`).
+
+.. warning::
+
+    This is all internal code, not intended for direct use by plugins. It is
+    subject to change between versions, even patch releases, without any
+    advance warning.
+
+    Please use the public APIs on :class:`bot <sopel.bot.Sopel>`.
 
 .. important::
 
     When working on core IRC protocol related features, consult protocol
-    documentation at https://www.irchelp.org/protocol/rfc/
+    documentation at https://modern.ircdocs.horse/
 
 """
 # Copyright 2008, Sean B. Palmer, inamidst.com
 # Copyright 2012, Elsie Powell, http://embolalia.com
 # Copyright © 2012, Elad Alfassa <elad@fedoraproject.org>
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-from datetime import datetime
+import abc
+from collections import deque
+from datetime import datetime, timezone
 import logging
 import os
-import sys
 import threading
 import time
-
-try:
-    import ssl
-    if not hasattr(ssl, 'match_hostname'):
-        # Attempt to import ssl_match_hostname from python-backports
-        # TODO: Remove when dropping Python 2 support
-        import backports.ssl_match_hostname
-        ssl.match_hostname = backports.ssl_match_hostname.match_hostname
-        ssl.CertificateError = backports.ssl_match_hostname.CertificateError
-    has_ssl = True
-except ImportError:
-    # no SSL support
-    has_ssl = False
+from typing import (
+    Any,
+    Optional,
+    TYPE_CHECKING,
+)
 
 from sopel import tools, trigger
-from .backends import AsynchatBackend, SSLAsynchatBackend
+from sopel.lifecycle import deprecated
+from sopel.tools import identifiers, memories
+from .backends import AsyncioBackend, UninitializedBackend
+from .capabilities import Capabilities
 from .isupport import ISupport
-from .utils import CapReq, safe
 
-if sys.version_info.major >= 3:
-    unicode = str
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+    from sopel.config import Config
+    from .abstract_backends import AbstractIRCBackend
+    from .utils import MyInfo
+
 
 __all__ = ['abstract_backends', 'backends', 'utils']
 
 LOGGER = logging.getLogger(__name__)
+ERR_BACKEND_NOT_INITIALIZED = 'Backend not initialized; is the bot running?'
 
 
-class AbstractBot(object):
+class AbstractBot(abc.ABC):
     """Abstract definition of Sopel's interface."""
-    def __init__(self, settings):
+    def __init__(self, settings: Config):
         # private properties: access as read-only properties
-        self._nick = tools.Identifier(settings.core.nick)
-        self._user = settings.core.user
-        self._name = settings.core.name
+        self._user: str = settings.core.user
+        self._name: str = settings.core.name
         self._isupport = ISupport()
-        self._myinfo = None
-
-        self.backend = None
-        """IRC connection backend."""
-        self.connection_registered = False
+        self._capabilities = Capabilities()
+        self._myinfo: Optional[MyInfo] = None
+        self._nick: identifiers.Identifier = self.make_identifier(
+            settings.core.nick)
+
+        self.backend: AbstractIRCBackend = UninitializedBackend(self)
+        """IRC Connection Backend."""
+        self._connection_registered = threading.Event()
         """Flag stating whether the IRC Connection is registered yet."""
         self.settings = settings
         """Bot settings."""
-        self.enabled_capabilities = set()
-        """A set containing the IRCv3 capabilities that the bot has enabled."""
-        self._cap_reqs = dict()
-        """A dictionary of capability names to a list of requests."""
 
         # internal machinery
         self.sending = threading.RLock()
-        self.last_error_timestamp = None
+        self.last_error_timestamp: Optional[datetime] = None
         self.error_count = 0
-        self.stack = {}
+        self.stack: dict[identifiers.Identifier, dict[str, Any]] = {}
         self.hasquit = False
+        self.wantsrestart = False
         self.last_raw_line = ''  # last raw line received
 
     @property
-    def nick(self):
+    def connection_registered(self) -> bool:
+        """Whether the IRC connection is registered.
+
+        This is a property so it can accurately reflect not only the socket
+        state (connection to IRC server), but also whether the connection is
+        ready to accept "normal" IRC commands.
+
+        Before registration is completed, only a very limited set of commands
+        are allowed to be used. Sopel itself takes care of these, so plugins
+        will be more concerned with whether they are allowed to use methods
+        like :meth:`say` yet.
+        """
+        return (
+            self.backend is not None
+            and self.backend.is_connected()
+            and self._connection_registered.is_set())
+
+    @property
+    def nick(self) -> identifiers.Identifier:
         """Sopel's current nick.
 
         Changing this while Sopel is running is unsupported and can result in
         undefined behavior.
         """
         return self._nick
 
     @property
-    def user(self):
+    def user(self) -> str:
         """Sopel's user/ident."""
         return self._user
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Sopel's "real name", as used for WHOIS responses."""
         return self._name
 
     @property
-    def config(self):
+    def config(self) -> Config:
         """The :class:`sopel.config.Config` for the current Sopel instance."""
         # TODO: Deprecate config, replaced by settings
         return self.settings
 
     @property
-    def isupport(self):
+    def capabilities(self) -> Capabilities:
+        """Capabilities negotiated with the server."""
+        return self._capabilities
+
+    @property
+    @deprecated(
+        reason='Capability handling has been rewritten. '
+        'Use `bot.capabilities.is_enabled()` or `bot.capabilities.enabled` instead.',
+        version='8.0',
+        warning_in='8.1',
+        removed_in='9.0',
+    )
+    def enabled_capabilities(self) -> set[str]:
+        """A set containing the IRCv3 capabilities that the bot has enabled.
+
+        .. deprecated:: 8.0
+
+            Enabled server capabilities are now managed by
+            :attr:`bot.capabilities <capabilities>` and its various methods and
+            attributes:
+
+            * use :meth:`bot.capabilities.is_enabled() <sopel.irc.capabilities.Capabilities.is_enabled>`
+              to check if a capability is enabled
+            * use :attr:`bot.capabilities.enabled <sopel.irc.capabilities.Capabilities.enabled>`
+              for a list of enabled capabilities
+
+            Will be removed in Sopel 9.
+
+        """
+        return set(self._capabilities.enabled)
+
+    @property
+    @deprecated(
+        reason='Capability handling has been rewritten. '
+        'Use `bot.capabilities.is_available()` or `bot.capabilities.available` instead.',
+        version='8.0',
+        warning_in='8.1',
+        removed_in='9.0',
+    )
+    def server_capabilities(self) -> dict[str, Optional[str]]:
+        """A dict mapping supported IRCv3 capabilities to their options.
+
+        For example, if the server specifies the capability ``sasl=EXTERNAL``,
+        it will be here as ``{"sasl": "EXTERNAL"}``. Capabilities specified
+        without any options will have ``None`` as the value.
+
+        For servers that do not support IRCv3, this will be an empty set.
+
+        .. deprecated:: 8.0
+
+            Enabled server capabilities are now managed by
+            :attr:`bot.capabilities <capabilities>` and its various methods and
+            attributes:
+
+            * use :meth:`bot.capabilities.is_available() <sopel.irc.capabilities.Capabilities.is_available>`
+              to check if a capability is available
+            * use :attr:`bot.capabilities.available <sopel.irc.capabilities.Capabilities.available>`
+              for a list of available capabilities and their parameters
+
+            Will be removed in Sopel 9.
+
+        """
+        return self._capabilities.available
+
+    @property
+    def isupport(self) -> ISupport:
         """Features advertised by the server.
 
         :type: :class:`~.isupport.ISupport` instance
         """
         return self._isupport
 
     @property
-    def myinfo(self):
+    def myinfo(self) -> MyInfo:
         """Server/network information.
 
         :type: :class:`~.utils.MyInfo` instance
 
         .. versionadded:: 7.0
         """
         if self._myinfo is None:
             raise AttributeError('myinfo')
         return self._myinfo
 
+    @property
+    @abc.abstractmethod
+    def hostmask(self) -> Optional[str]:
+        """The bot's hostmask."""
+
+    # Utility
+
+    def make_identifier(self, name: str) -> identifiers.Identifier:
+        """Instantiate an Identifier using the bot's context.
+
+        .. versionadded:: 8.0
+        """
+        casemapping = {
+            'ascii': identifiers.ascii_lower,
+            'rfc1459': identifiers.rfc1459_lower,
+            'rfc1459-strict': identifiers.rfc1459_strict_lower,
+        }.get(self.isupport.get('CASEMAPPING'), identifiers.rfc1459_lower)
+        chantypes = (
+            self.isupport.get('CHANTYPES', identifiers.DEFAULT_CHANTYPES))
+
+        return identifiers.Identifier(
+            name,
+            casemapping=casemapping,
+            chantypes=chantypes,
+        )
+
+    def make_identifier_memory(self) -> memories.SopelIdentifierMemory:
+        """Instantiate a SopelIdentifierMemory using the bot's context.
+
+        This is a shortcut for :class:`~.memories.SopelIdentifierMemory`\'s most
+        common use case, which requires remembering to pass the ``bot``\'s own
+        :meth:`make_identifier` method so the ``SopelIdentifierMemory`` will
+        cast its keys to :class:`~.tools.identifiers.Identifier`\\s that are
+        compatible with what the bot tracks internally and sends with
+        :class:`~.trigger.Trigger`\\s when a plugin callable runs.
+
+        Calling this method is equivalent to the following::
+
+            from sopel.tools import memories
+
+            memories.SopelIdentifierMemory(
+                identifier_factory=bot.make_identifier,
+            )
+
+        .. versionadded:: 8.0
+
+        .. seealso::
+
+            The :mod:`.tools.memories` module describes how to use
+            :class:`~.tools.memories.SopelIdentifierMemory` and its siblings.
+
+        """
+        return memories.SopelIdentifierMemory(
+            identifier_factory=self.make_identifier,
+        )
+
+    def safe_text_length(self, recipient: str) -> int:
+        """Estimate a safe text length for an IRC message.
+
+        :return: the maximum possible length of a message to ``recipient``
+
+        When the bot sends a message to a recipient (channel or nick), it has
+        512 bytes minus the command, arguments, various separators and trailing
+        CRLF for its text. However, this is not what other users will see from
+        the server; the message forwarded to other clients will be sent using
+        this format::
+
+            :nick!~user@hostname PRIVMSG #channel :text
+
+        Which takes more bytes, reducing the maximum length available for a
+        single line of text. This method computes a safe length of text that
+        can be sent using ``PRIVMSG`` or ``NOTICE`` by subtracting the size
+        required by the server to convey the bot's message.
+
+        .. seealso::
+
+            This method is useful when sending a message using :meth:`say`,
+            and can be used with :func:`sopel.tools.get_sendable_message`.
+
+        """
+        # Clients "SHOULD" assume messages will be truncated at 512 bytes if
+        # the LINELEN ISUPPORT token is not present.
+        # See https://modern.ircdocs.horse/#linelen-parameter
+        max_line_length = self.isupport.get('LINELEN', 512)
+
+        if self.hostmask is not None:
+            hostmask_length = len(self.hostmask)
+        else:
+            # calculate maximum possible length, given current nick/username
+            hostmask_length = (
+                len(self.nick)  # own nick length
+                + 1  # (! separator)
+                + 1  # (for the optional ~ in user)
+                + min(  # own ident length, capped to ISUPPORT or RFC maximum
+                    len(self.user),
+                    getattr(self.isupport, 'USERLEN', 9))
+                + 1  # (@ separator)
+                + 63  # <hostname> has a maximum length of 63 characters.
+            )
+
+        return (
+            max_line_length
+            - 1  # leading colon
+            - hostmask_length  # calculated/maximum length of own hostmask prefix
+            - 1  # space between prefix & command
+            - 7  # PRIVMSG command
+            - 1  # space before recipient
+            - len(recipient.encode('utf-8'))  # target channel/nick (can contain Unicode)
+            - 2  # space after recipient, colon before text
+            - 2  # trailing CRLF
+        )
+
     # Connection
 
-    def get_irc_backend(self):
+    def get_irc_backend(
+        self,
+        host: str,
+        port: int,
+        source_address: Optional[tuple[str, int]],
+    ) -> AbstractIRCBackend:
         """Set up the IRC backend based on the bot's settings.
 
         :return: the initialized IRC backend object
         :rtype: an object implementing the interface of
                 :class:`~sopel.irc.abstract_backends.AbstractIRCBackend`
         """
         timeout = int(self.settings.core.timeout)
         ping_interval = int(self.settings.core.timeout_ping_interval)
-        backend_class = AsynchatBackend
-        backend_args = [self]
-        backend_kwargs = {
-            'server_timeout': timeout,
-            'ping_interval': ping_interval,
-        }
-
-        if self.settings.core.use_ssl:
-            if has_ssl:
-                backend_class = SSLAsynchatBackend
-                backend_kwargs.update({
-                    'verify_ssl': self.settings.core.verify_ssl,
-                    'ca_certs': self.settings.core.ca_certs,
-                })
-            else:
-                LOGGER.warning(
-                    'SSL is not available on your system; '
-                    'attempting connection without it')
-
-        return backend_class(*backend_args, **backend_kwargs)
+        return AsyncioBackend(
+            self,
+            # connection
+            host=host,
+            port=port,
+            source_address=source_address,
+            # timeout
+            server_timeout=timeout,
+            ping_interval=ping_interval,
+            # ssl
+            use_ssl=self.settings.core.use_ssl,
+            certfile=self.settings.core.client_cert_file,
+            keyfile=self.settings.core.client_cert_file,
+            verify_ssl=self.settings.core.verify_ssl,
+            ca_certs=self.settings.core.ca_certs,
+            ssl_ciphers=self.settings.core.ssl_ciphers,
+            ssl_minimum_version=self.settings.core.ssl_minimum_version,
+        )
 
-    def run(self, host, port=6667):
+    def run(self, host: str, port: int = 6667) -> None:
         """Connect to IRC server and run the bot forever.
 
         :param str host: the IRC server hostname
         :param int port: the IRC server port
         """
         source_address = ((self.settings.core.bind_host, 0)
                           if self.settings.core.bind_host else None)
 
-        self.backend = self.get_irc_backend()
-        self.backend.initiate_connect(host, port, source_address)
+        self.backend = self.get_irc_backend(host, port, source_address)
         try:
             self.backend.run_forever()
         except KeyboardInterrupt:
             # raised only when the bot is not connected
             LOGGER.warning('Keyboard Interrupt')
             raise
 
-    def on_connect(self):
+    def on_connect(self) -> None:
         """Handle successful establishment of IRC connection."""
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         LOGGER.info('Connected, initiating setup sequence')
 
         # Request list of server capabilities. IRCv3 servers will respond with
         # CAP * LS (which we handle in coretasks). v2 servers will respond with
         # 421 Unknown command, which we'll ignore
         LOGGER.debug('Sending CAP request')
         self.backend.send_command('CAP', 'LS', '302')
@@ -201,236 +405,183 @@
             self.backend.send_pass(self.settings.core.server_auth_password)
 
         LOGGER.debug('Sending nick "%s"', self.nick)
         self.backend.send_nick(self.nick)
         LOGGER.debug('Sending user "%s" (name: "%s")', self.user, self.name)
         self.backend.send_user(self.user, '0', '*', self.name)
 
-    def on_message(self, message):
+    def on_message(self, message: str) -> None:
         """Handle an incoming IRC message.
 
         :param str message: the received raw IRC message
         """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         self.last_raw_line = message
 
         pretrigger = trigger.PreTrigger(
             self.nick,
             message,
             url_schemes=self.settings.core.auto_url_schemes,
+            identifier_factory=self.make_identifier,
+            statusmsg_prefixes=self.isupport.get('STATUSMSG'),
         )
-        if all(cap not in self.enabled_capabilities for cap in ['account-tag', 'extended-join']):
+        if all(
+            not self.capabilities.is_enabled(cap)
+            for cap in ['account-tag', 'extended-join']
+        ):
             pretrigger.tags.pop('account', None)
 
         if pretrigger.event == 'PING':
             self.backend.send_pong(pretrigger.args[-1])
         elif pretrigger.event == 'ERROR':
             LOGGER.error("ERROR received from server: %s", pretrigger.args[-1])
             self.backend.on_irc_error(pretrigger)
 
         self.dispatch(pretrigger)
 
-    def on_message_sent(self, raw):
+    def on_message_sent(self, raw: str) -> None:
         """Handle any message sent through the connection.
 
         :param str raw: raw text message sent through the connection
 
         When a message is sent through the IRC connection, the bot will log
         the raw message. If necessary, it will also simulate the
         `echo-message`_ feature of IRCv3.
 
         .. _echo-message: https://ircv3.net/irc/#echo-message
         """
         # Log raw message
         self.log_raw(raw, '>>')
 
         # Simulate echo-message
-        no_echo = 'echo-message' not in self.enabled_capabilities
+        no_echo = not self.capabilities.is_enabled('echo-message')
         echoed = ['PRIVMSG', 'NOTICE']
         if no_echo and any(raw.upper().startswith(cmd) for cmd in echoed):
             # Use the hostmask we think the IRC server is using for us,
             # or something reasonable if that's not available
             host = 'localhost'
             if self.settings.core.bind_host:
                 host = self.settings.core.bind_host
             else:
                 try:
-                    host = self.hostmask
+                    host = self.hostmask or host
                 except KeyError:
                     pass  # we tried, and that's good enough
 
             pretrigger = trigger.PreTrigger(
                 self.nick,
                 ":{0}!{1}@{2} {3}".format(self.nick, self.user, host, raw),
                 url_schemes=self.settings.core.auto_url_schemes,
+                identifier_factory=self.make_identifier,
+                statusmsg_prefixes=self.isupport.get('STATUSMSG'),
             )
             self.dispatch(pretrigger)
 
-    def on_error(self):
+    @deprecated(
+        'This method was used to log errors with asynchat; '
+        'use logging.getLogger("sopel.exception") instead.',
+        version='8.0',
+        removed_in='9.0',
+    )
+    def on_error(self) -> None:
         """Handle any uncaptured error in the bot itself."""
         LOGGER.error('Fatal error in core, please review exceptions log.')
 
         err_log = logging.getLogger('sopel.exceptions')
         err_log.error(
-            'Fatal error in core, handle_error() was called.\n'
-            'Buffer:\n%s\n'
+            'Fatal error in core, bot.on_error() was called.\n'
             'Last Line:\n%s',
-            self.backend.buffer,  # TODO: refactor without self.backend
             self.last_raw_line,
         )
         err_log.exception('Fatal error traceback')
         err_log.error('----------------------------------------')
 
         if self.error_count > 10:
             # quit if too many errors
-            dt = datetime.utcnow() - self.last_error_timestamp
-            dt_seconds = dt.total_seconds()
+            dt_seconds: float = 0.0
+            if self.last_error_timestamp is not None:
+                dt = datetime.now(timezone.utc) - self.last_error_timestamp
+                dt_seconds = dt.total_seconds()
+
             if dt_seconds < 5:
                 LOGGER.error('Too many errors, can\'t continue')
                 os._exit(1)
             # remove 1 error per full 5s that passed since last error
-            self.error_count = max(0, self.error_count - dt_seconds // 5)
+            self.error_count = int(max(0, self.error_count - dt_seconds // 5))
 
-        self.last_error_timestamp = datetime.utcnow()
+        self.last_error_timestamp = datetime.now(timezone.utc)
         self.error_count = self.error_count + 1
 
-    def change_current_nick(self, new_nick):
+    def rebuild_nick(self) -> None:
+        """Rebuild nick as a new identifier.
+
+        This method exists to update the casemapping rules for the
+        :class:`~sopel.tools.identifiers.Identifier` that represents the bot's
+        nick, e.g. after ISUPPORT info is received.
+        """
+        self._nick = self.make_identifier(str(self._nick))
+
+    def change_current_nick(self, new_nick: str) -> None:
         """Change the current nick without configuration modification.
 
         :param str new_nick: new nick to be used by the bot
         """
-        self._nick = tools.Identifier(new_nick)
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
+        self._nick = self.make_identifier(new_nick)
         LOGGER.debug('Sending nick "%s"', self.nick)
         self.backend.send_nick(self.nick)
 
-    def on_close(self):
+    def on_close(self) -> None:
         """Call shutdown methods."""
+        self._connection_registered.clear()
         self._shutdown()
 
-    def _shutdown(self):
+    def _shutdown(self) -> None:
         """Handle shutdown tasks.
 
         Must be overridden by subclasses to do anything useful.
         """
-        pass
 
     # Features
 
-    def dispatch(self, pretrigger):
+    @abc.abstractmethod
+    def dispatch(self, pretrigger: trigger.PreTrigger):
         """Handle running the appropriate callables for an incoming message.
 
         :param pretrigger: Sopel PreTrigger object
         :type pretrigger: :class:`sopel.trigger.PreTrigger`
-        :raise NotImplementedError: if the subclass does not implement this
-                                    required method
 
         .. important::
             This method **MUST** be implemented by concrete subclasses.
         """
-        raise NotImplementedError
 
-    def log_raw(self, line, prefix):
-        """Log a raw line to the raw log.
+    def log_raw(self, line: str, prefix: str) -> None:
+        """Log raw line to the raw log.
 
         :param str line: the raw line
         :param str prefix: additional information to prepend to the log line
 
         The ``prefix`` is usually either ``>>`` for an outgoing ``line`` or
         ``<<`` for a received one.
         """
         if not self.settings.core.log_raw:
             return
         logger = logging.getLogger('sopel.raw')
-        logger.info('\t'.join([prefix, line.strip()]))
-
-    def cap_req(self, plugin_name, capability, arg=None, failure_callback=None,
-                success_callback=None):
-        """Tell Sopel to request a capability when it starts.
-
-        :param str plugin_name: the plugin requesting the capability
-        :param str capability: the capability requested, optionally prefixed
-                               with ``-`` or ``=``
-        :param str arg: arguments for the capability request
-        :param failure_callback: a function that will be called if the
-                                 capability request fails
-        :type failure_callback: :term:`function`
-        :param success_callback: a function that will be called if the
-                                 capability is successfully requested
-        :type success_callback: :term:`function`
-
-        By prefixing the capability with ``-``, it will be ensured that the
-        capability is not enabled. Similarly, by prefixing the capability with
-        ``=``, it will be ensured that the capability is enabled. Requiring and
-        disabling is "first come, first served"; if one plugin requires a
-        capability, and another prohibits it, this function will raise an
-        exception in whichever plugin loads second. An exception will also be
-        raised if the plugin is being loaded after the bot has already started,
-        and the request would change the set of enabled capabilities.
-
-        If the capability is not prefixed, and no other plugin prohibits it, it
-        will be requested. Otherwise, it will not be requested. Since
-        capability requests that are not mandatory may be rejected by the
-        server, as well as by other plugins, a plugin which makes such a
-        request should account for that possibility.
-
-        The actual capability request to the server is handled after the
-        completion of this function. In the event that the server denies a
-        request, the ``failure_callback`` function will be called, if provided.
-        The arguments will be a :class:`~sopel.bot.Sopel` object, and the
-        capability which was rejected. This can be used to disable callables
-        which rely on the capability. It will be be called either if the server
-        NAKs the request, or if the server enabled it and later DELs it.
-
-        The ``success_callback`` function will be called upon acknowledgment
-        of the capability from the server, whether during the initial
-        capability negotiation, or later.
-
-        If ``arg`` is given, and does not exactly match what the server
-        provides or what other plugins have requested for that capability, it
-        is considered a conflict.
-        """
-        # TODO raise better exceptions
-        cap = capability[1:]
-        prefix = capability[0]
-
-        entry = self._cap_reqs.get(cap, [])
-        if any((ent.arg != arg for ent in entry)):
-            raise Exception('Capability conflict')
-
-        if prefix == '-':
-            if self.connection_registered and cap in self.enabled_capabilities:
-                raise Exception('Can not change capabilities after server '
-                                'connection has been completed.')
-            if any((ent.prefix != '-' for ent in entry)):
-                raise Exception('Capability conflict')
-            entry.append(CapReq(prefix, plugin_name, failure_callback, arg,
-                                success_callback))
-            self._cap_reqs[cap] = entry
-        else:
-            if prefix != '=':
-                cap = capability
-                prefix = ''
-            if self.connection_registered and (cap not in
-                                               self.enabled_capabilities):
-                raise Exception('Can not change capabilities after server '
-                                'connection has been completed.')
-            # Non-mandatory will callback at the same time as if the server
-            # rejected it.
-            if any((ent.prefix == '-' for ent in entry)) and prefix == '=':
-                raise Exception('Capability conflict')
-            entry.append(CapReq(prefix, plugin_name, failure_callback, arg,
-                                success_callback))
-            self._cap_reqs[cap] = entry
+        logger.info("%s\t%r", prefix, line)
 
-    def write(self, args, text=None):
+    def write(self, args: Iterable[str], text: Optional[str] = None) -> None:
         """Send a command to the server.
 
         :param args: an iterable of strings, which will be joined by spaces
-        :type args: :term:`iterable`
-        :param str text: a string that will be prepended with a ``:`` and added
-                         to the end of the command
+        :param text: a string that will be prepended with a ``:`` and added to
+                     the end of the command
 
         ``args`` is an iterable of strings, which are joined by spaces.
         ``text`` is treated as though it were the final item in ``args``, but
         is preceded by a ``:``. This is a special case which means that
         ``text``, unlike the items in ``args``, may contain spaces (though this
         constraint is not checked by ``write``).
 
@@ -446,116 +597,163 @@
 
             The connection backend is responsible for formatting and sending
             the message through the IRC connection. See the
             :meth:`sopel.irc.abstract_backends.AbstractIRCBackend.send_command`
             method for more information.
 
         """
-        args = [safe(arg) for arg in args]
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         self.backend.send_command(*args, text=text)
 
     # IRC Commands
 
-    def action(self, text, dest):
+    def action(self, text: str, dest: str) -> None:
         """Send a CTCP ACTION PRIVMSG to a user or channel.
 
         :param str text: the text to send in the CTCP ACTION
         :param str dest: the destination of the CTCP ACTION
 
         The same loop detection and length restrictions apply as with
         :func:`say`, though automatic message splitting is not available.
         """
         self.say('\001ACTION {}\001'.format(text), dest)
 
-    def join(self, channel, password=None):
+    def join(self, channel: str, password: Optional[str] = None) -> None:
         """Join a ``channel``.
 
         :param str channel: the channel to join
         :param str password: an optional channel password
 
         If ``channel`` contains a space, and no ``password`` is given, the
         space is assumed to split the argument into the channel to join and its
         password. ``channel`` should not contain a space if ``password``
         is given.
         """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         self.backend.send_join(channel, password=password)
 
-    def kick(self, nick, channel, text=None):
+    def kick(
+        self,
+        nick: str,
+        channel: str,
+        text: Optional[str] = None,
+    ) -> None:
         """Kick a ``nick`` from a ``channel``.
 
-        :param str nick: nick to kick out of the ``channel``
-        :param str channel: channel to kick ``nick`` from
-        :param str text: optional text for the kick
+        :param nick: nick to kick out of the ``channel``
+        :param channel: channel to kick ``nick`` from
+        :param text: optional text for the kick
 
         The bot must be an operator in the specified channel for this to work.
 
         .. versionadded:: 7.0
         """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         self.backend.send_kick(channel, nick, reason=text)
 
-    def notice(self, text, dest):
+    def notice(self, text: str, dest: str) -> None:
         """Send an IRC NOTICE to a user or channel (``dest``).
 
-        :param str text: the text to send in the NOTICE
-        :param str dest: the destination of the NOTICE
+        :param text: the text to send in the NOTICE
+        :param dest: the destination of the NOTICE
         """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         self.backend.send_notice(dest, text)
 
-    def part(self, channel, msg=None):
-        """Leave a ``channel``.
+    def part(self, channel: str, msg: Optional[str] = None) -> None:
+        """Leave a channel.
 
-        :param str channel: the channel to leave
-        :param str msg: the message to display when leaving a channel
+        :param channel: the channel to leave
+        :param msg: the message to display when leaving a channel
         """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         self.backend.send_part(channel, reason=msg)
 
-    def quit(self, message):
-        """Disconnect from IRC and close the bot."""
+    def quit(self, message: Optional[str] = None) -> None:
+        """Disconnect from IRC and close the bot.
+
+        :param message: optional QUIT message to send (e.g. "Bye!")
+        """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
+        self._connection_registered.clear()
         self.backend.send_quit(reason=message)
         self.hasquit = True
         # Wait for acknowledgment from the server. Per RFC 2812 it should be
         # an ERROR message, but many servers just close the connection.
         # Either way is fine by us. Closing the connection now would mean that
         # stuff in the buffers that has not yet been processed would never be
         # processed. It would also release the main thread, which is
         # problematic because whomever called quit might still want to do
         # something before the main thread quits.
 
-    def reply(self, text, dest, reply_to, notice=False):
-        """Send a PRIVMSG to a user or channel, prepended with a nickname.
+    def restart(self, message: Optional[str] = None) -> None:
+        """Disconnect from IRC and restart the bot.
 
-        :param str text: the text of the reply
-        :param str dest: the destination of the reply
-        :param str reply_to: the nickname that will be prepended to ``text``
-        :param bool notice: whether to send the reply as a NOTICE or not,
-                            defaults to ``False``
+        :param message: optional QUIT message to send (e.g. "Be right back!")
+        """
+        self.wantsrestart = True
+        self.quit(message)
 
-        If ``notice`` is ``True``, send a NOTICE rather than a PRIVMSG.
+    def reply(
+        self,
+        text: str,
+        dest: str,
+        reply_to: str,
+        notice: bool = False,
+    ) -> None:
+        """Send a PRIVMSG to a user or channel, prepended with ``reply_to``.
+
+        :param text: the text of the reply
+        :param dest: the destination of the reply
+        :param reply_to: the nickname that the reply will be prepended with
+        :param notice: whether to send the reply as a ``NOTICE`` or not,
+                       defaults to ``False``
+
+        If ``notice`` is ``True``, send a ``NOTICE`` rather than a ``PRIVMSG``.
 
         The same loop detection and length restrictions apply as with
         :meth:`say`, though automatic message splitting is not available.
         """
         text = '%s: %s' % (reply_to, text)
         if notice:
             self.notice(text, dest)
         else:
             self.say(text, dest)
 
-    def say(self, text, recipient, max_messages=1, truncation='', trailing=''):
-        """Send a PRIVMSG to a user or channel.
-
-        :param str text: the text to send
-        :param str recipient: the message recipient
-        :param int max_messages: split ``text`` into at most this many messages
-                                 if it is too long to fit in one (optional)
-        :param str truncation: string to append if ``text`` is too long to fit
-                               in a single message, or into the last message if
-                               ``max_messages`` is greater than 1 (optional)
-        :param str trailing: string to append after ``text`` and (if used)
-                             ``truncation`` (optional)
+    def say(
+        self,
+        text: str,
+        recipient: str,
+        max_messages: int = 1,
+        truncation: str = '',
+        trailing: str = '',
+    ) -> None:
+        """Send a ``PRIVMSG`` to a user or channel.
+
+        :param text: the text to send
+        :param recipient: the message recipient
+        :param max_messages: split ``text`` into at most this many messages
+                             if it is too long to fit in one (optional)
+        :param truncation: string to append if ``text`` is too long to fit in
+                           a single message, or into the last message if
+                           ``max_messages`` is greater than 1 (optional)
+        :param trailing: string to append after ``text`` and (if used)
+                         ``truncation`` (optional)
 
         By default, this will attempt to send the entire ``text`` in one
         message. If the text is too long for the server, it may be truncated.
 
         If ``max_messages`` is given, the ``text`` will be split into at most
         that many messages. The split is made at the last space character
         before the "safe length" (which is calculated based on the bot's
@@ -601,74 +799,60 @@
             # The ending " goes missing
 
         .. versionadded:: 7.1
 
             The ``truncation`` and ``trailing`` parameters.
 
         """
+        if self.backend is None:
+            raise RuntimeError(ERR_BACKEND_NOT_INITIALIZED)
+
         excess = ''
-        if not isinstance(text, unicode):
+
+        if not isinstance(text, str):
             # Make sure we are dealing with a Unicode string
             text = text.decode('utf-8')
 
-        if max_messages > 1 or truncation or trailing:
-            # Handle message splitting/truncation only if needed
-            try:
-                hostmask_length = len(self.hostmask)
-            except KeyError:
-                # calculate maximum possible length, given current nick/username
-                hostmask_length = (
-                    len(self.nick)  # own nick length
-                    + 1  # (! separator)
-                    + 1  # (for the optional ~ in user)
-                    + min(  # own ident length, capped to ISUPPORT or RFC maximum
-                        len(self.user),
-                        getattr(self.isupport, 'USERLEN', 9))
-                    + 1  # (@ separator)
-                    + 63  # <hostname> has a maximum length of 63 characters.
-                )
-            safe_length = (
-                512  # maximum IRC line length in bytes, per RFC
-                - 1  # leading colon
-                - hostmask_length  # calculated/maximum length of own hostmask prefix
-                - 1  # space between prefix & command
-                - 7  # PRIVMSG command
-                - 1  # space before recipient
-                - len(recipient.encode('utf-8'))  # target channel/nick (can contain Unicode)
-                - 2  # space after recipient, colon before text
-                - 2  # trailing CRLF
-            )
-
-            if max_messages == 1 and trailing:
-                safe_length -= len(trailing.encode('utf-8'))
-            text, excess = tools.get_sendable_message(text, safe_length)
-
-        if max_messages == 1:
-            if excess and truncation:
-                # only append `truncation` if this is the last message AND it's still too long
+        safe_length = self.safe_text_length(recipient)
+        if trailing and max_messages == 1:
+            # last message needs to leave room for `trailing`
+            safe_length -= len(trailing.encode('utf-8'))
+
+        # only think about `truncation` if we need to
+        if safe_length < len(text.encode('utf-8')):
+            if max_messages == 1:
+                # last message needs to leave room for `truncation`
+                # if it's still too long to fit in the line
                 safe_length -= len(truncation.encode('utf-8'))
-                text, excess = tools.get_sendable_message(text, safe_length)
+            text, excess = tools.get_sendable_message(text, safe_length)
+            if max_messages == 1:
                 text += truncation
 
-            # ALWAYS append `trailing`;
-            # its length is included when determining if truncation happened above
+        if max_messages == 1:
+            # ALWAYS append `trailing` to the last message;
+            # its size is included in the initial `safe_length` check
             text += trailing
 
         flood_max_wait = self.settings.core.flood_max_wait
         flood_burst_lines = self.settings.core.flood_burst_lines
         flood_refill_rate = self.settings.core.flood_refill_rate
         flood_empty_wait = self.settings.core.flood_empty_wait
 
         flood_text_length = self.settings.core.flood_text_length
         flood_penalty_ratio = self.settings.core.flood_penalty_ratio
 
+        antiloop_threshold = min(10, self.settings.core.antiloop_threshold)
+        antiloop_window = self.settings.core.antiloop_window
+        antiloop_repeat_text = self.settings.core.antiloop_repeat_text
+        antiloop_silent_after = self.settings.core.antiloop_silent_after
+
         with self.sending:
-            recipient_id = tools.Identifier(recipient)
+            recipient_id = self.make_identifier(recipient)
             recipient_stack = self.stack.setdefault(recipient_id, {
-                'messages': [],
+                'messages': deque(maxlen=10),
                 'flood_left': flood_burst_lines,
             })
 
             if recipient_stack['messages']:
                 elapsed = time.time() - recipient_stack['messages'][-1][0]
             else:
                 # Default to a high enough value that we won't care.
@@ -707,26 +891,29 @@
                         flood_max_wait,
                         initial_wait_time,
                         penalty,
                     )
                     time.sleep(sleep_time)
 
             # Loop detection
-            messages = [m[1] for m in recipient_stack['messages'][-8:]]
+            if antiloop_threshold > 0 and elapsed < antiloop_window:
+                messages = [m[1] for m in recipient_stack['messages']]
 
-            # If what we're about to send repeated at least 5 times in the last
-            # two minutes, replace it with '...'
-            if messages.count(text) >= 5 and elapsed < 120:
-                text = '...'
-                if messages.count('...') >= 3:
-                    # If we've already said '...' 3 times, discard message
-                    return
+                # If what we're about to send repeated at least N times
+                # in the anti-looping window, replace it
+                if messages.count(text) >= antiloop_threshold:
+                    text = antiloop_repeat_text
+                    if messages.count(text) >= antiloop_silent_after:
+                        # If we've already said that N times, discard message
+                        return
 
             self.backend.send_privmsg(recipient, text)
-            recipient_stack['flood_left'] = max(0, recipient_stack['flood_left'] - 1)
-            recipient_stack['messages'].append((time.time(), safe(text)))
-            recipient_stack['messages'] = recipient_stack['messages'][-10:]
+
+            # update recipient metadata
+            flood_left = recipient_stack['flood_left'] - 1
+            recipient_stack['flood_left'] = max(0, flood_left)
+            recipient_stack['messages'].append((time.time(), text))
 
         # Now that we've sent the first part, we need to send the rest if
         # requested. Doing so recursively seems simpler than iteratively.
         if max_messages > 1 and excess:
             self.say(excess, recipient, max_messages - 1, truncation, trailing)
```

### Comparing `sopel-7.1.9/sopel/irc/isupport.py` & `sopel-8.0.0/sopel/irc/isupport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# coding=utf-8
 """IRC Tools for ISUPPORT management.
 
 When a server wants to advertise its features and settings, it can use the
 ``RPL_ISUPPORT`` command (``005`` numeric) with a list of arguments.
 
 .. seealso::
 
     https://modern.ircdocs.horse/#rplisupport-005
 
 """
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import functools
 import itertools
 import re
 
 
 def _optional(parser, default=None):
@@ -94,15 +93,15 @@
 
     modes = result.group('modes')
     prefixes = result.group('prefixes')
 
     if len(modes) != len(prefixes):
         raise ValueError('Mode list does not match for PREFIX: %r' % value)
 
-    return tuple(sorted(zip(modes, prefixes)))
+    return tuple(zip(modes, prefixes))
 
 
 ISUPPORT_PARSERS = {
     'AWAYLEN': int,
     'CASEMAPPING': str,
     'CHANLIMIT': _map_items(int),
     'CHANMODES': _parse_chanmodes,
@@ -110,14 +109,15 @@
     'CHANTYPES': _optional(tuple),
     'ELIST': _parse_elist,
     'EXCEPTS': _optional(_single_character, default='e'),
     'EXTBAN': _parse_extban,
     'HOSTLEN': int,
     'INVEX': _optional(_single_character, default='I'),
     'KICKLEN': int,
+    'LINELEN': int,
     'MAXLIST': _map_items(int),
     'MAXTARGETS': _optional(int),
     'MODES': _optional(int),
     'NETWORK': str,
     'NICKLEN': int,
     'PREFIX': _optional(_parse_prefix),
     'SAFELIST': _no_value,
@@ -125,30 +125,57 @@
     'STATUSMSG': _optional(tuple),
     'TARGMAX': _optional(_map_items(int), default=tuple()),
     'TOPICLEN': int,
     'USERLEN': int,
 }
 
 
+def _unescape_param(param):
+    """Handle escape sequences in ISUPPORT parameter values.
+
+    Sopel follows the recommendation of `modern.ircdocs.horse`__ which only
+    recognizes the escape sequences ``\\x20, \\x5C, \\x3D``. All other such
+    escape sequences will be passed through unaltered.
+
+    .. __: https://modern.ircdocs.horse/#rplisupport-005
+    """
+    HEX_PATTERN = r"\\x([0-9a-fA-F]{2})"
+
+    def _unescape(match):
+        num = match.group(1).upper()
+        if num == "20":
+            result = " "
+        elif num == "5C":
+            result = "\\"
+        elif num == "3D":
+            result = "="
+        else:
+            result = match.group(0)
+
+        return result
+
+    return re.sub(HEX_PATTERN, _unescape, param)
+
+
 def parse_parameter(arg):
     items = arg.split('=', 1)
     if len(items) == 2:
-        key, value = items
+        key, value = items[0], _unescape_param(items[1])
     else:
         key, value = items[0], None
 
     if key.startswith('-'):
         # ignore value for removed parameters
         return (key, None)
 
     parser = ISUPPORT_PARSERS.get(key, _optional(str))
     return (key, parser(value))
 
 
-class ISupport(object):
+class ISupport:
     """Storage class for IRC's ``ISUPPORT`` feature.
 
     An instance of ``ISupport`` can be used as a read-only dict, to store
     features advertised by the IRC server::
 
         >>> isupport = ISupport(chanlimit=(('&', None), ('#', 70)))
         >>> isupport['CHANLIMIT']
@@ -166,14 +193,20 @@
         Traceback (most recent call last):
           File "<stdin>", line 1, in <module>
         AttributeError: 'ISupport' object has no attribute 'CHANMODE'
 
     The list of possible parameters can be found at
     `modern.ircdocs.horse's RPL_ISUPPORT Parameters`__.
 
+    .. important::
+
+        While this object's attributes and dict-like behavior are part of
+        Sopel's public API, its *methods* are considered internal code and
+        plugins should not call them.
+
     .. __: https://modern.ircdocs.horse/#rplisupport-parameters
     """
     def __init__(self, **kwargs):
         self.__isupport = dict(
             (key.upper(), value)
             for key, value in kwargs.items()
             if not key.startswith('-'))
@@ -193,15 +226,15 @@
 
         return self.__isupport[name]
 
     def __setattr__(self, name, value):
         # make sure you can't set the value of any ISUPPORT attribute yourself
         if name == '_ISupport__isupport':
             # allow to set self.__isupport inside of the class
-            super(ISupport, self).__setattr__(name, value)
+            super().__setattr__(name, value)
         elif name in self.__isupport:
             # reject any modification of __isupport
             raise AttributeError("Can't set value for %r" % name)
         elif name not in self.__dict__:
             raise AttributeError('Unknown attribute')
 
     def get(self, name, default=None):
@@ -325,29 +358,31 @@
         """
         if 'MAXLIST' not in self:
             raise AttributeError('MAXLIST')
 
         return dict(self['MAXLIST'])
 
     @property
-    def PREFIX(self):
+    def PREFIX(self) -> dict[str, str]:
         """Expose ``PREFIX`` as a dict, if advertised by the server.
 
         This exposes information about the modes and nick prefixes used for
         user privileges in channels::
 
             >>> isupport.PREFIX
             {
                 'q': '~',
                 'a': '&',
                 'o': '@',
                 'h': '%',
                 'v': '+',
             }
 
+        Entries are in order of descending privilege.
+
         This attribute is not available if the server does not provide the
         right information, and accessing it will raise an
         :exc:`AttributeError`.
 
         .. seealso::
 
             https://modern.ircdocs.horse/#prefix-parameter
```

### Comparing `sopel-7.1.9/sopel/loader.py` & `sopel-8.0.0/sopel/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,30 @@
-# coding=utf-8
 """Utility functions to manage plugin callables from a Python module.
 
 .. important::
 
     Its usage and documentation is for Sopel core development and advanced
     developers. It is subject to rapid changes between versions without much
     (or any) warning.
 
     Do **not** build your plugin based on what is here, you do **not** need to.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import inspect
 import logging
 import re
-import sys
 
 from sopel.config.core_section import COMMAND_DEFAULT_HELP_PREFIX
-from sopel.tools import deprecated, itervalues
-
-
-if sys.version_info.major >= 3:
-    basestring = (str, bytes)
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-@deprecated(
-    reason="Replaced by simple logic using inspect.getdoc()",
-    version='7.1',
-    removed_in='8.0',
-)
-def trim_docstring(doc):
-    """Get the docstring as a series of lines that can be sent.
-
-    :param str doc: a callable's docstring to trim
-    :return: a list of trimmed lines
-    :rtype: list
-
-    This function acts like :func:`inspect.cleandoc` but doesn't replace tabs,
-    and instead of a :class:`str` it returns a :class:`list`.
-    """
-    if not doc:
-        return []
-    lines = doc.expandtabs().splitlines()
-    indent = sys.maxsize
-    for line in lines[1:]:
-        stripped = line.lstrip()
-        if stripped:
-            indent = min(indent, len(line) - len(stripped))
-    trimmed = [lines[0].strip()]
-    if indent < sys.maxsize:
-        for line in lines[1:]:
-            trimmed.append(line[:].rstrip())
-    while trimmed and not trimmed[-1]:
-        trimmed.pop()
-    while trimmed and not trimmed[0]:
-        trimmed.pop(0)
-    return trimmed
-
-
 def clean_callable(func, config):
     """Clean the callable. (compile regexes, fix docs, set defaults)
 
     :param func: the callable to clean
     :type func: callable
     :param config: Sopel's settings
     :type config: :class:`sopel.config.Config`
@@ -85,73 +44,68 @@
         doc = docstring.splitlines()
 
     func.thread = getattr(func, 'thread', True)
 
     if is_limitable(func):
         # These attributes are a waste of memory on callables that don't pass
         # through Sopel's rate-limiting machinery
-        func.rate = getattr(func, 'rate', 0)
+        func.user_rate = getattr(func, 'user_rate', 0)
         func.channel_rate = getattr(func, 'channel_rate', 0)
         func.global_rate = getattr(func, 'global_rate', 0)
+        func.user_rate_message = getattr(func, 'user_rate_message', None)
+        func.channel_rate_message = getattr(func, 'channel_rate_message', None)
+        func.global_rate_message = getattr(func, 'global_rate_message', None)
+        func.default_rate_message = getattr(func, 'default_rate_message', None)
         func.unblockable = getattr(func, 'unblockable', False)
 
     if not is_triggerable(func) and not is_url_callback(func):
         # Adding the remaining default attributes below is potentially
         # confusing to other code (and a waste of memory) for jobs.
         return
 
+    func.allow_bots = getattr(func, 'allow_bots', False)
     func.echo = getattr(func, 'echo', False)
     func.priority = getattr(func, 'priority', 'medium')
     func.output_prefix = getattr(func, 'output_prefix', '')
 
     if not hasattr(func, 'event'):
         func.event = ['PRIVMSG']
     else:
-        if isinstance(func.event, basestring):
-            func.event = [func.event.upper()]
-        else:
-            func.event = [event.upper() for event in func.event]
-
-    # TODO: remove in Sopel 8
-    # Stay compatible with old Phenny/Jenni "modules" (plugins)
-    # that set the attribute directly
-    if hasattr(func, 'rule') and isinstance(func.rule, basestring):
-        LOGGER.warning(
-            'The `rule` attribute of %s.%s should be a list, not a string; '
-            'this behavior is deprecated in Sopel 7.1 '
-            'and will be removed in Sopel 8. '
-            'To prevent this problem always use `sopel.plugin.rule(%r)`.',
-            func.__module__, func.__name__, func.rule)
-        func.rule = [func.rule]
+        func.event = [event.upper() for event in func.event]
 
     if any(hasattr(func, attr) for attr in ['commands', 'nickname_commands', 'action_commands']):
         if hasattr(func, 'example'):
-            # If no examples are flagged as user-facing, just show the first one like Sopel<7.0 did
-            examples = [rec["example"] for rec in func.example if rec["help"]] or [func.example[0]["example"]]
+            # If no examples are flagged as user-facing,
+            # just show the first one like Sopel<7.0 did
+            examples = [
+                rec["example"]
+                for rec in func.example
+                if rec["is_help"]
+            ] or [func.example[0]["example"]]
             for i, example in enumerate(examples):
                 example = example.replace('$nickname', nick)
                 if example[0] != help_prefix and not example.startswith(nick):
                     example = example.replace(
                         COMMAND_DEFAULT_HELP_PREFIX, help_prefix, 1)
                 examples[i] = example
         if doc or examples:
-            cmds = []
+            cmds: list[str] = []
             cmds.extend(getattr(func, 'commands', []))
             cmds.extend(getattr(func, 'nickname_commands', []))
             for command in cmds:
                 func._docs[command] = (doc, examples)
 
-    if hasattr(func, 'intents'):
+    if hasattr(func, 'ctcp'):
         # Can be implementation-dependent
         _regex_type = type(re.compile(''))
-        func.intents = [
-            (intent
-                if isinstance(intent, _regex_type)
-                else re.compile(intent, re.IGNORECASE))
-            for intent in func.intents
+        func.ctcp = [
+            (ctcp_pattern
+                if isinstance(ctcp_pattern, _regex_type)
+                else re.compile(ctcp_pattern, re.IGNORECASE))
+            for ctcp_pattern in func.ctcp
         ]
 
 
 def is_limitable(obj):
     """Check if ``obj`` needs to carry attributes related to limits.
 
     :param obj: any :term:`function` to check
@@ -170,15 +124,15 @@
         'rule',
         'rule_lazy_loaders',
         'find_rules',
         'find_rules_lazy_loaders',
         'search_rules',
         'search_rules_lazy_loaders',
         'event',
-        'intents',
+        'ctcp',
         'commands',
         'nickname_commands',
         'action_commands',
         'url_regex',
         'url_lazy_loaders',
     )
     allowed = any(hasattr(obj, attr) for attr in allowed_attrs)
@@ -190,16 +144,16 @@
     """Check if ``obj`` can handle the bot's triggers.
 
     :param obj: any :term:`function` to check
     :return: ``True`` if ``obj`` can handle the bot's triggers
 
     A triggerable is a callable that will be used by the bot to handle a
     particular trigger (i.e. an IRC message): it can be a regex rule, an
-    event, an intent, a command, a nickname command, or an action command.
-    However, it must not be a job or a URL callback.
+    event, a CTCP command, a command, a nickname command, or an action
+    command. However, it must not be a job or a URL callback.
 
     .. seealso::
 
         Many of the decorators defined in :mod:`sopel.plugin` make the
         decorated function a triggerable object.
 
     """
@@ -214,15 +168,15 @@
         'rule',
         'rule_lazy_loaders',
         'find_rules',
         'find_rules_lazy_loaders',
         'search_rules',
         'search_rules_lazy_loaders',
         'event',
-        'intents',
+        'ctcp',
         'commands',
         'nickname_commands',
         'action_commands',
     )
     allowed = any(hasattr(obj, attr) for attr in allowed_attrs)
 
     return allowed and not forbidden
@@ -278,15 +232,15 @@
     callable, i.e. properties related to threading, docs, examples, rate
     limiting, commands, rules, and other features.
     """
     callables = []
     shutdowns = []
     jobs = []
     urls = []
-    for obj in itervalues(vars(module)):
+    for obj in vars(module).values():
         if callable(obj):
             is_sopel_callable = getattr(obj, '_sopel_callable', False) is True
             if getattr(obj, '__name__', None) == 'shutdown':
                 shutdowns.append(obj)
             elif not is_sopel_callable:
                 continue
             elif is_triggerable(obj):
```

### Comparing `sopel-7.1.9/sopel/logger.py` & `sopel-8.0.0/sopel/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding=utf-8
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import logging
 from logging.config import dictConfig
 import os
 
 from sopel import tools
+from sopel.lifecycle import deprecated
 
 
 class IrcLoggingHandler(logging.Handler):
     """Logging handler for output to an IRC channel.
 
     :param bot: a Sopel instance
     :type bot: :class:`sopel.bot.Sopel`
     :param level: minimum level of log messages to report through this handler
     :type level: :ref:`logging level <levels>`
 
     Implementation of a :class:`logging.Handler`.
     """
     def __init__(self, bot, level):
-        super(IrcLoggingHandler, self).__init__(level)
+        super().__init__(level)
         self._bot = bot
         self._channel = bot.settings.core.logging_channel
 
     def emit(self, record):
         """Emit a log ``record`` to the IRC channel.
 
         :param record: the log record to output
         :type record: :class:`logging.LogRecord`
         """
-        if self._bot.backend is None or not self._bot.backend.is_connected():
-            # Don't emit logs when the bot is not connected.
+        if not self._bot.connection_registered:
+            # Don't emit logs to IRC when the bot is not connected & registered.
             return
 
         try:
             msg = self.format(record).replace('\n', ' ')
             self._bot.say(msg, self._channel)
         except (KeyboardInterrupt, SystemExit):
             raise
@@ -49,15 +49,15 @@
     :type fmt: :ref:`format string <formatstrings>`
     :param datefmt: date format
     :type datefmt: :ref:`format string <formatstrings>`
 
     Implementation of a :class:`logging.Formatter`.
     """
     def __init__(self, fmt='[%(filename)s] %(message)s', datefmt=None):
-        super(ChannelOutputFormatter, self).__init__(fmt=fmt, datefmt=datefmt)
+        super().__init__(fmt=fmt, datefmt=datefmt)
 
     def formatException(self, exc_info):
         """Format the exception info as a string for output.
 
         :param tuple exc_info: standard exception information returned by
                                :func:`~sys.exc_info`
         """
@@ -103,14 +103,19 @@
             },
             # asynchat exception logger
             'sopel.exceptions': {
                 'level': 'INFO',
                 'propagate': False,
                 'handlers': ['exceptionfile'],
             },
+            # asyncio logging
+            'asyncio': {
+                'level': 'DEBUG',
+                'handlers': ['console'],
+            },
         },
         'handlers': {
             # output on stderr
             'console': {
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
                 'formatter': 'sopel',
@@ -152,15 +157,15 @@
                 'formatter': 'raw',
             },
         },
     }
     dictConfig(logging_config)
 
 
-@tools.deprecated(
+@deprecated(
     reason='use sopel.tools.get_logger instead',
     version='7.0',
     warning_in='8.0',
     removed_in='9.0',
 )
 def get_logger(name=None):
     """Return a logger for a module, if the name is given.
```

### Comparing `sopel-7.1.9/sopel/module.py` & `sopel-8.0.0/sopel/module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# coding=utf-8
 """The :mod:`sopel.module` sub-module is replaced by :mod:`sopel.plugin`.
 
 .. deprecated:: 7.1
 
     Use :mod:`sopel.plugin` instead. This will be removed in Sopel 9.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+from sopel.lifecycle import deprecated
 # Import everything from sopel.plugin at the time of replacement.
 # Everything new from this point on must *not* leak here.
 # Therefore, don't add anything to this import list. Ever.
 from sopel.plugin import (  # noqa
     ADMIN,
     action_commands,
     commands,
@@ -39,14 +39,28 @@
     thread,
     unblockable,
     url,
     VOICE,
 )
 
 
+deprecated(
+    'sopel.module has been replaced by sopel.plugin',
+    version='8.0',
+    removed_in='9.0',
+    func=lambda *args: ...,
+)()
+
+
+@deprecated(
+    '`@intent` is replaced by `sopel.plugin.ctcp`',
+    version='7.1',
+    removed_in='9.0',
+    warning_in='8.0',
+)
 def intent(*intent_list):
     """Decorate a callable to trigger on intent messages.
 
     :param str intent_list: one or more intent(s) on which to trigger (really,
                             the only useful value is ``ACTION``)
 
     .. versionadded:: 5.2.0
```

### Comparing `sopel-7.1.9/sopel/modules/admin.py` & `sopel-8.0.0/sopel/builtins/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# coding=utf-8
 """
 admin.py - Sopel Admin Plugin
 Copyright 2010-2011, Sean B. Palmer (inamidst.com) and Michael Yanovich
 (yanovich.net)
 Copyright © 2012, Elad Alfassa, <elad@fedoraproject.org>
 Copyright 2013, Ari Koivula <ari@koivu.la>
 Copyright 2019, Florian Strzelecki, https://github.com/Exirel
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import logging
 
 from sopel import plugin
 from sopel.config import types
 
 LOGGER = logging.getLogger(__name__)
 
 ERROR_JOIN_NO_CHANNEL = 'Which channel should I join?'
 """Error message when channel is missing from command arguments."""
 ERROR_PART_NO_CHANNEL = 'Which channel should I quit?'
 """Error message when channel is missing from command arguments."""
 ERROR_NOTHING_TO_SAY = 'I need a channel and a message to talk.'
 """Error message when channel and/or message are missing."""
+ERROR_NOTHING_TO_RAW = 'I need an IRC message to send.'
+"""Error message when no raw IRC message was given."""
 
 
 class AdminSection(types.StaticSection):
     hold_ground = types.BooleanAttribute('hold_ground', default=False)
     """Auto re-join on kick"""
     auto_accept_invite = types.BooleanAttribute('auto_accept_invite', default=True)
     """Auto-join channels when invited"""
@@ -50,21 +51,21 @@
 
 def setup(bot):
     bot.config.define_section('admin', AdminSection)
 
 
 class InvalidSection(Exception):
     def __init__(self, section):
-        super(InvalidSection, self).__init__(self, 'Section [{}] does not exist.'.format(section))
+        super().__init__(self, 'Section [{}] does not exist.'.format(section))
         self.section = section
 
 
 class InvalidSectionOption(Exception):
     def __init__(self, section, option):
-        super(InvalidSectionOption, self).__init__(self, 'Section [{}] does not have option \'{}\'.'.format(section, option))
+        super().__init__(self, 'Section [{}] does not have option \'{}\'.'.format(section, option))
         self.section = section
         self.option = option
 
 
 def _get_config_channels(channels):
     """List"""
     for channel_info in channels:
@@ -221,14 +222,31 @@
         quit_message = default_message
 
     LOGGER.info(default_message)
     bot.quit(quit_message)
 
 
 @plugin.require_privmsg
+@plugin.require_owner
+@plugin.command('raw')
+@plugin.priority('low')
+@plugin.example('.raw PRIVMSG NickServ :CERT ADD')
+def raw(bot, trigger):
+    """
+    Send a raw IRC message. Can only be done in privmsg by the bot owner.
+    This is mostly useful for debugging.
+    """
+    if trigger.group(2) is None:
+        bot.reply(ERROR_NOTHING_TO_RAW)
+        return
+
+    bot.write([trigger.group(2)])
+
+
+@plugin.require_privmsg
 @plugin.require_admin
 @plugin.command('say', 'msg')
 @plugin.priority('low')
 @plugin.example('.say #YourPants Does anyone else smell neurotoxin?')
 def say(bot, trigger):
     """
     Send a message to a given channel or nick. Can only be done in privmsg by
```

### Comparing `sopel-7.1.9/sopel/modules/adminchannel.py` & `sopel-8.0.0/sopel/builtins/adminchannel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# coding=utf-8
 """
 adminchannel.py - Sopel Channel Admin Plugin
 Copyright 2010-2011, Michael Yanovich, Alek Rollyson, and Elsie Powell
 Copyright © 2012, Elad Alfassa <elad@fedoraproject.org>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import re
 
-from sopel import formatting, plugin, tools
+from sopel import formatting, plugin
 
 
 ERROR_MESSAGE_NOT_OP = "I'm not a channel operator!"
 ERROR_MESSAGE_NO_PRIV = "You are not a channel operator."
 
 
 def default_mask(trigger):
@@ -98,52 +97,65 @@
 @plugin.priority('high')
 def kick(bot, trigger):
     """Kick a user from the channel."""
     text = trigger.group().split()
     argc = len(text)
     if argc < 2:
         return
-    opt = tools.Identifier(text[1])
+    opt = bot.make_identifier(text[1])
     nick = opt
     channel = trigger.sender
     reasonidx = 2
     if not opt.is_nick():
         if argc < 3:
             return
         nick = text[2]
         channel = opt
         reasonidx = 3
     reason = ' '.join(text[reasonidx:])
-    if nick != bot.config.core.nick:
-        bot.kick(nick, channel, reason)
+
+    if nick == bot.nick:
+        bot.reply("Hey! Don't kick me. :(")
+        return
+
+    bot.kick(nick, channel, reason)
 
 
 def configureHostMask(mask):
-    if mask == '*!*@*':
-        return mask
-    if re.match('^[^.@!/]+$', mask) is not None:
+    # shortcut for nick!*@*
+    if re.match(r'^[^.@!/\s]+$', mask) is not None:
         return '%s!*@*' % mask
-    if re.match('^[^@!]+$', mask) is not None:
+
+    # shortcut for *!*@host
+    # won't work for local names w/o dot, but does support cloaks/with/slashes
+    if re.match(r'^[^@!\s]+$', mask) is not None:
         return '*!*@%s' % mask
 
-    m = re.match('^([^!@]+)@$', mask)
+    # shortcut for *!user@*
+    # requires trailing @ to be recognized as a username instead of a nick
+    m = re.match(r'^([^!@\s]+)@$', mask)
     if m is not None:
         return '*!%s@*' % m.group(1)
 
-    m = re.match('^([^!@]+)@([^@!]+)$', mask)
+    # shortcut for *!user@host
+    m = re.match(r'^([^!@\s]+)@([^@!\s]+)$', mask)
     if m is not None:
         return '*!%s@%s' % (m.group(1), m.group(2))
 
-    m = re.match('^([^!@]+)!([^!@]+)@?$', mask)
+    # shortcut for nick!user@*
+    m = re.match(r'^([^!@\s]+)!([^!@\s]+)@?$', mask)
     if m is not None:
         return '%s!%s@*' % (m.group(1), m.group(2))
 
-    if re.match(r'^\S+[!]\S+[@]\S+$', mask) is not None:
+    # not a shortcut; validate full NUH format
+    if re.match(r'^[^!@\s]+![^!@\s]+@[^!@\s]+$', mask) is not None:
         return mask
-    return ''
+
+    # not a shortcut nor a valid hostmask
+    raise ValueError('Invalid hostmask format or unsupported shorthand')
 
 
 @plugin.require_chanmsg
 @plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV, reply=True)
 @plugin.require_bot_privilege(plugin.HALFOP, ERROR_MESSAGE_NOT_OP, reply=True)
 @plugin.command('ban')
 @plugin.priority('high')
@@ -152,25 +164,28 @@
 
     The bot must be a channel operator for this command to work.
     """
     text = trigger.group().split()
     argc = len(text)
     if argc < 2:
         return
-    opt = tools.Identifier(text[1])
+    opt = bot.make_identifier(text[1])
     banmask = opt
     channel = trigger.sender
     if not opt.is_nick():
         if argc < 3:
             return
         channel = opt
         banmask = text[2]
-    banmask = configureHostMask(banmask)
-    if banmask == '':
+
+    try:
+        banmask = configureHostMask(banmask)
+    except ValueError:
         return
+
     bot.write(['MODE', channel, '+b', banmask])
 
 
 @plugin.require_chanmsg
 @plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV, reply=True)
 @plugin.require_bot_privilege(plugin.HALFOP, ERROR_MESSAGE_NOT_OP, reply=True)
 @plugin.command('unban')
@@ -179,25 +194,28 @@
 
     The bot must be a channel operator for this command to work.
     """
     text = trigger.group().split()
     argc = len(text)
     if argc < 2:
         return
-    opt = tools.Identifier(text[1])
+    opt = bot.make_identifier(text[1])
     banmask = opt
     channel = trigger.sender
     if not opt.is_nick():
         if argc < 3:
             return
         channel = opt
         banmask = text[2]
-    banmask = configureHostMask(banmask)
-    if banmask == '':
+
+    try:
+        banmask = configureHostMask(banmask)
+    except ValueError:
         return
+
     bot.write(['MODE', channel, '-b', banmask])
 
 
 @plugin.require_chanmsg
 @plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV, reply=True)
 @plugin.require_bot_privilege(plugin.OP, ERROR_MESSAGE_NOT_OP, reply=True)
 @plugin.command('quiet')
@@ -206,25 +224,28 @@
 
     The bot must be a channel operator for this command to work.
     """
     text = trigger.group().split()
     argc = len(text)
     if argc < 2:
         return
-    opt = tools.Identifier(text[1])
+    opt = bot.make_identifier(text[1])
     quietmask = opt
     channel = trigger.sender
     if not opt.is_nick():
         if argc < 3:
             return
         quietmask = text[2]
         channel = opt
-    quietmask = configureHostMask(quietmask)
-    if quietmask == '':
+
+    try:
+        quietmask = configureHostMask(quietmask)
+    except ValueError:
         return
+
     bot.write(['MODE', channel, '+q', quietmask])
 
 
 @plugin.require_chanmsg
 @plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV, reply=True)
 @plugin.require_bot_privilege(plugin.OP, ERROR_MESSAGE_NOT_OP, reply=True)
 @plugin.command('unquiet')
@@ -233,25 +254,28 @@
 
     The bot must be a channel operator for this command to work.
     """
     text = trigger.group().split()
     argc = len(text)
     if argc < 2:
         return
-    opt = tools.Identifier(text[1])
+    opt = bot.make_identifier(text[1])
     quietmask = opt
     channel = trigger.sender
     if not opt.is_nick():
         if argc < 3:
             return
         quietmask = text[2]
         channel = opt
-    quietmask = configureHostMask(quietmask)
-    if quietmask == '':
+
+    try:
+        quietmask = configureHostMask(quietmask)
+    except ValueError:
         return
+
     bot.write(['MODE', channel, '-q', quietmask])
 
 
 @plugin.require_chanmsg
 @plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV, reply=True)
 @plugin.require_bot_privilege(plugin.OP, ERROR_MESSAGE_NOT_OP, reply=True)
 @plugin.command('kickban', 'kb')
@@ -262,30 +286,33 @@
 
     The bot must be a channel operator for this command to work.
     """
     text = trigger.group().split()
     argc = len(text)
     if argc < 4:
         return
-    opt = tools.Identifier(text[1])
+    opt = bot.make_identifier(text[1])
     nick = opt
     mask = text[2]
     channel = trigger.sender
     reasonidx = 3
     if not opt.is_nick():
         if argc < 5:
             return
         channel = opt
         nick = text[2]
         mask = text[3]
         reasonidx = 4
     reason = ' '.join(text[reasonidx:])
-    mask = configureHostMask(mask)
-    if mask == '':
+
+    try:
+        mask = configureHostMask(mask)
+    except ValueError:
         return
+
     bot.write(['MODE', channel, '+b', mask])
     bot.kick(nick, channel, reason)
 
 
 @plugin.require_chanmsg
 @plugin.command('topic')
 def topic(bot, trigger):
@@ -300,17 +327,16 @@
     if mode_t and bot.channels[trigger.sender].privileges[trigger.nick] < plugin.HALFOP:
         bot.reply(ERROR_MESSAGE_NO_PRIV)
         return
     if not trigger.group(2):
         return
     channel = trigger.sender.lower()
 
-    mask = None
-    mask = bot.db.get_channel_value(channel, 'topic_mask')
-    mask = mask or default_mask(trigger)
+    mask = bot.db.get_channel_value(
+        channel, 'topic_mask', default_mask(trigger))
     mask = mask.replace('%s', '{}')
     narg = len(re.findall('{}', mask))
 
     top = trigger.group(2)
     args = []
     if top:
         args = top.split('~', narg)
@@ -331,32 +357,52 @@
                 "the server limit is {} bytes."
                 .format(my_len, topiclen))
             return
 
     bot.write(('TOPIC', channel + ' :' + topic))
 
 
-@plugin.require_chanmsg
 @plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV)
-@plugin.command('tmask')
-def set_mask(bot, trigger):
-    """Set the topic mask to use for the current channel
-
-    Within the topic mask, {} is used to allow substituting in chunks of text.
-
-    This mask is used when running the 'topic' command.
-    """
-    bot.db.set_channel_value(trigger.sender, 'topic_mask', trigger.group(2))
-    message = (
-        'Topic mask set. '
-        'Use `{prefix}topic <args>` to set topic '
-        'and `{prefix}showmask` to see current mask.'
-    ).format(prefix=bot.settings.core.help_prefix)
-    bot.reply(message)
+@plugin.commands('tmask set', 'tmask get', 'tmask clear', 'tmask')
+@plugin.example('.tmask clear', user_help=True)
+@plugin.example('.tmask get', user_help=True)
+@plugin.example('.tmask set My {} topic mask!', user_help=True)
+def topic_mask_management(bot, trigger):
+    """Set, get, or clear the current channel's topic mask.
+
+    Recognized subcommands are 'set', 'get', and 'clear'. A plain 'tmask'
+    command with no arguments is equivalent to 'tmask get'.
+
+    This mask is used by the 'topic' command. `{}` allows interpolating a chunk
+    of text within the topic mask template.
+    """
+    command, _, subcommand = trigger.group(1).partition(' ')
+
+    if not subcommand or subcommand == 'get':
+        mask = bot.db.get_channel_value(
+            trigger.sender, 'topic_mask', default_mask(trigger))
+        bot.reply('Current topic mask: {}'.format(mask))
+        return
+
+    if subcommand == 'set':
+        if not trigger.group(2):
+            message = (
+                'I need a non-empty topic mask to set. '
+                'To delete the saved topic mask, use `{prefix}tmask clear`.'
+            ).format(prefix=bot.settings.core.help_prefix)
+            bot.reply(message)
+            return
 
+        bot.db.set_channel_value(trigger.sender, 'topic_mask', trigger.group(2))
+        message = (
+            'Topic mask set. '
+            'Use `{prefix}topic <args>` to set topic, '
+            '`{prefix}tmask get` to see the current mask, '
+            'and `{prefix}tmask clear` to delete the saved topic mask.'
+        ).format(prefix=bot.settings.core.help_prefix)
+        bot.reply(message)
+        return
 
-@plugin.require_chanmsg
-@plugin.require_privilege(plugin.OP, ERROR_MESSAGE_NO_PRIV)
-@plugin.command('showmask')
-def show_mask(bot, trigger):
-    """Show the topic mask for the current channel."""
-    bot.say(bot.db.get_channel_value(trigger.sender, 'topic_mask', default_mask(trigger)))
+    if subcommand == 'clear':
+        bot.db.delete_channel_value(trigger.sender, 'topic_mask')
+        bot.reply('Cleared topic mask.')
+        return
```

### Comparing `sopel-7.1.9/sopel/modules/announce.py` & `sopel-8.0.0/sopel/builtins/announce.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# coding=utf-8
 """
 announce.py - Sopel Announcement Plugin
 Sends announcements to all channels the bot has joined.
 Copyright © 2013, Elad Alfassa, <elad@fedoraproject.org>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import itertools
 
 from sopel import plugin
 
 
 def _chunks(items, size):
@@ -22,20 +21,16 @@
     :param int size: the size of each chunk
     :return: a :term:`generator` of chunks
     :rtype: :term:`generator` of :class:`tuple`
     """
     # This approach is safer than slicing with non-subscriptable types,
     # for example `dict_keys` objects
     iterator = iter(items)
-    # TODO: Simplify to assignment expression (`while cond := expr`)
-    # when dropping Python 3.7
-    chunk = tuple(itertools.islice(iterator, size))
-    while chunk:
+    while (chunk := tuple(itertools.islice(iterator, size))):
         yield chunk
-        chunk = tuple(itertools.islice(iterator, size))
 
 
 @plugin.command('announce')
 @plugin.example('.announce Some important message here')
 @plugin.require_admin('Sorry, I can\'t let you do that', reply=True)
 @plugin.output_prefix('[ANNOUNCEMENT] ')
 def announce(bot, trigger):
```

### Comparing `sopel-7.1.9/sopel/modules/choose.py` & `sopel-8.0.0/sopel/builtins/choose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-# coding=utf-8
 """
 choose.py - Sopel Choice Plugin
 Copyright 2010-2013, Dimitri "Tyrope" Molenaars, TyRope.nl
 Copyright 2013, Ari Koivula, <ari@koivu.la>
 Copyright 2018, Florian Strzelecki, <florian.strzelecki@gmail.com>
 Copyright 2019, dgw, technobabbl.es
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import random
 import unicodedata
 
 from sopel import formatting, plugin
 
-# Remove when dropping py2 support
-try:
-    str = unicode
-except NameError:
-    pass
-
 
 def _format_safe(text):
     """Remove excess whitespace and terminate IRC formatting.
 
     :param str text: text to clean of whitespace
     :rtype: str
     :raises TypeError: if the passed ``text`` is not a string
```

### Comparing `sopel-7.1.9/sopel/modules/clock.py` & `sopel-8.0.0/sopel/builtins/clock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# coding=utf-8
 """clock.py - Sopel Clock Plugin
 
 Copyright 2008-9, Sean B. Palmer, inamidst.com
 Copyright 2012, Elsie Powell, embolalia.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-from sopel import plugin, tools
+from sopel import plugin
 from sopel.tools.time import (
     format_time,
     get_channel_timezone,
     get_nick_timezone,
     get_timezone,
     validate_timezone
 )
@@ -57,15 +56,15 @@
         # get default timezone from nick, or sender, or bot, or UTC
         zone = get_timezone(
             bot.db, bot.config, None, trigger.nick, trigger.sender)
     else:
         # guess if the argument is a nick, a channel, or a timezone
         zone = None
         argument = argument.strip()
-        channel_or_nick = tools.Identifier(argument)
+        channel_or_nick = bot.make_identifier(argument)
 
         # first, try to get nick or channel's timezone
         help_prefix = bot.config.core.help_prefix
         if channel_or_nick.is_nick():
             zone = get_nick_timezone(bot.db, channel_or_nick)
             if zone is None and channel_or_nick in bot.users:
                 # zone not found for a known nick: error case
@@ -156,14 +155,22 @@
         bot.reply(
             'Okay, but you should use one from https://sopel.chat/tz '
             'if you use DST.')
     else:
         bot.reply('I now have you in the %s timezone.' % zone)
 
 
+@plugin.command('unsettz', 'unsettimezone')
+@plugin.example('.unsettz')
+def unset_user_tz(bot, trigger):
+    """Unset your preferred timezone."""
+    bot.db.delete_nick_value(trigger.nick, 'timezone')
+    bot.reply('Successfully unset timezone')
+
+
 @plugin.command('gettz', 'gettimezone')
 @plugin.example('.gettz Exirel', user_help=True)
 @plugin.example('.gettz', user_help=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def get_user_tz(bot, trigger):
     """Gets a user's preferred time zone.
 
@@ -213,14 +220,22 @@
 
     set_command = '%ssettz' % bot.settings.core.help_prefix
     bot.reply('Your time will now appear as %s. '
               '(If the timezone is wrong, you might try the %s command)'
               % (timef, set_command))
 
 
+@plugin.command('unsettimeformat', 'unsettf')
+@plugin.example('.unsettf')
+def unset_user_format(bot, trigger):
+    """Unsets your preferred format for time."""
+    bot.db.delete_nick_value(trigger.nick, 'time_format')
+    bot.reply('Successfully unset time format')
+
+
 @plugin.command('gettimeformat', 'gettf')
 @plugin.example('.gettf Exirel', user_help=True)
 @plugin.example('.gettf', user_help=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def get_user_format(bot, trigger):
     """Gets a user's preferred time format.
 
@@ -265,14 +280,25 @@
         bot.reply(
             'Okay, but you should use one from https://sopel.chat/tz '
             'if you use DST.')
     else:
         bot.reply('I now have %s in the %s timezone.' % (channel, zone))
 
 
+@plugin.command('unsetchanneltz', 'unsetctz')
+@plugin.example('.unsetctz')
+@plugin.require_chanmsg
+@plugin.require_privilege(plugin.OP, message='Changing the channel timezone requires OP privileges.')
+def unset_channel(bot, trigger):
+    """Unset the preferred timezone for the current channel."""
+    channel = trigger.sender
+    bot.db.delete_channel_value(channel, 'timezone')
+    bot.reply('Successfully unset channel timezone')
+
+
 @plugin.command('getchanneltz', 'getctz')
 @plugin.example('.getctz #sopel', user_help=True)
 @plugin.example('.getctz', user_help=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def get_channel_tz(bot, trigger):
     """Gets the channel's preferred timezone.
 
@@ -329,14 +355,25 @@
     channel_command = '%schanneltz' % help_prefix
     bot.say("Times in this channel will now appear as %s "
             "unless a user has their own format set. (If the timezone"
             " is wrong, you might try the %s and %s "
             "commands)" % (timef, set_command, channel_command))
 
 
+@plugin.command('unsetchanneltimeformat', 'unsetctf')
+@plugin.example('.unsetctf')
+@plugin.require_chanmsg
+@plugin.require_privilege(plugin.OP, message='Changing the channel time format requires OP privileges.')
+def unset_channel_format(bot, trigger):
+    """Unset the preferred time format for the current channel."""
+    channel = trigger.sender
+    bot.db.delete_channel_value(channel, 'time_format')
+    bot.reply('Successfully unset channel time format')
+
+
 @plugin.command('getchanneltimeformat', 'getctf')
 @plugin.example('.getctf #sopel', user_help=True)
 @plugin.example('.getctf', user_help=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def get_channel_format(bot, trigger):
     """Gets the channel's preferred time format
```

### Comparing `sopel-7.1.9/sopel/modules/countdown.py` & `sopel-8.0.0/sopel/builtins/countdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding=utf-8
 """
 countdown.py - Sopel Countdown Plugin
 Copyright 2011, Michael Yanovich, yanovich.net
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import datetime
 
 from sopel import plugin
 
 
 @plugin.command('countdown')
```

### Comparing `sopel-7.1.9/sopel/modules/currency.py` & `sopel-8.0.0/sopel/builtins/currency.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-# coding=utf-8
 """
 currency.py - Sopel Currency Conversion Plugin
 Copyright 2013, Elsie Powell, embolalia.com
 Copyright 2019, Mikkel Jeppesen
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import logging
 import re
 import time
 
 import requests
 
 from sopel import plugin
 from sopel.config import types
 from sopel.tools import web
 
 
 PLUGIN_OUTPUT_PREFIX = '[currency] '
 FIAT_PROVIDERS = {
-    'exchangerate.host': 'https://api.exchangerate.host/latest?base=EUR',
+    'open.er-api.com': 'https://open.er-api.com/v6/latest/EUR',
     'fixer.io': '//data.fixer.io/api/latest?base=EUR&access_key={}',
 }
 CRYPTO_URL = 'https://api.coingecko.com/api/v3/exchange_rates'
 EXCHANGE_REGEX = re.compile(r'''
     ^(\d+(?:\.\d+)?)                                            # Decimal number
     \s*([a-zA-Z]{3})                                            # 3-letter currency code
     \s+(?:in|as|of|to)\s+                                       # preposition
     (([a-zA-Z]{3}$)|([a-zA-Z]{3})\s)+$                          # one or more 3-letter currency code
 ''', re.VERBOSE)
 LOGGER = logging.getLogger(__name__)
 UNSUPPORTED_CURRENCY = "Sorry, {} isn't currently supported."
 UNRECOGNIZED_INPUT = "Sorry, I didn't understand the input."
 
-rates = {}
+rates: dict[str, float] = {}
 rates_updated = 0.0
 
 
 class CurrencySection(types.StaticSection):
-    fiat_provider = types.ChoiceAttribute('fiat_provider',
-                                          list(FIAT_PROVIDERS.keys()),
-                                          default='exchangerate.host')
+    fiat_provider = types.ChoiceAttribute(
+        'fiat_provider',
+        list(FIAT_PROVIDERS.keys()),
+        default='open.er-api.com',
+    )
     """Which data provider to use (some of which require no API key)"""
     fixer_io_key = types.ValidatedAttribute('fixer_io_key', default=None)
     """API key for Fixer.io (widest currency support)"""
     fixer_use_ssl = types.BooleanAttribute('fixer_use_ssl', default=False)
     """Whether to use SSL (HTTPS) for Fixer API"""
     auto_convert = types.BooleanAttribute('auto_convert', default=False)
     """Whether to convert currencies without an explicit command"""
@@ -66,38 +67,37 @@
     config.currency.configure_setting(
         'fiat_provider',
         'Which exchange rate provider do you want to use?\n'
         'Available choices: {}'.format(
             ', '.join(FIAT_PROVIDERS.keys())
         ))
     if config.currency.fiat_provider == 'fixer.io':
-        config.currency.configure_setting('fixer_io_key', 'API key for Fixer.io:')
-        config.currency.configure_setting('fixer_use_ssl', 'Use SSL (paid plans only) for Fixer.io?')
-    elif config.currency.fixer_io_key is not None:
-        # Must be unset or it will override the chosen fiat_provider
-        # TODO: this is temporary for Sopel 7.x; see below
-        print('Chosen provider is {}; clearing Fixer.io API key.'.format(config.currency.fiat_provider))
-        config.currency.fixer_io_key = None
-    config.currency.configure_setting('auto_convert', 'Convert currencies without an explicit command?')
+        config.currency.configure_setting(
+            'fixer_io_key', 'API key for Fixer.io:')
+        config.currency.configure_setting(
+            'fixer_use_ssl', 'Use SSL (paid plans only) for Fixer.io?')
+
+    config.currency.configure_setting(
+        'auto_convert', 'Convert currencies without an explicit command?')
 
 
 def setup(bot):
     bot.config.define_section('currency', CurrencySection)
 
 
 class FixerError(Exception):
     """A Fixer.io API Error Exception"""
     def __init__(self, status):
-        super(FixerError, self).__init__("FixerError: {}".format(status))
+        super().__init__("FixerError: {}".format(status))
 
 
 class UnsupportedCurrencyError(Exception):
     """A currency is currently not supported by the API"""
     def __init__(self, currency):
-        super(UnsupportedCurrencyError, self).__init__(currency)
+        super().__init__(currency)
 
 
 def build_reply(amount, base, target, out_string):
     rate_raw = get_rate(base, target)
     rate = float(rate_raw)
     result = float(rate * amount)
 
@@ -133,23 +133,15 @@
         ))
         return
     except FixerError as err:
         bot.reply('Sorry, something went wrong with Fixer')
         LOGGER.error(err)
         return
 
-    query = match.string
-
-    targets = query.split()
-    amount_in = targets.pop(0)
-    base = targets.pop(0)
-    targets.pop(0)
-
-    # TODO: Use this instead after dropping Python 2 support
-    # amount, base, _, *targets = query.split()
+    amount_in, base, _, *targets = match.string.split()
 
     try:
         amount = float(amount_in)
     except ValueError:
         bot.reply(UNRECOGNIZED_INPUT)
         return
     except OverflowError:
@@ -211,36 +203,37 @@
     # Update crypto rates
     LOGGER.debug('Updating crypto rates from %s', CRYPTO_URL)
     response = requests.get(CRYPTO_URL)
     response.raise_for_status()
     rates_crypto = response.json()
 
     # Update fiat rates
-    if bot.config.currency.fixer_io_key is not None:
+    fiat_provider = bot.settings.currency.fiat_provider
+    fixer_io_key = bot.settings.currency.fixer_io_key
+    fixer_use_ssl = bot.settings.currency.fixer_use_ssl
+
+    if fiat_provider == 'fixer.io':
         LOGGER.debug('Updating fiat rates from Fixer.io')
-        if bot.config.currency.fiat_provider != 'fixer.io':
-            # Warning about future behavior change
-            LOGGER.warning(
-                'fiat_provider is set to %s, but Fixer.io API key is present; '
-                'using Fixer anyway. In Sopel 8, fiat_provider will take precedence.',
-                bot.config.currency.fiat_provider)
+        if not fixer_io_key:
+            raise FixerError('Fixer.io requires an API key.')
 
-        proto = 'https:' if bot.config.currency.fixer_use_ssl else 'http:'
+        proto = 'https:' if fixer_use_ssl else 'http:'
         response = requests.get(
             proto +
-            FIAT_PROVIDERS['fixer.io'].format(
-                web.quote(bot.config.currency.fixer_io_key)
-            )
+            FIAT_PROVIDERS['fixer.io'].format(web.quote(fixer_io_key))
         )
 
         if not response.json()['success']:
-            raise FixerError('Fixer.io request failed with error: {}'.format(response.json()['error']))
+            error_message = response.json()['error']
+            raise FixerError(
+                'Fixer.io request failed with error: {}'.format(error_message),
+            )
     else:
-        LOGGER.debug('Updating fiat rates from %s', bot.config.currency.fiat_provider)
-        response = requests.get(FIAT_PROVIDERS[bot.config.currency.fiat_provider])
+        LOGGER.debug('Updating fiat rates from %s', fiat_provider)
+        response = requests.get(FIAT_PROVIDERS[fiat_provider])
 
     response.raise_for_status()
     rates_fiat = response.json()
 
     rates = rates_fiat['rates']
     rates['EUR'] = 1.0  # Put this here to make logic easier
 
@@ -252,15 +245,15 @@
 
     # if an error aborted the operation prematurely, we want the next call to retry updating rates
     # therefore we'll update the stored timestamp at the last possible moment
     rates_updated = time.time()
     LOGGER.debug('Rate update completed')
 
 
-@plugin.command('cur', 'currency', 'exchange')
+@plugin.commands('cur', 'currency', 'exchange')
 @plugin.example('.cur 100 usd in btc cad eur',
                 r'100 USD is [\d\.]+ BTC, [\d\.]+ CAD, [\d\.]+ EUR',
                 re=True, online=True, vcr=True)
 @plugin.example('.cur 100 usd in btc cad eur can aux',
                 r'100 USD is [\d\.]+ BTC, [\d\.]+ CAD, [\d\.]+ EUR, \(unsupported: CAN, AUX\)',
                 re=True, online=True, vcr=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
@@ -278,7 +271,25 @@
 @plugin.rule(EXCHANGE_REGEX)
 @plugin.example('100 usd in btc cad eur')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def exchange_re(bot, trigger):
     if bot.config.currency.auto_convert:
         match = EXCHANGE_REGEX.match(trigger)
         exchange(bot, match)
+
+
+@plugin.command('currencies')
+@plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
+def supported_cmd(bot, trigger):
+    """List which currency codes are supported for conversion."""
+    if not rates:
+        try:
+            update_rates(bot)
+        except Exception:
+            bot.reply("Couldn't fetch supported currencies. Please try again later.")
+            return
+
+    codes = sorted(list(rates.keys()))
+
+    bot.say(
+        "Supported currency codes: " + ' '.join(codes),
+        trigger.nick, max_messages=5)
```

### Comparing `sopel-7.1.9/sopel/modules/dice.py` & `sopel-8.0.0/sopel/builtins/dice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-# coding=utf-8
 """
 dice.py - Sopel Dice Plugin
 Copyright 2010-2013, Dimitri "Tyrope" Molenaars, TyRope.nl
 Copyright 2013, Ari Koivula, <ari@koivu.la>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import operator
 import random
 import re
+from typing import TYPE_CHECKING
 
 from sopel import plugin
 from sopel.tools.calculation import eval_equation
 
+if TYPE_CHECKING:
+    from sopel.bot import SopelWrapper
+    from sopel.trigger import Trigger
+
+
+MAX_DICE = 1000
+
 
 class DicePouch:
-    def __init__(self, num_of_die, type_of_die, addition):
+    def __init__(self, dice_count: int, dice_type: int) -> None:
         """Initialize dice pouch and roll the dice.
 
-        Args:
-            num_of_die: number of dice in the pouch.
-            type_of_die: how many faces the dice have.
-            addition: how much is added to the result of the dice.
+        :param dice_count: the number of dice in the pouch
+        :param dice_type: how many faces each die has
         """
-        self.num = num_of_die
-        self.type = type_of_die
-        self.addition = addition
+        self.num: int = dice_count
+        self.type: int = dice_type
 
-        self.dice = {}
-        self.dropped = {}
+        self.dice: dict[int, int] = {}
+        self.dropped: dict[int, int] = {}
 
         self.roll_dice()
 
-    def roll_dice(self):
+    def roll_dice(self) -> None:
         """Roll all the dice in the pouch."""
         self.dice = {}
         self.dropped = {}
         for __ in range(self.num):
             number = random.randint(1, self.type)
             count = self.dice.setdefault(number, 0)
             self.dice[number] = count + 1
 
-    def drop_lowest(self, n):
-        """Drop n lowest dice from the result.
+    def drop_lowest(self, n: int) -> None:
+        """Drop ``n`` lowest dice from the result.
 
-        Args:
-            n: the number of dice to drop.
+        :param n: the number of dice to drop
         """
 
         sorted_x = sorted(self.dice.items(), key=operator.itemgetter(0))
 
         for i, count in sorted_x:
             count = self.dice[i]
             if n == 0:
@@ -66,181 +69,257 @@
                 self.dropped[i] = count
                 n = n - count
 
         for i, count in self.dropped.items():
             if self.dice[i] == 0:
                 del self.dice[i]
 
-    def get_simple_string(self):
-        """Return the values of the dice like (2+2+2[+1+1])+1."""
+    def get_simple_string(self) -> str:
+        """Return the values of the dice like (2+2+2[+1+1])."""
         dice = self.dice.items()
         faces = ("+".join([str(face)] * times) for face, times in dice)
         dice_str = "+".join(faces)
 
         dropped_str = ""
         if self.dropped:
             dropped = self.dropped.items()
             dfaces = ("+".join([str(face)] * times) for face, times in dropped)
             dropped_str = "[+%s]" % ("+".join(dfaces),)
 
-        plus_str = ""
-        if self.addition:
-            plus_str = "{:+d}".format(self.addition)
-
-        return "(%s%s)%s" % (dice_str, dropped_str, plus_str)
+        return "(%s%s)" % (dice_str, dropped_str)
 
-    def get_compressed_string(self):
-        """Return the values of the dice like (3x2[+2x1])+1."""
+    def get_compressed_string(self) -> str:
+        """Return the values of the dice like (3x2[+2x1])."""
         dice = self.dice.items()
         faces = ("%dx%d" % (times, face) for face, times in dice)
         dice_str = "+".join(faces)
 
         dropped_str = ""
         if self.dropped:
             dropped = self.dropped.items()
             dfaces = ("%dx%d" % (times, face) for face, times in dropped)
             dropped_str = "[+%s]" % ("+".join(dfaces),)
 
-        plus_str = ""
-        if self.addition:
-            plus_str = "{:+d}".format(self.addition)
-
-        return "(%s%s)%s" % (dice_str, dropped_str, plus_str)
-
-    def get_sum(self):
-        """Get the sum of non-dropped dice and the addition."""
-        result = self.addition
+        return "(%s%s)" % (dice_str, dropped_str)
+
+    def get_sum(self) -> int:
+        """Get the sum of non-dropped dice."""
+        result = 0
         for face, times in self.dice.items():
             result += face * times
         return result
 
-    def get_number_of_faces(self):
-        """Returns sum of different faces for dropped and not dropped dice
+    def get_number_of_faces(self) -> int:
+        """Returns sum of different faces for dropped and not dropped dice.
 
-        This can be used to estimate, whether the result can be shown in
-        compressed form in a reasonable amount of space.
+        This can be used to estimate whether the result can be shown (in
+        compressed form) in a reasonable amount of space.
         """
         return len(self.dice) + len(self.dropped)
 
 
-def _roll_dice(bot, dice_expression):
-    result = re.search(
-        r"""
-        (?P<dice_num>-?\d*)
-        d
-        (?P<dice_type>-?\d+)
-        (v(?P<drop_lowest>-?\d+))?
-        $""",
-        dice_expression,
-        re.IGNORECASE | re.VERBOSE)
+class DiceError(Exception):
+    """Custom base exception type."""
+
+
+class InvalidDiceFacesError(DiceError):
+    """Custom exception type for invalid number of die faces."""
+    def __init__(self, faces: int):
+        super().__init__(faces)
+
+    @property
+    def faces(self) -> int:
+        return self.args[0]
+
+
+class NegativeDiceCountError(DiceError):
+    """Custom exception type for invalid numbers of dice."""
+    def __init__(self, count: int):
+        super().__init__(count)
+
+    @property
+    def count(self) -> int:
+        return self.args[0]
+
+
+class TooManyDiceError(DiceError):
+    """Custom exception type for excessive numbers of dice."""
+    def __init__(self, requested: int, available: int):
+        super().__init__(requested, available)
+
+    @property
+    def available(self) -> int:
+        return self.args[1]
+
+    @property
+    def requested(self) -> int:
+        return self.args[0]
 
-    dice_num = int(result.group('dice_num') or 1)
-    dice_type = int(result.group('dice_type'))
+
+class UnableToDropDiceError(DiceError):
+    """Custom exception type for failing to drop lowest N dice."""
+    def __init__(self, dropped: int, total: int):
+        super().__init__(dropped, total)
+
+    @property
+    def dropped(self) -> int:
+        return self.args[0]
+
+    @property
+    def total(self) -> int:
+        return self.args[1]
+
+
+def _get_error_message(exc: DiceError) -> str:
+    if isinstance(exc, InvalidDiceFacesError):
+        return "I don't have any dice with {} sides.".format(exc.faces)
+    if isinstance(exc, NegativeDiceCountError):
+        return "I can't roll {} dice.".format(exc.count)
+    if isinstance(exc, TooManyDiceError):
+        return "I only have {}/{} dice.".format(exc.available, exc.requested)
+    if isinstance(exc, UnableToDropDiceError):
+        return "I can't drop the lowest {} of {} dice.".format(
+            exc.dropped, exc.total)
+
+    return "Unknown error rolling dice: %r" % exc
+
+
+def _roll_dice(dice_match: re.Match[str]) -> DicePouch:
+    dice_num = int(dice_match.group('dice_num') or 1)
+    dice_type = int(dice_match.group('dice_type'))
 
     # Dice can't have zero or a negative number of sides.
     if dice_type <= 0:
-        bot.reply("I don't have any dice with %d sides. =(" % dice_type)
-        return None  # Signal there was a problem
+        raise InvalidDiceFacesError(dice_type)
 
     # Can't roll a negative number of dice.
     if dice_num < 0:
-        bot.reply("I'd rather not roll a negative amount of dice. =(")
-        return None  # Signal there was a problem
+        raise NegativeDiceCountError(dice_num)
 
     # Upper limit for dice should be at most a million. Creating a dict with
     # more than a million elements already takes a noticeable amount of time
     # on a fast computer and ~55kB of memory.
-    if dice_num > 1000:
-        bot.reply('I only have 1000 dice. =(')
-        return None  # Signal there was a problem
+    if dice_num > MAX_DICE:
+        raise TooManyDiceError(dice_num, MAX_DICE)
 
-    dice = DicePouch(dice_num, dice_type, 0)
+    dice = DicePouch(dice_num, dice_type)
 
-    if result.group('drop_lowest'):
-        drop = int(result.group('drop_lowest'))
+    if dice_match.group('drop_lowest'):
+        drop = int(dice_match.group('drop_lowest'))
         if drop >= 0:
             dice.drop_lowest(drop)
         else:
-            bot.reply("I can't drop the lowest %d dice. =(" % drop)
+            raise UnableToDropDiceError(drop, dice_num)
 
     return dice
 
 
 @plugin.command('roll', 'dice', 'd')
 @plugin.priority("medium")
+@plugin.example(".roll", "No dice to roll.")
+@plugin.example(".roll 2d6+4^2&",
+                "I don't know how to process that. "
+                "Are the dice as well as the algorithms correct?")
+@plugin.example(".roll 65(2)", "I couldn't find any valid dice expressions.")
+@plugin.example(".roll 2d-2", "I don't have any dice with -2 sides.")
+@plugin.example(".roll 1d0", "I don't have any dice with 0 sides.")
+@plugin.example(".roll -1d6", "I can't roll -1 dice.")
+@plugin.example(".roll 3d6v-1", "I can't drop the lowest -1 of 3 dice.")
+@plugin.example(".roll 2d6v0", r'2d6v0: \(\d\+\d\) = \d+', re=True)
+@plugin.example(".roll 2d6v4", r'2d6v4: \(\[\+\d\+\d\]\) = 0', re=True)
+@plugin.example(".roll 2d6v1+8", r'2d6v1\+8: \(\d\[\+\d\]\)\+8 = \d+', re=True)
+@plugin.example(".roll 11d1v1", "11d1v1: (10x1[+1x1]) = 10")
 @plugin.example(".roll 3d1+1", '3d1+1: (1+1+1)+1 = 4')
 @plugin.example(".roll 3d1v2+1", '3d1v2+1: (1[+1+1])+1 = 2')
 @plugin.example(".roll 2d4", r'2d4: \(\d\+\d\) = \d', re=True)
 @plugin.example(".roll 100d1", r'[^:]*: \(100x1\) = 100', re=True)
-@plugin.example(".roll 1001d1", 'I only have 1000 dice. =(')
+@plugin.example(".roll 100d100", r'100d100: \(\.{3}\) = \d+', re=True)
+@plugin.example(".roll 1000d999^1000d999", 'You roll 1000d999^1000d999: (...)^(...) = very big')
+@plugin.example(".roll 1000d999^1000d99", "I can't display a number that big. =(")
+@plugin.example(
+    ".roll {}d1".format(MAX_DICE + 1), 'I only have {}/{} dice.'.format(MAX_DICE, MAX_DICE + 1))
 @plugin.example(".roll 1d1 + 1d1", '1d1 + 1d1: (1) + (1) = 2')
 @plugin.example(".roll 1d1+1d1", '1d1+1d1: (1)+(1) = 2')
-@plugin.example(".roll 1d6 # initiative", r'1d6: \(\d\) = \d', re=True)
+@plugin.example(".roll d6 # initiative", r'd6: \(\d\) = \d', re=True)
 @plugin.example(".roll 2d20v1+2 # roll with advantage", user_help=True)
 @plugin.example(".roll 2d10+3", user_help=True)
 @plugin.example(".roll 1d6", user_help=True)
 @plugin.output_prefix('[dice] ')
-def roll(bot, trigger):
+def roll(bot: SopelWrapper, trigger: Trigger):
     """Rolls dice and reports the result.
 
     The dice roll follows this format: XdY[vZ][+N][#COMMENT]
 
     X is the number of dice. Y is the number of faces in the dice. Z is the
     number of lowest dice to be dropped from the result. N is the constant to
     be applied to the end result. Comment is for easily noting the purpose.
     """
-    # This regexp is only allowed to have one capture group, because having
-    # more would alter the output of re.findall.
-    dice_regexp = r"-?\d*[dD]-?\d+(?:[vV]-?\d+)?"
+    dice_regexp = r"""
+        (?P<dice_num>-?\d*)
+        d
+        (?P<dice_type>-?\d+)
+        (v(?P<drop_lowest>-?\d+))?
+    """
 
     # Get a list of all dice expressions, evaluate them and then replace the
     # expressions in the original string with the results. Replacing is done
     # using string formatting, so %-characters must be escaped.
     if not trigger.group(2):
         bot.reply("No dice to roll.")
         return
+
     arg_str_raw = trigger.group(2).split("#", 1)[0].strip()
-    dice_expressions = re.findall(dice_regexp, arg_str_raw)
     arg_str = arg_str_raw.replace("%", "%%")
-    arg_str = re.sub(dice_regexp, "%s", arg_str)
+    arg_str = re.sub(dice_regexp, "%s", arg_str, 0, re.IGNORECASE | re.VERBOSE)
 
-    dice = [_roll_dice(bot, dice_expr) for dice_expr in dice_expressions]
+    dice_expressions = [
+        match for match in
+        re.finditer(dice_regexp, arg_str_raw, re.IGNORECASE | re.VERBOSE)
+    ]
+
+    if not dice_expressions:
+        bot.reply("I couldn't find any valid dice expressions.")
+        return
 
-    if None in dice:
+    try:
+        dice = [_roll_dice(dice_expr) for dice_expr in dice_expressions]
+    except DiceError as err:
         # Stop computing roll if there was a problem rolling dice.
+        bot.reply(_get_error_message(err))
         return
 
-    def _get_eval_str(dice):
+    def _get_eval_str(dice: DicePouch) -> str:
         return "(%d)" % (dice.get_sum(),)
 
-    def _get_pretty_str(dice):
+    def _get_pretty_str(dice: DicePouch) -> str:
         if dice.num <= 10:
             return dice.get_simple_string()
         elif dice.get_number_of_faces() <= 10:
             return dice.get_compressed_string()
         else:
             return "(...)"
 
-    eval_str = arg_str % (tuple(map(_get_eval_str, dice)))
-    pretty_str = arg_str % (tuple(map(_get_pretty_str, dice)))
+    eval_str: str = arg_str % (tuple(map(_get_eval_str, dice)))
+    pretty_str: str = arg_str % (tuple(map(_get_pretty_str, dice)))
 
     try:
         result = eval_equation(eval_str)
-    except TypeError:
-        bot.reply(
-            "The type of this equation is, apparently, not a string. "
-            "How did you do that, anyway?"
-        )
     except ValueError:
         # As it seems that ValueError is raised if the resulting equation would
         # be too big, give a semi-serious answer to reflect on this.
         bot.reply("You roll %s: %s = very big" % (
             arg_str_raw, pretty_str))
         return
     except (SyntaxError, eval_equation.Error):
         bot.reply(
             "I don't know how to process that. "
             "Are the dice as well as the algorithms correct?"
         )
         return
 
-    bot.say("%s: %s = %d" % (arg_str_raw, pretty_str, result))
+    try:
+        bot.say("%s: %s = %d" % (arg_str_raw, pretty_str, result))
+    except ValueError:
+        # Converting the result to a string can also raise ValueError if it has
+        # more than int_max_str_digits digits (4300 by default on CPython)
+        # See https://docs.python.org/3.12/library/stdtypes.html#int-max-str-digits
+        bot.reply("I can't display a number that big. =(")
```

### Comparing `sopel-7.1.9/sopel/modules/emoticons.py` & `sopel-8.0.0/sopel/builtins/emoticons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding=utf-8
 """
 emoticons.py - Sopel Emoticons Plugin
 Copyright 2018, brasstax
 Licensed under the Eiffel Forum License 2
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 from sopel import plugin
 
 
 @plugin.command('shrug')
 @plugin.action_command('shrugs')
 @plugin.example('.shrug', r'¯\_(ツ)_/¯')
@@ -35,19 +34,19 @@
 @plugin.action_command('flips table', 'flips a table', 'flips the table')
 @plugin.example('.tableflip', '(╯°□°）╯︵ ┻━┻')
 @plugin.example('.tflip', '(╯°□°）╯︵ ┻━┻')
 def tableflip(bot, trigger):
     bot.say('(╯°□°）╯︵ ┻━┻')
 
 
-@plugin.command('unflip')
+@plugin.command('unflip', 'tback')
 @plugin.action_command('unflips table', 'unflips the table')
-@plugin.example('.unflip', '┬┬ ﻿ノ( ゜-゜ノ)')
+@plugin.example('.unflip', '┳━┳ ﻿ノ( ゜-゜ノ)')
 def unflip(bot, trigger):
-    bot.say('┬┬ ﻿ノ( ゜-゜ノ)')
+    bot.say('┳━┳ ﻿ノ( ゜-゜ノ)')
 
 
 @plugin.command('lenny')
 @plugin.example('.lenny', '( ͡° ͜ʖ ͡°)')
 def lenny(bot, trigger):
     bot.say('( ͡° ͜ʖ ͡°)')
```

### Comparing `sopel-7.1.9/sopel/modules/find.py` & `sopel-8.0.0/sopel/builtins/find.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-# coding=utf-8
 """
 find.py - Sopel Spelling Correction Plugin
 This plugin will fix spelling errors if someone corrects them
 using the sed notation (s///) commonly found in vi/vim.
 
 Copyright 2011, Michael Yanovich, yanovich.net
 Copyright 2013, Elsie Powell, embolalia.com
 Copyright 2020, dgw, technobabbl.es
 Includes contributions from: Matt Meinwald, and Morgan Goose
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 from collections import deque
 import re
 
 from sopel import plugin
 from sopel.formatting import bold
-from sopel.tools import Identifier, SopelIdentifierMemory
 
 
 def setup(bot):
     if 'find_lines' not in bot.memory:
-        bot.memory['find_lines'] = SopelIdentifierMemory()
+        bot.memory['find_lines'] = bot.make_identifier_memory()
 
 
 def shutdown(bot):
     try:
         del bot.memory['find_lines']
     except KeyError:
         pass
@@ -37,30 +35,31 @@
 @plugin.echo
 @plugin.rule('.*')
 @plugin.priority('low')
 @plugin.require_chanmsg
 @plugin.unblockable
 def collectlines(bot, trigger):
     """Create a temporary log of what people say"""
+    line = trigger.group()
+    if line.startswith('s/') or line.startswith('s|'):
+        # Don't remember substitutions
+        return
+
     # Add a log for the channel and nick, if there isn't already one
     if trigger.sender not in bot.memory['find_lines']:
-        bot.memory['find_lines'][trigger.sender] = SopelIdentifierMemory()
+        bot.memory['find_lines'][trigger.sender] = bot.make_identifier_memory()
     if trigger.nick not in bot.memory['find_lines'][trigger.sender]:
         bot.memory['find_lines'][trigger.sender][trigger.nick] = deque(maxlen=10)
 
     # Update in-memory list of the user's lines in the channel
     line_list = bot.memory['find_lines'][trigger.sender][trigger.nick]
-    line = trigger.group()
-    if line.startswith('s/') or line.startswith('s|'):
-        # Don't remember substitutions
-        return
-    # store messages in reverse order (most recent first)
-    elif line.startswith('\x01ACTION'):  # For /me messages
-        line = line[:-1]
-        line_list.appendleft(line)
+
+    # Messages are stored in reverse order (most recent first)
+    if line.startswith('\x01ACTION'):
+        line_list.appendleft(line[:-1])
     else:
         line_list.appendleft(line)
 
 
 def _cleanup_channel(bot, channel):
     bot.memory['find_lines'].pop(channel, None)
 
@@ -99,66 +98,66 @@
 
 @plugin.echo
 @plugin.event('KICK')
 @plugin.priority('low')
 @plugin.unblockable
 def kick_cleanup(bot, trigger):
     """Clean up cached data when a user is kicked from a channel."""
-    nick = Identifier(trigger.args[1])
+    nick = bot.make_identifier(trigger.args[1])
     if nick == bot.nick:
         # We got kicked! Nuke the whole channel.
         _cleanup_channel(bot, trigger.sender)
     else:
         # Clean up after the poor sod (or more likely, spammer) who got the boot
         _cleanup_nickname(bot, nick, trigger.sender)
 
 
 # Match nick, s/find/replace/flags. Flags and nick are optional, nick can be
 # followed by comma or colon, anything after the first space after the third
 # slash is ignored, and you can use either a slash or a pipe.
 # If you want to search for an actual slash AND a pipe in the same message,
 # you can escape your separator, in old and/or new.
 @plugin.rule(r"""(?:
-             (?P<nick>\S+)    # Catch a nick in group 1
-             [:,]\s+)?        # Followed by optional colon/comma and whitespace
-             s(?P<sep>/)      # The literal s and a separator / as group 2
-             (?P<old>         # Group 3 is the thing to find
-               (?:\\/|[^/])+  # One or more non-slashes or escaped slashes
+             (?P<nick>\S+)     # Catch a nick in group 1
+             [:,]\s+)?         # Followed by optional colon/comma and whitespace
+             s(?P<sep>/)       # The literal s and a separator / as group 2
+             (?P<old>          # Group 3 is the thing to find
+               (?:\\/|[^/])+   # One or more non-slashes or escaped slashes
              )
-             /                # The separator again
-             (?P<new>         # Group 4 is what to replace with
-               (?:\\/|[^/])*  # One or more non-slashes or escaped slashes
+             /                 # The separator again
+             (?P<new>          # Group 4 is what to replace with
+               (?:\\/|[^/])*   # One or more non-slashes or escaped slashes
              )
-             (?:/             # Optional separator followed by group 5 (flags)
+             (?:/              # Optional separator followed by group 5 (flags)
                 (?P<flags>\S+)
              )?
             """)
 @plugin.rule(r"""(?:
-             (?P<nick>\S+)    # Catch a nick in group 1
-             [:,]\s+)?        # Followed by optional colon/comma and whitespace
-             s(?P<sep>\|)     # The literal s and a separator | as group 2
-             (?P<old>         # Group 3 is the thing to find
+             (?P<nick>\S+)     # Catch a nick in group 1
+             [:,]\s+)?         # Followed by optional colon/comma and whitespace
+             s(?P<sep>\|)      # The literal s and a separator | as group 2
+             (?P<old>          # Group 3 is the thing to find
                (?:\\\||[^|])+  # One or more non-pipe or escaped pipe
              )
-             \|               # The separator again
-             (?P<new>         # Group 4 is what to replace with
-               (?:\\\||[^|])* # One or more non-pipe or escaped pipe
+             \|                # The separator again
+             (?P<new>          # Group 4 is what to replace with
+               (?:\\\||[^|])*  # One or more non-pipe or escaped pipe
              )
-             (?:|             # Optional separator followed by group 5 (flags)
+             (?:\|             # Optional separator followed by group 5 (flags)
                 (?P<flags>\S+)
              )?
             """)
 @plugin.priority('high')
 def findandreplace(bot, trigger):
     # Don't bother in PM
     if trigger.is_privmsg:
         return
 
     # Correcting other person vs self.
-    rnick = Identifier(trigger.group('nick') or trigger.nick)
+    rnick = bot.make_identifier(trigger.group('nick') or trigger.nick)
 
     # only do something if there is conversation to work with
     history = bot.memory['find_lines'].get(trigger.sender, {}).get(rnick, None)
     if not history:
         return
 
     sep = trigger.group('sep')
```

### Comparing `sopel-7.1.9/sopel/modules/find_updates.py` & `sopel-8.0.0/sopel/builtins/find_updates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# coding=utf-8
 """
 find_updates.py - Sopel Update Check Plugin
 This is separated from version.py, so that it can be easily overridden by
 distribution packagers, and they can check their repositories rather than the
 Sopel website.
 Copyright 2014, Elsie Powell, embolalia.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
+
+import json
 
 import requests
 
 from sopel import (
     __version__ as current_version,
     _version_info,
     plugin,
@@ -49,28 +50,28 @@
 def _check_failed(bot):
     bot.memory['update_failures'] = 1 + bot.memory.get('update_failures', 0)
 
 
 @plugin.interval(wait_time)
 def check_version(bot):
     version = version_info
+    r = None
     success = False
 
     try:
         r = requests.get(version_url, timeout=(5, 5))
     except requests.exceptions.RequestException:
         _check_failed(bot)
     else:
         success = True
 
     try:
-        if success:
+        if r is not None:
             info = r.json()
-    except ValueError:
-        # TODO: use JSONDecodeError when dropping Pythons < 3.5
+    except json.JSONDecodeError:
         _check_failed(bot)
         success = False
 
     if not success:
         if bot.memory.get('update_failures', 0) <= max_failures:
             # not enough failures to worry; silently ignore this one
             return
```

### Comparing `sopel-7.1.9/sopel/modules/invite.py` & `sopel-8.0.0/sopel/builtins/invite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# coding=utf-8
 """
 invite.py - Sopel Invite Plugin
 Copyright © 2016, João Vanzuita, https://github.com/converge
 Copyright © 2019, dgw, https://github.com/dgw
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-from sopel import plugin, tools
+from sopel import plugin
 
 
 MIN_PRIV = plugin.HALFOP
 
 
 def invite_handler(bot, sender, user, channel):
     """Common control logic for invite commands received from anywhere."""
-    sender = tools.Identifier(sender)
-    user = tools.Identifier(user)
-    channel = tools.Identifier(channel)
+    sender = bot.make_identifier(sender)
+    user = bot.make_identifier(user)
+    channel = bot.make_identifier(channel)
 
     # Sanity checks, in case someone reuses this function from outside the plugin
     if not sender.is_nick():
         raise ValueError("Invite sender must be a nick, not a channel.")
     if not user.is_nick():
         raise ValueError("User to invite must be a nick, not a channel.")
     if channel.is_nick():
```

### Comparing `sopel-7.1.9/sopel/modules/isup.py` & `sopel-8.0.0/sopel/builtins/isup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding=utf-8
 """
 isup.py - Sopel Website Status Check Plugin
 Copyright 2011, Elsie Powell http://embolalia.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import requests
 
 from sopel import plugin
 
 
 PLUGIN_OUTPUT_PREFIX = '[isup] '
```

### Comparing `sopel-7.1.9/sopel/modules/ping.py` & `sopel-8.0.0/sopel/builtins/ping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# coding=utf-8
 """
 ping.py - Sopel Ping Plugin
 Copyright 2008 (?), Sean B. Palmer, inamidst.com
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import random
 
 from sopel import plugin
 
 
 @plugin.rule(r'(?i)(hi|hello|hey),? $nickname[ \t]*$')
```

### Comparing `sopel-7.1.9/sopel/modules/rand.py` & `sopel-8.0.0/sopel/builtins/rand.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding=utf-8
 """
 rand.py - Rand Plugin
 Copyright 2013, Ari Koivula, <ari@koivu.la>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import random
 import sys
 
 from sopel import plugin
```

### Comparing `sopel-7.1.9/sopel/modules/reload.py` & `sopel-8.0.0/sopel/builtins/reload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# coding=utf-8
 """
 reload.py - Sopel Plugin Reloader Plugin
 Copyright 2008, Sean B. Palmer, inamidst.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import logging
-import subprocess
 
 from sopel import plugin, plugins
 
 
 LOGGER = logging.getLogger(__name__)
 PLUGIN_OUTPUT_PREFIX = '[reload] '
 
@@ -32,15 +30,19 @@
 
 @plugin.nickname_command("reload")
 @plugin.priority("low")
 @plugin.thread(False)
 @plugin.require_admin
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def f_reload(bot, trigger):
-    """Reloads a plugin (for use by admins only)."""
+    """Reload a plugin (for use by admins only)
+
+    NOTE: Designed to work with single-file plugins only, during development.
+    Restart the bot instead when making significant changes.
+    """
     name = trigger.group(2)
 
     if not name or name == '*' or name.upper() == 'ALL THE THINGS':
         bot.reload_plugins()
         bot.say('done')
         return
 
@@ -53,34 +55,21 @@
     bot.say('done: %s reloaded (%s from %s)' % (
         name,
         plugin_meta['type'],
         plugin_meta['source'],
     ))
 
 
-@plugin.nickname_command('update')
-@plugin.require_admin
-@plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
-def f_update(bot, trigger):
-    """Pulls the latest versions of all plugins from Git (for use by admins only)."""
-    proc = subprocess.Popen('/usr/bin/git pull',
-                            stdout=subprocess.PIPE,
-                            stderr=subprocess.PIPE, shell=True)
-    bot.reply(proc.communicate()[0])
-
-    f_reload(bot, trigger)
-
-
 @plugin.nickname_command("load")
 @plugin.priority("low")
 @plugin.thread(False)
 @plugin.require_admin
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def f_load(bot, trigger):
-    """Loads a plugin (for use by admins only)."""
+    """Load a plugin (for use by admins only)"""
     name = trigger.group(2)
     if not name:
         bot.reply('Load what?')
         return
 
     if bot.has_plugin(name):
         bot.reply('Plugin already loaded; use the `reload` command.')
@@ -116,22 +105,14 @@
 @plugin.require_privmsg
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def pm_f_reload(bot, trigger):
     """Wrapper for allowing delivery of .reload command via PM"""
     f_reload(bot, trigger)
 
 
-@plugin.command('update')
-@plugin.require_privmsg
-@plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
-def pm_f_update(bot, trigger):
-    """Wrapper for allowing delivery of .update command via PM"""
-    f_update(bot, trigger)
-
-
 @plugin.command("load")
 @plugin.priority("low")
 @plugin.thread(False)
 @plugin.require_privmsg
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def pm_f_load(bot, trigger):
     """Wrapper for allowing delivery of .load command via PM"""
```

### Comparing `sopel-7.1.9/sopel/modules/search.py` & `sopel-8.0.0/sopel/builtins/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-# coding=utf-8
 """
 search.py - Sopel Search Engine Plugin
 Copyright 2008-9, Sean B. Palmer, inamidst.com
 Copyright 2012, Elsie Powell, embolalia.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import re
 
 import requests
-import xmltodict
+import xmltodict  # type: ignore[import]
 
 from sopel import plugin
 from sopel.tools import web
 
 PLUGIN_OUTPUT_PREFIX = '[search] '
 
 header_spoof = {
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36'
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36',
 }
 r_bing = re.compile(r'<li(?: class="b_algo")?><h2><a href="([^"]+)"')
 r_duck = re.compile(r'nofollow" class="[^"]+" href="(?!(?:https?:\/\/r\.search\.yahoo)|(?:https?:\/\/duckduckgo\.com\/y\.js)(?:\/l\/\?kh=-1&amp;uddg=))(.*?)">')
 
 
 def bing_search(query, lang='en-US'):
     base = 'https://www.bing.com/search'
     parameters = {
         'mkt': lang,
         'q': query,
     }
     response = requests.get(base, parameters, headers=header_spoof)
-    m = r_bing.search(response.text)
-    if m:
-        return m.group(1)
+
+    match = r_bing.search(response.text)
+
+    if match:
+        return web.decode(match.group(1))
 
 
 def duck_search(query):
     query = query.replace('!', '')
     base = 'https://duckduckgo.com/html/'
     parameters = {
         'kl': 'us-en',
         'q': query,
     }
-    bytes = requests.get(base, parameters, headers=header_spoof).text
-    if 'web-result' in bytes:  # filter out the adds on top of the page
-        bytes = bytes.split('web-result')[1]
-    m = r_duck.search(bytes)
-    if m:
-        return web.decode(m.group(1))
+    content = requests.get(base, parameters, headers=header_spoof).text
+
+    if 'web-result' in content:  # filter out the ads on top of the page
+        content = content.split('web-result')[1]
+
+    match = r_duck.search(content)
+
+    if match:
+        return web.decode(match.group(1))
 
 
 def duck_api(query):
     if '!bang' in query.lower():
         return 'https://duckduckgo.com/bang.html'
 
     base = 'https://api.duckduckgo.com/'
@@ -127,16 +131,18 @@
 @plugin.example('.bing sopel.chat irc bot')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def bing(bot, trigger):
     """Queries Bing for the specified input."""
     if not trigger.group(2):
         bot.reply('{}bing what?'.format(bot.settings.core.help_prefix))
         return
+
     query = trigger.group(2)
     result = bing_search(query)
+
     if result:
         bot.say(result)
     else:
         msg = "No results found for '%s'." % query
         if query.count('site:') >= 2:
             # This check exists because of issue #1415.
             # The shortcut link will take the user there.
@@ -149,14 +155,15 @@
 @plugin.example('.search sopel irc bot')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def search(bot, trigger):
     """Searches both Bing and DuckDuckGo."""
     if not trigger.group(2):
         bot.reply('{}search for what?'.format(bot.settings.core.help_prefix))
         return
+
     query = trigger.group(2)
     bu = bing_search(query) or '-'
     du = duck_search(query) or '-'
 
     if bu == '-' and du == '-':
         msg = "No results found for '%s'." % query
         if query.count('site:') >= 2:
@@ -175,37 +182,51 @@
             du = '(extremely long link)'
         result = '%s (b), %s (d)' % (bu, du)
 
     bot.say(result)
 
 
 @plugin.command('suggest')
-@plugin.example('.suggest wikip', 'wikipedia', online=True, vcr=True)
 @plugin.example('.suggest', '.suggest what?')
+@plugin.example('.suggest sopel irc', 'sopel irc', online=True, vcr=True)
+@plugin.example('.suggest wikip', 'wikipedia', online=True, vcr=True, user_help=True)
 @plugin.example('.suggest lkashdfiauwgaef', 'Sorry, no result.', online=True, vcr=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def suggest(bot, trigger):
     """Suggests terms starting with given input"""
     if not trigger.group(2):
         bot.reply('{}suggest what?'.format(bot.settings.core.help_prefix))
         return
+
     query = trigger.group(2)
+
     # Using Google isn't necessarily ideal, but at most they'll be able to build
     # a composite profile of all users on a given instance, not a profile of any
     # single user. This can be switched out as soon as someone finds (or builds)
     # an alternative suggestion API.
     base = 'https://suggestqueries.google.com/complete/search'
     parameters = {
         'output': 'toolbar',
         'hl': 'en',
         'q': query,
     }
+
     response = requests.get(base, parameters)
     answer = xmltodict.parse(response.text)['toplevel']
+
     try:
-        answer = answer['CompleteSuggestion'][0]['suggestion']['@data']
+        answer = answer['CompleteSuggestion']
+
+        try:
+            answer = answer[0]
+        except KeyError:
+            # only one suggestion; don't need to extract first item
+            pass
+
+        answer = answer['suggestion']['@data']
     except TypeError:
         answer = None
+
     if answer:
         bot.say(answer)
     else:
         bot.reply('Sorry, no result.')
```

### Comparing `sopel-7.1.9/sopel/modules/seen.py` & `sopel-8.0.0/sopel/builtins/seen.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-# coding=utf-8
 """
 seen.py - Sopel Seen Plugin
 Copyright 2008, Sean B. Palmer, inamidst.com
 Copyright © 2012, Elad Alfassa <elad@fedoraproject.org>
 Copyright 2019, Sopel contributors
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-import datetime
-import time
+import logging
 
-from sopel import plugin, tools
+from sqlalchemy.exc import SQLAlchemyError
+
+from sopel import plugin
 from sopel.tools.time import seconds_to_human
 
 
+logger = logging.getLogger(__name__)
+
+
 @plugin.command('seen')
 @plugin.output_prefix('[seen] ')
 def seen(bot, trigger):
     """Reports when and where the user was last seen."""
     if not trigger.group(2):
         bot.reply(
             "Use `%sseen <nick>` to know when <nick> was last seen."
@@ -28,28 +31,28 @@
         return
 
     nick = trigger.group(2).strip()
     if nick == bot.nick:
         bot.reply("I'm right here!")
         return
 
-    timestamp = bot.db.get_nick_value(nick, 'seen_timestamp')
-    if not timestamp:
+    saw = bot.db.get_nick_value(nick, 'seen_timestamp')
+    if not saw:
         bot.reply("Sorry, I haven't seen {nick} around.".format(nick=nick))
         return
 
     channel = bot.db.get_nick_value(nick, 'seen_channel')
     message = bot.db.get_nick_value(nick, 'seen_message')
     action = bot.db.get_nick_value(nick, 'seen_action')
 
-    saw = datetime.datetime.utcfromtimestamp(timestamp)
-    delta = seconds_to_human((trigger.time - saw).total_seconds())
+    # as of Sopel 8, trigger.time is an aware datetime
+    delta = seconds_to_human(trigger.time.timestamp() - saw)
 
     msg = "I last saw " + nick
-    if tools.Identifier(channel) == trigger.sender:
+    if bot.make_identifier(channel) == trigger.sender:
         if action:
             msg += " in here {since}, doing: {nick} {action}".format(
                 since=delta,
                 nick=nick,
                 action=message)
         else:
             msg += " in here {since}, saying: {message}".format(
@@ -63,11 +66,16 @@
 @plugin.thread(False)
 @plugin.rule('(.*)')
 @plugin.priority('low')
 @plugin.unblockable
 @plugin.require_chanmsg
 def note(bot, trigger):
     nick = trigger.nick
-    bot.db.set_nick_value(nick, 'seen_timestamp', time.time())
-    bot.db.set_nick_value(nick, 'seen_channel', trigger.sender)
-    bot.db.set_nick_value(nick, 'seen_message', trigger)
-    bot.db.set_nick_value(nick, 'seen_action', trigger.ctcp is not None)
+    try:
+        # as of Sopel 8, `trigger.time` is Aware, meaning we should store its value
+        # for timezone safety when comparing it later
+        bot.db.set_nick_value(nick, 'seen_timestamp', trigger.time.timestamp())
+        bot.db.set_nick_value(nick, 'seen_channel', trigger.sender)
+        bot.db.set_nick_value(nick, 'seen_message', trigger)
+        bot.db.set_nick_value(nick, 'seen_action', trigger.ctcp is not None)
+    except SQLAlchemyError as error:
+        logger.error("Unable to save seen, database error: %s" % error)
```

### Comparing `sopel-7.1.9/sopel/modules/tell.py` & `sopel-8.0.0/sopel/builtins/tell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-# coding=utf-8
 """
 tell.py - Sopel Tell and Ask Plugin
 Copyright 2008, Sean B. Palmer, inamidst.com
 Copyright 2019, dgw, technobabbl.es
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 from collections import defaultdict
 import io  # don't use `codecs` for loading the DB; it will split lines on some IRC formatting
 import logging
 import os
-import sys
 import threading
 import time
 import unicodedata
 
-from sopel import formatting, plugin, tools
+from sopel import formatting, plugin
 from sopel.config import types
 from sopel.tools.time import format_time, get_timezone
 
 
-if sys.version_info.major >= 3:
-    unicode = str
-
-
 LOGGER = logging.getLogger(__name__)
 
 
 class TellSection(types.StaticSection):
     use_private_reminder = types.BooleanAttribute(
         'use_private_reminder', default=False)
     """When set to ``true``, Sopel will send reminder as private message."""
@@ -142,15 +136,15 @@
     :param str text: text to clean
     :rtype: str
     :raises TypeError: if the passed ``text`` is not a string
 
     Stolen and tweaked from the ``choose`` plugin's ``_format_safe()``
     function by the person who wrote it.
     """
-    if not isinstance(text, unicode):
+    if not isinstance(text, str):
         raise TypeError("A string is required.")
     elif not text:
         # unnecessary optimization
         return ''
 
     start = 0
 
@@ -172,69 +166,75 @@
 
     return text[start:]
 
 
 @plugin.command('tell', 'ask')
 @plugin.nickname_command('tell', 'ask')
 @plugin.example('$nickname, tell dgw he broke it again.', user_help=True)
+@plugin.example('.ask ', 'ask whom?')
 @plugin.example('.tell ', 'tell whom?')
+@plugin.example('.ask @', 'ask whom?')
+@plugin.example('.tell @', 'tell whom?')
 @plugin.example('.ask Exirel ', 'ask Exirel what?')
+@plugin.example('.tell Exirel ', 'tell Exirel what?')
+@plugin.example('.ask @Exirel ', 'ask Exirel what?')
+@plugin.example('.tell @Exirel ', 'tell Exirel what?')
 def f_remind(bot, trigger):
     """Give someone a message the next time they're seen"""
     teller = trigger.nick
     verb = trigger.group(1)
 
     if not trigger.group(3):
+        tellee = ""
+    else:
+        tellee = trigger.group(3).rstrip('.,:;').lstrip('@')
+
+    if not tellee:
         bot.reply("%s whom?" % verb)
         return
 
-    tellee = trigger.group(3).rstrip('.,:;')
-
     # all we care about is having at least one non-whitespace
     # character after the name
     if not trigger.group(4):
         bot.reply("%s %s what?" % (verb, tellee))
         return
 
     msg = _format_safe_lstrip(trigger.group(2).split(' ', 1)[1])
 
     if not msg:
         bot.reply("%s %s what?" % (verb, tellee))
         return
 
-    tellee = tools.Identifier(tellee)
+    tellee = bot.make_identifier(tellee)
 
     if not os.path.exists(bot.tell_filename):
         return
 
     if len(tellee) > bot.isupport.get('NICKLEN', 30):
         bot.reply('That nickname is too long.')
         return
 
-    if tellee[0] == '@':
-        tellee = tellee[1:]
-
     if tellee == bot.nick:
         bot.reply("I'm here now; you can %s me whatever you want!" % verb)
         return
 
-    if tellee not in (tools.Identifier(teller), bot.nick, 'me'):
+    if tellee not in (bot.make_identifier(teller), bot.nick, 'me'):
         tz = get_timezone(bot.db, bot.config, None, tellee)
         timenow = format_time(bot.db, bot.config, tz, tellee)
         with bot.memory['tell_lock']:
             if tellee not in bot.memory['reminders']:
                 bot.memory['reminders'][tellee] = [(teller, verb, timenow, msg)]
             else:
                 bot.memory['reminders'][tellee].append((teller, verb, timenow, msg))
             # save the reminders
             dump_reminders(bot.tell_filename, bot.memory['reminders'])
 
         response = "I'll pass that on when %s is around." % tellee
         bot.reply(response)
-    elif tools.Identifier(teller) == tellee:
+    elif bot.make_identifier(teller) == tellee:
         bot.reply('You can %s yourself that.' % verb)
     else:
         bot.reply("Hey, I'm not as stupid as Monty you know!")
 
 
 def get_nick_reminders(reminders, nick):
     lines = []
```

### Comparing `sopel-7.1.9/sopel/modules/tld.py` & `sopel-8.0.0/sopel/builtins/tld.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-# coding=utf-8
 """
 tld.py - Sopel TLD Plugin
 Copyright 2009-10, Michael Yanovich, yanovich.net
 Copyright 2020, dgw, technobabbl.es
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 from datetime import datetime
 from encodings import idna
+from html.parser import HTMLParser
+from json import JSONDecodeError
 import logging
 import re
-import sys
+from typing import Union
 
 import pytz
 import requests
 
 from sopel import formatting, plugin, tools
 
-if sys.version_info.major >= 3:
-    unicode = str
-    from html.parser import HTMLParser
-else:
-    from HTMLParser import HTMLParser
-
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _strptime_as_utc(time_string):
     return datetime.strptime(
         time_string, DATE_FORMAT).replace(tzinfo=pytz.utc)
@@ -40,14 +35,21 @@
 DEFAULT_CACHE_DATETIME = _strptime_as_utc(DEFAULT_CACHE_TIME)
 
 IANA_LIST_URI = 'https://data.iana.org/TLD/tlds-alpha-by-domain.txt'
 WIKI_PAGE_NAMES = [
     'List_of_Internet_top-level_domains',
     'Country_code_top-level_domain',
 ]
+WIKI_API_PARAMS: dict[str, Union[str, int]] = {
+    "action": "parse",
+    "format": "json",
+    "prop": "text",
+    "utf8": 1,
+    "formatversion": 2,
+}
 r_tld = re.compile(r'^\.(\S+)')
 r_idn = re.compile(r'^(xn--[A-Za-z0-9]+)')
 
 
 def setup(bot):
     bot.memory['tld_list_cache'] = bot.db.get_plugin_value(
         'tld', 'tld_list_cache', [])
@@ -103,14 +105,15 @@
         HTMLParser.__init__(self)
         self.in_cell = False
         self.skipping = True
         self.current_row = []
         self.current_cell = ''
         self.rows = []
         self.tables = []
+        self.parsed: dict[str, dict[str, str]] = {}
         self.finished = False
 
     def handle_starttag(self, tag, attrs):
         if tag == 'td' or tag == 'th':
             self.in_cell = True
         elif tag == 'sup' and self.in_cell:
             # ignore superscripts; they're almost exclusively footnotes
@@ -161,15 +164,15 @@
         if self.in_cell and not self.skipping:
             self.current_cell += data
 
     def get_processed_data(self):
         LOGGER.debug("Processed TLD data requested.")
         if self.finished:
             LOGGER.debug("Returning stored previously-processed data.")
-            return self.tables
+            return self.parsed
 
         LOGGER.debug("Ensuring all buffered data has been parsed.")
         self.close()
 
         LOGGER.debug("Processing tables.")
         tld_list = {}
         for table in self.tables:
@@ -205,17 +208,21 @@
                 }
                 if key:
                     tld_list[key] = zipped
                 if idn_key:
                     tld_list[idn_key] = zipped
 
         LOGGER.debug("Finished processing TLD data; returning it.")
-        self.tables = tld_list
         self.finished = True
-        return self.tables
+        # clear working data
+        del self.tables
+        # cache parsed data for future requests to this parser
+        self.parsed = tld_list
+
+        return self.parsed
 
 
 def _update_tld_data(bot, which, force=False):
     if which == 'list':
         then = bot.memory['tld_list_cache_updated']
     elif which == 'data':
         then = bot.memory['tld_data_cache_updated']
@@ -231,49 +238,45 @@
             which,
             '1 day' if since.days == 1 else ('%d days' % since.days),
         )
         return
 
     if which == 'list':
         try:
-            tld_list = requests.get(IANA_LIST_URI).text
+            tld_raw = requests.get(IANA_LIST_URI).text
         except requests.exceptions.RequestException:
             # Probably a transient error; log it and continue life
             LOGGER.warning(
                 "Error fetching IANA TLD list; will try again later.",
                 exc_info=True)
             return
 
         tld_list = [
             line.lower()
-            for line in tld_list.splitlines()
+            for line in tld_raw.splitlines()
             if not line.startswith('#')
         ]
 
         bot.memory['tld_list_cache'] = tld_list
         bot.memory['tld_list_cache_updated'] = now
     elif which == 'data':
         data_pages = []
         for title in WIKI_PAGE_NAMES:
+            # don't one-liner this; dict.update() returns None, not the updated dict
+            parameters = WIKI_API_PARAMS.copy()
+            parameters.update({"page": title})
+
             try:
                 # https://www.mediawiki.org/wiki/Special:MyLanguage/API:Get_the_contents_of_a_page
                 tld_response = requests.get(
                     "https://en.wikipedia.org/w/api.php",
-                    params={
-                        "action": "parse",
-                        "format": "json",
-                        "prop": "text",
-                        "utf8": 1,
-                        "formatversion": 2,
-                        "page": title,
-                    },
+                    params=parameters,
                 ).json()
                 data_pages.append(tld_response["parse"]["text"])
-            # py <3.5 needs ValueError instead of more specific json.decoder.JSONDecodeError
-            except (requests.exceptions.RequestException, ValueError, KeyError):
+            except (requests.exceptions.RequestException, JSONDecodeError, KeyError):
                 # Log error and continue life; it'll be fine
                 LOGGER.warning(
                     'Error fetching TLD data from "%s" on Wikipedia; will try again later.',
                     title, exc_info=True)
                 return
 
         parser = WikipediaTLDListParser()
```

### Comparing `sopel-7.1.9/sopel/modules/translate.py` & `sopel-8.0.0/sopel/builtins/translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-# coding=utf-8
 """
 translate.py - Sopel Translation Plugin
 Copyright 2008, Sean B. Palmer, inamidst.com
 Copyright 2013-2014, Elad Alfassa <elad@fedoraproject.org>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import json
 import logging
 import random
 import re
-import sys
 
 import requests
 
-from sopel import plugin, tools
+from sopel import plugin
 from sopel.tools import web
 
-if sys.version_info.major >= 3:
-    unicode = str
 
 LOGGER = logging.getLogger(__name__)
 PLUGIN_OUTPUT_PREFIX = '[translate] '
 
 
 def setup(bot):
     if 'mangle_lines' not in bot.memory:
-        bot.memory['mangle_lines'] = tools.SopelIdentifierMemory()
+        bot.memory['mangle_lines'] = bot.make_identifier_memory()
 
 
 def shutdown(bot):
     try:
         del bot.memory['mangle_lines']
     except KeyError:
         pass
 
 
 def translate(text, in_lang='auto', out_lang='en'):
     raw = False
-    if unicode(out_lang).endswith('-raw'):
+    if str(out_lang).endswith('-raw'):
         out_lang = out_lang[:-4]
         raw = True
 
     headers = {
         'User-Agent': 'Mozilla/5.0' +
         '(X11; U; Linux i686)' +
         'Gecko/20071127 Firefox/2.0.0.11'
@@ -132,35 +128,32 @@
     if not msg:
         bot.reply(
             'The %s to %s translation failed; are you sure you specified '
             'valid language abbreviations?' % (in_lang, out_lang)
         )
         return
 
-    if sys.version_info.major < 3 and isinstance(msg, str):
-        msg = msg.decode('utf-8')
-
     msg = web.decode(msg)
     msg = '"%s" (%s to %s, translate.google.com)' % (msg, in_lang, out_lang)
     bot.say(msg)
 
 
 @plugin.command('translate', 'tr')
 @plugin.example('.tr :en :fr my dog',
                 '"mon chien" (en to fr, translate.google.com)',
-                online=True, vcr=True)
+                online=True, vcr=True, user_help=True)
 @plugin.example('.tr מחשב',
                 '"computer" (iw to en, translate.google.com)',
                 online=True, vcr=True)
 @plugin.example('.tr mon chien',
                 '"my dog" (fr to en, translate.google.com)',
-                online=True, vcr=True)
+                online=True, vcr=True, user_help=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def tr2(bot, trigger):
-    """Translates a phrase, with an optional language hint."""
+    """Translates a phrase, with an optional language :hint."""
     command = trigger.group(2)
 
     if not command:
         bot.reply('You did not give me anything to translate.')
         return
 
     def langcode(p):
@@ -221,17 +214,14 @@
     if not msg:
         bot.reply(
             'The %s to %s translation failed; '
             'are you sure you specified valid language abbreviations?'
             % (src, dest))
         return
 
-    if sys.version_info.major < 3 and isinstance(msg, str):
-        msg = msg.decode('utf-8')
-
     msg = web.decode(msg)  # msg.replace('&#39;', "'")
     msg = '"%s" (%s to %s, translate.google.com)' % (msg, src, dest)
 
     bot.say(msg)
 
 
 def get_random_lang(long_list, short_list):
@@ -245,20 +235,21 @@
 
 
 @plugin.command('mangle', 'mangle2')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def mangle(bot, trigger):
     """Repeatedly translate the input until it makes absolutely no sense."""
     long_lang_list = ['fr', 'de', 'es', 'it', 'no', 'he', 'la', 'ja', 'cy', 'ar', 'yi', 'zh', 'nl', 'ru', 'fi', 'hi', 'af', 'jw', 'mr', 'ceb', 'cs', 'ga', 'sv', 'eo', 'el', 'ms', 'lv']
-    lang_list = []
+    lang_list: list[str] = []
 
     for __ in range(0, 8):
         lang_list = get_random_lang(long_lang_list, lang_list)
     random.shuffle(lang_list)
 
+    phrase: tuple[str, ...] = ()
     if trigger.group(2) is None:
         try:
             phrase = (bot.memory['mangle_lines'][trigger.sender], '')
         except KeyError:
             bot.reply("What do you want me to mangle?")
             return
     else:
@@ -269,15 +260,15 @@
         return
 
     for lang in lang_list:
         backup = phrase
         try:
             phrase = translate(phrase[0], 'en', lang)
         except Exception:  # TODO: Be specific
-            phrase = False
+            phrase = ()
         if not phrase:
             phrase = backup
             break
 
         try:
             phrase = translate(phrase[0], lang, 'en')
         except Exception:  # TODO: Be specific
```

### Comparing `sopel-7.1.9/sopel/modules/unicode_info.py` & `sopel-8.0.0/sopel/builtins/unicode_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-# coding=utf-8
 """
 unicode_info.py - Sopel Codepoints Plugin
 Copyright 2013, Elsie Powell, embolalia.com
 Copyright 2008, Sean B. Palmer, inamidst.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
-
-import sys
-import unicodedata
+from __future__ import annotations
 
 from sopel import plugin
 
-if sys.version_info.major >= 3:
-    # Note on unicode and str (required for py2 compatibility)
-    # the `hex` function returns a `str`, both in py2 and py3
-    # however, a `str` is a unicode string in py3, but a bytestring in py2
-    # in order to prevent that, we encode the return from `hex` as `unicode`
-    # and since this class does not exist anymore on py3, we create an alias
-    # for `str` in py3
-    unichr = chr
-    unicode = str
+# Python built-in unicodedata uses UCD version 13 (as of Python 3.10)
+# unicodedata2 can provide a more recent version, so we use that if present
+# See also: https://docs.python.org/3/library/unicodedata.html
+try:
+    # ignore type check for these imports (no stubs for unicodedata2)
+    import unicodedata2 as unicodedata  # type: ignore[import]
+except ImportError:
+    import unicodedata  # type: ignore[no-redef]
 
 
 def get_codepoint_name(char):
     """Retrieve the code point (and name, if possible) for a given character"""
     # Get the hex value for the code point, and drop the 0x from the front
-    point = unicode(hex(ord(char)))[2:]
+    point = hex(ord(char))[2:]
 
     # Make the hex 4 characters long with preceding 0s, and all upper case
     point = point.rjust(4, '0').upper()
 
     # get codepoint's name
     name = None
     try:
@@ -56,15 +51,15 @@
     stripped = arg.strip()
     if len(stripped) > 0:
         arg = stripped
     if len(arg) > 1:
         if arg.startswith('U+'):
             arg = arg[2:]
         try:
-            arg = unichr(int(arg, 16))
+            arg = chr(int(arg, 16))
         except (ValueError, TypeError):
             bot.reply("That's not a valid code point.")
             return plugin.NOLIMIT
 
     point, name = get_codepoint_name(arg)
     if name is None:
         name = '(No name found)'
```

### Comparing `sopel-7.1.9/sopel/modules/units.py` & `sopel-8.0.0/sopel/builtins/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# coding=utf-8
 """
 units.py - Sopel Unit Conversion Plugin
 Copyright © 2013, Elad Alfassa, <elad@fedoraproject.org>
 Copyright © 2013, Dimitri Molenaars, <tyrope@tyrope.nl>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import re
 
 from sopel import plugin
 
 
 PLUGIN_OUTPUT_PREFIX = '[units] '
@@ -33,29 +32,37 @@
     return (9.0 / 5.0 * temp + 32)
 
 
 def k_to_c(temp):
     return temp - 273.15
 
 
+def _extract_source(pattern, trigger) -> tuple[str, ...]:
+    match = pattern.match(trigger.group(2))
+    if match:
+        return match.groups()
+    else:
+        raise ValueError("Pattern does not match")
+
+
 @plugin.command('temp')
 @plugin.example('.temp 100F', '37.78°C = 100.00°F = 310.93K')
 @plugin.example('.temp 100C', '100.00°C = 212.00°F = 373.15K')
 @plugin.example('.temp 100K', '-173.15°C = -279.67°F = 100.00K')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def temperature(bot, trigger):
     """Convert temperatures"""
     try:
-        source = find_temp.match(trigger.group(2)).groups()
-    except (AttributeError, TypeError):
+        source = _extract_source(find_temp, trigger)
+    except (ValueError, TypeError):
         bot.reply("That's not a valid temperature.")
         return plugin.NOLIMIT
     unit = source[1].upper()
     numeric = float(source[0])
-    celsius = 0
+    celsius = 0.0
     if unit == 'C':
         celsius = numeric
     elif unit == 'F':
         celsius = f_to_c(numeric)
     elif unit == 'K':
         celsius = k_to_c(numeric)
 
@@ -84,21 +91,21 @@
 @plugin.example('.length 3 ly', '28382191417742.40km = 17635876112814.77 miles')
 @plugin.example('.length 3 au', '448793612.10km = 278867421.71 miles')
 @plugin.example('.length 3 parsec', '92570329129020.20km = 57520535754731.61 miles')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def distance(bot, trigger):
     """Convert distances"""
     try:
-        source = find_length.match(trigger.group(2)).groups()
-    except (AttributeError, TypeError):
+        source = _extract_source(find_length, trigger)
+    except (ValueError, TypeError):
         bot.reply("That's not a valid length unit.")
         return plugin.NOLIMIT
     unit = source[1].lower()
     numeric = float(source[0])
-    meter = 0
+    meter = 0.0
     if unit in ("meters", "meter", "m"):
         meter = numeric
     elif unit in ("millimeters", "millimeter", "mm"):
         meter = numeric / 1000
     elif unit in ("kilometers", "kilometer", "km"):
         meter = numeric * 1000
     elif unit in ("miles", "mile", "mi"):
@@ -155,21 +162,21 @@
 
 
 @plugin.command('weight', 'mass')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def mass(bot, trigger):
     """Convert mass"""
     try:
-        source = find_mass.match(trigger.group(2)).groups()
-    except (AttributeError, TypeError):
+        source = _extract_source(find_mass, trigger)
+    except (ValueError, TypeError):
         bot.reply("That's not a valid mass unit.")
         return plugin.NOLIMIT
     unit = source[1].lower()
     numeric = float(source[0])
-    metric = 0
+    metric = 0.0
     if unit in ("gram", "grams", "gramme", "grammes", "g"):
         metric = numeric
     elif unit in ("kilogram", "kilograms", "kilogramme", "kilogrammes", "kg"):
         metric = numeric * 1000
     elif unit in ("lb", "lbm", "pound", "pounds"):
         metric = numeric * 453.59237
     elif unit in ("oz", "ounce"):
```

### Comparing `sopel-7.1.9/sopel/modules/uptime.py` & `sopel-8.0.0/sopel/builtins/uptime.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# coding=utf-8
 """
 uptime.py - Sopel Uptime Plugin
 Copyright 2014, Fabian Neundorf
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-import datetime
+from datetime import datetime, timedelta, timezone
 
 from sopel import plugin
 
 
 def setup(bot):
     if "start_time" not in bot.memory:
-        bot.memory["start_time"] = datetime.datetime.utcnow()
+        bot.memory["start_time"] = datetime.now(timezone.utc)
 
 
 @plugin.command('uptime')
 @plugin.example('.uptime', user_help=True)
 @plugin.output_prefix('[uptime] ')
 def uptime(bot, trigger):
     """Return the uptime of Sopel."""
-    delta = datetime.timedelta(seconds=round((datetime.datetime.utcnow() -
-                                              bot.memory["start_time"])
-                                             .total_seconds()))
+    delta = timedelta(seconds=round((datetime.now(timezone.utc) -
+                                    bot.memory["start_time"])
+                                    .total_seconds()))
     bot.say("I've been sitting here for {} and I keep going!".format(delta))
```

### Comparing `sopel-7.1.9/sopel/modules/url.py` & `sopel-8.0.0/sopel/builtins/url.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-# coding=utf-8
 """
 url.py - Sopel URL Title Plugin
 Copyright 2010-2011, Michael Yanovich (yanovich.net) & Kenneth Sham
 Copyright 2012-2013, Elsie Powell
 Copyright 2013, Lior Ramati <firerogue517@gmail.com>
 Copyright 2014, Elad Alfassa <elad@fedoraproject.org>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-import ipaddress
+from ipaddress import ip_address
 import logging
 import re
+from typing import NamedTuple, Optional, TYPE_CHECKING
+from urllib.parse import urlparse
 
 import dns.resolver
 import requests
-from urllib3.exceptions import LocationValueError
+from urllib3.exceptions import LocationValueError  # type: ignore[import]
 
-from sopel import plugin, tools
+from sopel import plugin, privileges, tools
 from sopel.config import types
 from sopel.tools import web
 
-# Python3 vs Python2
-try:
-    from urllib.parse import urlparse
-except ImportError:
-    from urlparse import urlparse
+if TYPE_CHECKING:
+    from collections.abc import Generator
+    from sopel.bot import Sopel, SopelWrapper
+    from sopel.config import Config
+    from sopel.trigger import Trigger
+
 
 LOGGER = logging.getLogger(__name__)
 USER_AGENT = (
     'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
     'AppleWebKit/537.36 (KHTML, like Gecko) '
     'Chrome/98.0.4758.102 Safari/537.36'
 )
@@ -40,53 +42,53 @@
     'Accept': 'text/html, application/xhtml+xml, application/xml;q=0.9, */*;q=0.8',
     'Accept-Language': 'en,en-US;q=0,5',
 }
 # These are used to clean up the title tag before actually parsing it. Not the
 # world's best way to do this, but it'll do for now.
 TITLE_TAG_DATA = re.compile('<(/?)title( [^>]+)?>', re.IGNORECASE)
 QUOTED_TITLE = re.compile('[\'"]<title>[\'"]', re.IGNORECASE)
-# This is another regex that presumably does something important.
-RE_DCC = re.compile(r'(?i)dcc\ssend')
 # This sets the maximum number of bytes that should be read in order to find
 # the title. We don't want it too high, or a link to a big file/stream will
 # just keep downloading until there's no more memory. 640k ought to be enough
 # for anybody, but the modern web begs to differ.
 MAX_BYTES = 655360 * 2
 
 
 class UrlSection(types.StaticSection):
     enable_auto_title = types.BooleanAttribute(
         'enable_auto_title', default=True)
     """Enable auto-title (enabled by default)"""
     # TODO some validation rules maybe?
     exclude = types.ListAttribute('exclude')
     """A list of regular expressions to match URLs for which the title should not be shown."""
+    exclude_required_access = types.ChoiceAttribute(
+        'exclude_required_access',
+        choices=privileges.__all__,
+        default='OP',
+    )
+    """Minimum channel access level required to edit ``exclude`` list using chat commands."""
     exclusion_char = types.ValidatedAttribute('exclusion_char', default='!')
     """A character (or string) which, when immediately preceding a URL, will stop that URL's title from being shown."""
     shorten_url_length = types.ValidatedAttribute(
         'shorten_url_length', int, default=0)
     """If greater than 0, the title fetcher will include a TinyURL version of links longer than this many characters."""
     enable_private_resolution = types.BooleanAttribute(
         'enable_private_resolution', default=False)
-    """Enable URL lookups for RFC1918 addresses"""
-    enable_dns_resolution = types.BooleanAttribute(
-        'enable_dns_resolution', default=False)
-    """Enable DNS resolution for all domains to validate if there are RFC1918 resolutions"""
+    """Enable requests to private and local network IP addresses"""
 
 
-def configure(config):
+def configure(config: Config):
     """
     | name | example | purpose |
     | ---- | ------- | ------- |
     | enable_auto_title | yes | Enable auto-title. |
     | exclude | https?://git\\\\.io/.* | A list of regular expressions for URLs for which the title should not be shown. |
     | exclusion\\_char | ! | A character (or string) which, when immediately preceding a URL, will stop the URL's title from being shown. |
     | shorten\\_url\\_length | 72 | If greater than 0, the title fetcher will include a TinyURL version of links longer than this many characters. |
-    | enable\\_private\\_resolution | False | Enable URL lookups for RFC1918 addresses. |
-    | enable\\_dns\\_resolution | False | Enable DNS resolution for all domains to validate if there are RFC1918 resolutions. |
+    | enable\\_private\\_resolution | False | Enable requests to private and local network IP addresses. |
     """
     config.define_section('url', UrlSection)
     config.url.configure_setting(
         'enable_auto_title',
         'Enable auto-title?'
     )
     config.url.configure_setting(
@@ -101,23 +103,19 @@
         'shorten_url_length',
         'Enter how many characters a URL should be before the bot puts a'
         ' shorter version of the URL in the title as a TinyURL link'
         ' (0 to disable)'
     )
     config.url.configure_setting(
         'enable_private_resolution',
-        'Enable URL lookups for RFC1918 addresses?'
-    )
-    config.url.configure_setting(
-        'enable_dns_resolution',
-        'Enable DNS resolution for all domains to validate if there are RFC1918 resolutions?'
+        'Enable requests to private and local network IP addresses?'
     )
 
 
-def setup(bot):
+def setup(bot: Sopel):
     bot.config.define_section('url', UrlSection)
 
     if bot.config.url.exclude:
         regexes = [re.compile(s) for s in bot.config.url.exclude]
     else:
         regexes = []
 
@@ -131,47 +129,67 @@
         exclude = bot.memory['url_exclude']
         if regexes:
             exclude.extend(regexes)
         bot.memory['url_exclude'] = exclude
 
     # Ensure last_seen_url is in memory
     if 'last_seen_url' not in bot.memory:
-        bot.memory['last_seen_url'] = tools.SopelIdentifierMemory()
+        bot.memory['last_seen_url'] = bot.make_identifier_memory()
 
     # Initialize shortened_urls as a dict if it doesn't exist.
     if 'shortened_urls' not in bot.memory:
         bot.memory['shortened_urls'] = tools.SopelMemory()
 
 
-def shutdown(bot):
+def shutdown(bot: Sopel):
     # Unset `url_exclude` and `last_seen_url`, but not `shortened_urls`;
     # clearing `shortened_urls` will increase API calls. Leaving it in memory
     # should not lead to unexpected behavior.
     for key in ['url_exclude', 'last_seen_url']:
         try:
             del bot.memory[key]
         except KeyError:
             pass
 
 
+def _user_can_change_excludes(bot: SopelWrapper, trigger: Trigger):
+    if trigger.admin:
+        return True
+
+    required_access = bot.config.url.exclude_required_access
+    channel = bot.channels[trigger.sender]
+    user_access = channel.privileges[trigger.nick]
+
+    if user_access >= getattr(privileges, required_access):
+        return True
+
+    return False
+
+
 @plugin.command('urlexclude', 'urlpexclude', 'urlban', 'urlpban')
 @plugin.example('.urlpexclude example\\.com/\\w+', user_help=True)
 @plugin.example('.urlexclude example.com/path', user_help=True)
 @plugin.output_prefix('[url] ')
-def url_ban(bot, trigger):
+def url_ban(bot: SopelWrapper, trigger: Trigger):
     """Exclude a URL from auto title.
 
     Use ``urlpexclude`` to exclude a pattern instead of a URL.
     """
     url = trigger.group(2)
 
     if not url:
         bot.reply('This command requires a URL to exclude.')
         return
 
+    if not _user_can_change_excludes(bot, trigger):
+        bot.reply(
+            'Only admins and channel members with %s access or higher may '
+            'modify URL excludes.' % bot.config.url.exclude_required_access)
+        return
+
     if trigger.group(1) in ['urlpexclude', 'urlpban']:
         # validate regex pattern
         try:
             re.compile(url)
         except re.error as err:
             bot.reply('Invalid regex pattern: %s' % err)
             return
@@ -198,25 +216,31 @@
     bot.reply('This URL is now excluded from auto title.')
 
 
 @plugin.command('urlallow', 'urlpallow', 'urlunban', 'urlpunban')
 @plugin.example('.urlpallow example\\.com/\\w+', user_help=True)
 @plugin.example('.urlallow example.com/path', user_help=True)
 @plugin.output_prefix('[url] ')
-def url_unban(bot, trigger):
+def url_unban(bot: SopelWrapper, trigger: Trigger):
     """Allow a URL for auto title.
 
     Use ``urlpallow`` to allow a pattern instead of a URL.
     """
     url = trigger.group(2)
 
     if not url:
         bot.reply('This command requires a URL to allow.')
         return
 
+    if not _user_can_change_excludes(bot, trigger):
+        bot.reply(
+            'Only admins and channel members with %s access or higher may '
+            'modify URL excludes.' % bot.config.url.exclude_required_access)
+        return
+
     if trigger.group(1) in ['urlpallow', 'urlpunban']:
         # validate regex pattern
         try:
             re.compile(url)
         except re.error as err:
             bot.reply('Invalid regex pattern: %s' % err)
             return
@@ -245,39 +269,36 @@
 
 @plugin.command('title')
 @plugin.example(
     '.title https://www.google.com',
     'Google | www.google.com',
     online=True, vcr=True)
 @plugin.output_prefix('[url] ')
-def title_command(bot, trigger):
+def title_command(bot: SopelWrapper, trigger: Trigger):
     """
     Show the title or URL information for the given URL, or the last URL seen
     in this channel.
     """
+    result_count = 0
+
     if not trigger.group(2):
         if trigger.sender not in bot.memory['last_seen_url']:
             return
-        matched = check_callbacks(
-            bot, bot.memory['last_seen_url'][trigger.sender])
-        if matched:
-            return
-        else:
-            urls = [bot.memory['last_seen_url'][trigger.sender]]
+        urls = [bot.memory["last_seen_url"][trigger.sender]]
     else:
-        urls = list(  # needs to be a list so len() can be checked later
-            web.search_urls(
-                trigger,
-                exclusion_char=bot.config.url.exclusion_char
-            )
-        )
+        # needs to be a list so len() can be checked later
+        urls = list(web.search_urls(trigger))
 
-    result_count = 0
-    for url, title, domain, tinyurl in process_urls(bot, trigger, urls):
-        message = '%s | %s' % (title, domain)
+    for url, title, domain, tinyurl, ignored in process_urls(
+        bot, trigger, urls, requested=True
+    ):
+        if ignored:
+            result_count += 1
+            continue
+        message = "%s | %s" % (title, domain)
         if tinyurl:
             message += ' ( %s )' % tinyurl
         bot.reply(message)
         bot.memory['last_seen_url'][trigger.sender] = url
         result_count += 1
 
     expected_count = len(urls)
@@ -288,149 +309,227 @@
             bot.reply("Sorry, I couldn't fetch titles for any of those.")
         else:
             bot.reply("I couldn't get all of the titles, but I fetched what I could!")
 
 
 @plugin.rule(r'(?u).*(https?://\S+).*')
 @plugin.output_prefix('[url] ')
-def title_auto(bot, trigger):
+def title_auto(bot: SopelWrapper, trigger: Trigger):
     """
     Automatically show titles for URLs. For shortened URLs/redirects, find
-    where the URL redirects to and show the title for that (or call a function
-    from another plugin to give more information).
+    where the URL redirects to and show the title for that.
+
+    .. note::
+
+        URLs that match (before redirection) any other registered callbacks
+        will *not* have their titles shown.
+
     """
     # Enabled or disabled by feature flag
     if not bot.settings.url.enable_auto_title:
         return
 
     # Avoid fetching links from another command
     if re.match(bot.config.core.prefix + r'\S+', trigger):
         return
 
-    # Avoid fetching known malicious links
-    if 'safety_cache' in bot.memory and trigger in bot.memory['safety_cache']:
-        if bot.memory['safety_cache'][trigger]['positives'] > 1:
-            return
-
-    urls = web.search_urls(
+    unchecked_urls = web.search_urls(
         trigger, exclusion_char=bot.config.url.exclusion_char, clean=True)
 
-    for url, title, domain, tinyurl in process_urls(bot, trigger, urls):
-        message = '%s | %s' % (title, domain)
-        if tinyurl:
-            message += ' ( %s )' % tinyurl
-        # Guard against responding to other instances of this bot.
-        if message != trigger:
-            bot.say(message)
-            bot.memory['last_seen_url'][trigger.sender] = url
+    urls = []
+    safety_cache = bot.memory.get("safety_cache", {})
+    safety_cache_local = bot.memory.get("safety_cache_local", {})
+    for url in unchecked_urls:
+        # Avoid fetching known malicious links
+        if url in safety_cache and safety_cache[url]["positives"] > 0:
+            continue
+        parsed = urlparse(url)
+        if not parsed.hostname or parsed.hostname.lower() in safety_cache_local:
+            continue
+        urls.append(url)
+
+    for url, title, domain, tinyurl, ignored in process_urls(bot, trigger, urls):
+        if not ignored:
+            message = '%s | %s' % (title, domain)
+            if tinyurl:
+                message += ' ( %s )' % tinyurl
+            # Guard against responding to other instances of this bot.
+            if message != trigger:
+                bot.say(message)
+        bot.memory["last_seen_url"][trigger.sender] = url
+
+
+class URLInfo(NamedTuple):
+    """Helper class for information about a URL handled by this plugin."""
 
+    url: str
+
+    title: Optional[str]
+    """The title associated with ``url``, if appropriate."""
+
+    hostname: Optional[str]
+    """The hostname associated with ``url``, if appropriate."""
+
+    tinyurl: Optional[str]
+    """A shortened form of ``url``, if appropriate."""
+
+    ignored: bool
+    """Whether or not this URL matches any registered callbacks or is explicitly excluded."""
+
+
+def process_urls(
+    bot: SopelWrapper,
+    trigger: Trigger,
+    urls: list[str],
+    requested: bool = False,
+) -> Generator[URLInfo, None, None]:
+    """
+    For each URL in the list, ensure it should be titled, and do so.
+
+    :param bot: Sopel instance
+    :param trigger: The trigger object for this event
+    :param urls: The URLs detected in the triggering message
+    :param requested: Whether the title was explicitly requested (vs automatic)
+
+    Yields a tuple ``(url, title, hostname, tinyurl, ignored)`` for each URL.
+
+    .. note:
+
+        If a URL in ``urls`` has any registered callbacks, this function will NOT
+        retrieve the title, and considers the URL as dispatched to those callbacks.
+        In this case, only the ``url`` and ``ignored=True`` will be set; all
+        other values will be ``None``.
+
+    .. note:
+
+        For titles explicitly requested by the user, ``exclusion_char`` and
+        exclusions from the ``.urlban``/``.urlpban`` commands are skipped.
+
+    .. versionchanged:: 8.0
+
+        This function **does not** notify callbacks registered for URLs
+        redirected to from URLs passed to this function. See #2432, #2230.
 
-def process_urls(bot, trigger, urls):
-    """
-    For each URL in the list, ensure that it isn't handled by another plugin.
-    If not, find where it redirects to, if anywhere. If that redirected URL
-    should be handled by another plugin, dispatch the callback for it.
-    Return a list of (title, hostname) tuples for each URL which is not handled
-    by another plugin.
     """
     shorten_url_length = bot.config.url.shorten_url_length
     for url in urls:
         # Exclude URLs that start with the exclusion char
-        if url.startswith(bot.config.url.exclusion_char):
+        if not requested and url.startswith(bot.config.url.exclusion_char):
             continue
 
-        # Check the URL does not match an existing URL callback
-        if check_callbacks(bot, url):
+        parsed_url = urlparse(url)
+
+        if check_callbacks(bot, url, use_excludes=not requested):
+            # URL matches a callback OR is excluded, ignore
+            yield URLInfo(url, None, None, None, True)
             continue
 
         # Prevent private addresses from being queried if enable_private_resolution is False
+        # FIXME: This does nothing when an attacker knows how to host a 302
+        # FIXME: This whole concept has a TOCTOU issue
         if not bot.config.url.enable_private_resolution:
-            parsed = urlparse(url)
-            # Check if it's an address like http://192.168.1.1
+            if not parsed_url.hostname:
+                # URL like file:///path is a valid local path (i.e. private)
+                LOGGER.debug("Ignoring private URL: %s", url)
+                continue
+
             try:
-                if ipaddress.ip_address(parsed.hostname).is_private or ipaddress.ip_address(parsed.hostname).is_loopback:
-                    LOGGER.debug('Ignoring private URL: %s', url)
-                    continue
+                ips = [ip_address(parsed_url.hostname)]
             except ValueError:
-                pass
-
-            # Check if domains are RFC1918 addresses if enable_dns_resolutions is set
-            if bot.config.url.enable_dns_resolution:
-                private = False
-                for result in dns.resolver.query(parsed.hostname):
-                    if ipaddress.ip_address(result).is_private or ipaddress.ip_address(parsed.hostname).is_loopback:
-                        private = True
-                        break
-                if private:
-                    LOGGER.debug('Ignoring private URL: %s', url)
+                # Extra try/except here in case the DNS resolution fails, see #2348
+                try:
+                    ips = [ip_address(ip) for ip in dns.resolver.resolve(parsed_url.hostname)]
+                except Exception as exc:
+                    LOGGER.debug(
+                        "Cannot resolve hostname %s, ignoring URL %s"
+                        " (exception was: %r)",
+                        parsed_url.hostname,
+                        url,
+                        exc,
+                    )
                     continue
 
+            private = False
+            for ip in ips:
+                if ip.is_private or ip.is_loopback:
+                    private = True
+                    break
+            if private:
+                LOGGER.debug("Ignoring private URL: %s", url)
+                continue
+
         # Call the URL to get a title, if possible
         title = find_title(url)
         if not title:
             # No title found: don't handle this URL
             LOGGER.debug('No title found; ignoring URL: %s', url)
             continue
 
         # If the URL is over bot.config.url.shorten_url_length, shorten the URL
         tinyurl = None
         if (shorten_url_length > 0) and (len(url) > shorten_url_length):
             tinyurl = get_or_create_shorturl(bot, url)
 
-        yield (url, title, get_hostname(url), tinyurl)
+        yield URLInfo(url, title, parsed_url.hostname, tinyurl, False)
 
 
-def check_callbacks(bot, url):
+def check_callbacks(bot: SopelWrapper, url: str, use_excludes: bool = True) -> bool:
     """Check if ``url`` is excluded or matches any URL callback patterns.
 
     :param bot: Sopel instance
-    :param str url: URL to check
+    :param url: URL to check
+    :param use_excludes: Use or ignore the configured exclusion lists
     :return: True if ``url`` is excluded or matches any URL callback pattern
 
     This function looks at the ``bot.memory`` for ``url_exclude`` patterns and
     it returns ``True`` if any matches the given ``url``. Otherwise, it looks
     at the ``bot``'s URL callback patterns, and it returns ``True`` if any
     matches, ``False`` otherwise.
 
     .. seealso::
 
-        The :func:`~sopel.modules.url.setup` function that defines the
+        The :func:`~sopel.builtins.url.setup` function that defines the
         ``url_exclude`` in ``bot.memory``.
 
     .. versionchanged:: 7.0
 
         This function **does not** trigger URL callbacks anymore when ``url``
         matches a pattern.
 
     """
     # Check if it matches the exclusion list first
-    matched = any(regex.search(url) for regex in bot.memory['url_exclude'])
+    excluded = use_excludes and any(
+        regex.search(url) for regex in bot.memory["url_exclude"]
+    )
     return (
-        matched or
+        excluded or
         any(bot.search_url_callbacks(url)) or
         bot.rules.check_url_callback(bot, url)
     )
 
 
-def find_title(url, verify=True):
-    """Return the title for the given URL."""
+def find_title(url: str, verify: bool = True) -> Optional[str]:
+    """Return the title for the given URL.
+
+    :param verify: Whether to require a valid certificate when using https
+    """
     try:
         response = requests.get(url, stream=True, verify=verify,
                                 headers=DEFAULT_HEADERS)
-        content = b''
+        raw_content = b''
         for byte in response.iter_content(chunk_size=512):
-            content += byte
-            if b'</title>' in content or len(content) > MAX_BYTES:
+            raw_content += byte
+            if b'</title>' in raw_content or len(raw_content) > MAX_BYTES:
                 break
-        content = content.decode('utf-8', errors='ignore')
+        content = raw_content.decode('utf-8', errors='ignore')
         # Need to close the connection because we have not read all
         # the data
         response.close()
-    except requests.exceptions.ConnectionError:
-        LOGGER.debug('Unable to reach URL: %s', url, exc_info=True)
+    except requests.exceptions.ConnectionError as e:
+        LOGGER.debug("Unable to reach URL: %r: %s", url, e)
         return None
     except (
         requests.exceptions.InvalidURL,  # e.g. http:///
         UnicodeError,  # e.g. http://.example.com (urllib3<1.26)
         LocationValueError,  # e.g. http://.example.com (urllib3>=1.26)
     ):
         LOGGER.debug('Invalid URL: %s', url)
@@ -440,46 +539,30 @@
     # we'll keep it (with the compiled regexes made global) for now.
     content = TITLE_TAG_DATA.sub(r'<\1title>', content)
     content = QUOTED_TITLE.sub('', content)
 
     start = content.rfind('<title>')
     end = content.rfind('</title>')
     if start == -1 or end == -1:
-        return
+        return None
+
     title = web.decode(content[start + 7:end])
     title = title.strip()[:200]
 
     title = ' '.join(title.split())  # cleanly remove multiple spaces
 
-    # More cryptic regex substitutions. This one looks to be myano's invention.
-    title = RE_DCC.sub('', title)
-
     return title or None
 
 
-def get_hostname(url):
-    idx = 7
-    if url.startswith('https://'):
-        idx = 8
-    elif url.startswith('ftp://'):
-        idx = 6
-    hostname = url[idx:]
-    slash = hostname.find('/')
-    if slash != -1:
-        hostname = hostname[:slash]
-    return hostname
-
-
-def get_or_create_shorturl(bot, url):
+def get_or_create_shorturl(bot: SopelWrapper, url: str) -> Optional[str]:
     """Get or create a short URL for ``url``
 
     :param bot: Sopel instance
-    :param str url: URL to get or create a short URL for
+    :param url: URL to get or create a short URL for
     :return: A short URL
-    :rtype: str
 
     It gets the short URL for ``url`` from the bot's memory if it exists.
     Otherwise, it creates a short URL (see :func:`get_tinyurl`), stores it
     into the bot's memory, then returns it.
     """
     # Check bot memory to see if the shortened URL is already in
     # memory
@@ -487,15 +570,15 @@
         return bot.memory['shortened_urls'][url]
 
     tinyurl = get_tinyurl(url)
     bot.memory['shortened_urls'][url] = tinyurl
     return tinyurl
 
 
-def get_tinyurl(url):
+def get_tinyurl(url: str) -> Optional[str]:
     """Returns a shortened tinyURL link of the URL"""
     base_url = "https://tinyurl.com/api-create.php"
     tinyurl = "%s?%s" % (base_url, web.urlencode({'url': url}))
     try:
         res = requests.get(tinyurl)
         res.raise_for_status()
     except requests.exceptions.RequestException:
```

### Comparing `sopel-7.1.9/sopel/modules/version.py` & `sopel-8.0.0/sopel/builtins/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# coding=utf-8
 """
 version.py - Sopel Version Plugin
 Copyright 2009, Silas Baronda
 Copyright 2014, Dimitri Molenaars <tyrope@tyrope.nl>
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import datetime
 import os
 import platform
 
 from sopel import __version__ as release, plugin
 
@@ -30,21 +29,42 @@
             with open(head_file) as h:
                 sha = h.readline()
                 if sha:
                     return sha
 
 
 @plugin.command('version')
+@plugin.example('.version [plugin_name]')
 @plugin.output_prefix('[version] ')
 def version(bot, trigger):
-    """Display the installed version of Sopel.
+    """Display the installed version of Sopel or a plugin.
 
     Includes the version of Python Sopel is installed on.
     Includes the commit hash if Sopel is installed from source.
     """
+    plugin = trigger.group(3)
+    if plugin and plugin.lower() != "sopel":
+        # Plugin version
+        if not bot.has_plugin(plugin):
+            bot.say("I don't have a plugin named %r loaded." % plugin)
+            return
+
+        meta = bot.get_plugin_meta(plugin)
+        if meta["version"] is None:
+            version = "(unknown)"
+        else:
+            version = "v" + str(meta["version"])
+
+        if meta["source"].startswith("sopel."):
+            version += " (built in)"
+
+        bot.say(plugin + " " + version)
+        return
+
+    # Sopel version
     parts = [
         'Sopel v%s' % release,
         'Python: %s' % platform.python_version()
     ]
     sha = git_info()
     if sha:
         parts.append('Commit: %s' % sha)
```

### Comparing `sopel-7.1.9/sopel/modules/wikipedia.py` & `sopel-8.0.0/sopel/builtins/wikipedia.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-# coding=utf-8
 """
 wikipedia.py - Sopel Wikipedia Plugin
 Copyright 2013 Elsie Powell - embolalia.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+from html.parser import HTMLParser
 import logging
 import re
+from urllib.parse import quote, unquote, urlparse
 
 from requests import get
 
 from sopel import plugin
 from sopel.config import types
-from sopel.tools.web import quote, unquote
 
-try:  # TODO: Remove fallback when dropping py2
-    from html.parser import HTMLParser
-except ImportError:
-    from HTMLParser import HTMLParser
 
 LOGGER = logging.getLogger(__name__)
+
 REDIRECT = re.compile(r'^REDIRECT (.*)')
 PLUGIN_OUTPUT_PREFIX = '[wikipedia] '
 
 
 class WikiParser(HTMLParser):
     NO_CONSUME_TAGS = ('sup', 'style')
     """Tags whose contents should always be ignored.
@@ -125,19 +122,14 @@
     def get_result(self):
         return self.result
 
 
 class WikipediaSection(types.StaticSection):
     default_lang = types.ValidatedAttribute('default_lang', default='en')
     """The default language to find articles from (same as Wikipedia language subdomain)."""
-    lang_per_channel = types.ValidatedAttribute('lang_per_channel')
-    """List of ``#channel:langcode`` pairs to define Wikipedia language per channel.
-
-    Deprecated: Will be removed in Sopel 8. Use ``.wpclang`` to manage per-channel language settings.
-    """
 
 
 def setup(bot):
     bot.config.define_section('wikipedia', WikipediaSection)
 
 
 def configure(config):
@@ -160,25 +152,14 @@
         return user_lang
 
     if not trigger.sender.is_nick():
         channel_lang = bot.db.get_channel_value(trigger.sender, 'wikipedia_lang')
         if channel_lang:
             return channel_lang
 
-    if bot.config.wikipedia.lang_per_channel:
-        customlang = re.search('(' + trigger.sender + r'):(\w+)',
-                               bot.config.wikipedia.lang_per_channel)
-        if customlang is not None:
-            LOGGER.warning(
-                'Language for %s loaded from the deprecated config setting, '
-                'wikipedia.lang_per_channel',
-                trigger.sender,
-            )
-            return customlang.group(2)
-
     return bot.config.wikipedia.default_lang
 
 
 def mw_search(server, query, num):
     """Search a MediaWiki site
 
     Searches the specified MediaWiki server for the given query, and returns
@@ -191,28 +172,34 @@
     query = get(search_url).json()
     if 'query' in query:
         query = query['query']['search']
         return [r['title'] for r in query]
     return None
 
 
-def say_snippet(bot, trigger, server, query, show_url=True):
+def say_snippet(bot, trigger, server, query, show_url=True, commanded=False):
     page_name = query.replace('_', ' ')
     query = quote(query.replace(' ', '_'))
     url = 'https://{}/wiki/{}'.format(server, query)
 
     # If the trigger looks like another instance of this plugin, assume it is
     if trigger.startswith(PLUGIN_OUTPUT_PREFIX) and trigger.endswith(' | ' + url):
         return
 
     try:
         snippet = mw_snippet(server, query)
+        # Coalesce repeated whitespace to avoid problems with <math> on MediaWiki
+        # see https://github.com/sopel-irc/sopel/issues/2259
+        snippet = re.sub(r"\s+", " ", snippet)
     except KeyError:
-        if show_url:
-            bot.reply("Error fetching snippet for \"{}\".".format(page_name))
+        msg = 'Error fetching snippet for "{}".'.format(page_name)
+        if commanded:
+            bot.reply(msg)
+        else:
+            bot.say(msg)
         return
 
     msg = '{} | "{}'.format(page_name, snippet)
 
     trailing = '"'
     if show_url:
         trailing += ' | ' + url
@@ -238,15 +225,15 @@
 
 def say_section(bot, trigger, server, query, section):
     page_name = query.replace('_', ' ')
     query = quote(query.replace(' ', '_'))
 
     snippet = mw_section(server, query, section)
     if not snippet:
-        bot.reply("Error fetching section \"{}\" for page \"{}\".".format(section, page_name))
+        bot.say('Error fetching section "{}" for page "{}".'.format(section, page_name))
         return
 
     msg = '{} - {} | "{}"'.format(page_name, section.replace('_', ' '), snippet)
     bot.say(msg, truncation=' […]"')
 
 
 def mw_section(server, query, section):
@@ -255,59 +242,124 @@
     on the given server.
     """
     sections_url = ('https://{0}/w/api.php?format=json&redirects'
                     '&action=parse&prop=sections&page={1}'
                     .format(server, query))
     sections = get(sections_url).json()
 
-    section_number = None
+    fetch_title = section_number = None
 
     for entry in sections['parse']['sections']:
         if entry['anchor'] == section:
             section_number = entry['index']
             # Needed to handle sections from transcluded pages properly
             # e.g. template documentation (usually pulled in from /doc subpage).
             # One might expect this prop to be nullable because in most cases it
             # will simply repeat the requested page title, but it's always set.
-            fetch_title = quote(entry['fromtitle'])
+            fetch_title = entry.get('fromtitle')
             break
 
-    if not section_number:
+    if section_number is None or fetch_title is None:
         return None
 
     snippet_url = ('https://{0}/w/api.php?format=json&redirects'
                    '&action=parse&page={1}&prop=text'
-                   '&section={2}').format(server, fetch_title, section_number)
+                   '&section={2}').format(server, quote(fetch_title), section_number)
 
     data = get(snippet_url).json()
 
     parser = WikiParser(section.replace('_', ' '))
     parser.feed(data['parse']['text']['*'])
     text = parser.get_result()
     text = ' '.join(text.split())  # collapse multiple whitespace chars
 
     return text
 
 
-# Matches a wikipedia page (excluding spaces and #, but not /File: links), with a separate optional field for the section
-@plugin.url(r'https?:\/\/([a-z]+(?:\.m)?\.wikipedia\.org)\/wiki\/((?!File\:)[^ #]+)#?([^ ]*)')
+def say_image_description(bot, trigger, server, image):
+    desc = mw_image_description(server, image)
+
+    if desc:
+        bot.say(desc, truncation=" […]")
+
+
+def mw_image_description(server, image):
+    """Retrieves the description for the given image."""
+    params = "&".join([
+        "action=query",
+        "prop=imageinfo",
+        "format=json",
+        "indexpageids=1",
+        "iiprop=extmetadata",
+        "iiextmetadatafilter=ImageDescription",
+        "iilimit=1",
+        "titles={image}".format(image=image),
+    ])
+    url = "https://{server}/w/api.php?{params}".format(server=server, params=params)
+
+    response = get(url)
+    json = response.json()
+
+    try:
+        query_data = json["query"]
+        pageids = query_data["pageids"]
+        pages = query_data["pages"]
+
+        page = pages[pageids[0]]
+
+        raw_desc = page["imageinfo"][0]["extmetadata"]["ImageDescription"]["value"]
+
+    except LookupError:
+        LOGGER.exception("Error getting image description for %r, response was: %r", image, json)
+        return None
+
+    # Some descriptions contain markup, use WikiParser to discard that
+    parser = WikiParser(image)
+    parser.feed(raw_desc)
+    desc = parser.get_result()
+    desc = ' '.join(desc.split())  # collapse multiple whitespace chars
+
+    return desc
+
+
+# Matches a Wikipedia link (excluding /File: pages)
+@plugin.url(r'https?:\/\/([a-z]+(?:\.m)?\.wikipedia\.org)\/wiki\/((?!File\:)[^ ]+)')
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def mw_info(bot, trigger, match=None):
     """Retrieves and outputs a snippet of the linked page."""
-    if match.group(3):
-        if match.group(3).startswith('cite_note-'):  # Don't bother trying to retrieve a snippet when cite-note is linked
-            say_snippet(bot, trigger, match.group(1), unquote(match.group(2)), show_url=False)
+    server = match.group(1)
+    page_info = urlparse(match.group(0))
+    # in Python 3.9+ this can be str.removeprefix() instead, but we're confident that
+    # "/wiki/" is at the start of the path anyway since it's part of the pattern
+    trim_offset = len("/wiki/")
+    article = unquote(page_info.path)[trim_offset:]
+    section = unquote(page_info.fragment)
+
+    if article.startswith("Special:"):
+        # The MediaWiki query API does not include pages in the Special:
+        # namespace, so there's no point bothering when we know this will error
+        LOGGER.debug("Ignoring page in Special: namespace")
+        return False
+
+    if section:
+        if section.startswith('cite_note-'):
+            # Don't bother trying to retrieve a section snippet if cite-note is linked
+            say_snippet(bot, trigger, server, article, show_url=False)
+        elif section.startswith('/media'):
+            # gh2316: media fragments are usually images; try to get an image description
+            image = section[7:]  # strip '/media' prefix in pre-3.9 friendly way
+            say_image_description(bot, trigger, server, image)
         else:
-            say_section(bot, trigger, match.group(1), unquote(match.group(2)), unquote(match.group(3)))
+            say_section(bot, trigger, server, article, section)
     else:
-        say_snippet(bot, trigger, match.group(1), unquote(match.group(2)), show_url=False)
+        say_snippet(bot, trigger, server, article, show_url=False)
 
 
-@plugin.command('w', 'wiki', 'wik')
-@plugin.example('.w San Francisco')
+@plugin.command('wikipedia', 'wp')
+@plugin.example('.wp San Francisco')
 @plugin.output_prefix('[wikipedia] ')
 def wikipedia(bot, trigger):
     """Search Wikipedia."""
     if trigger.group(2) is None:
         bot.reply("What do you want me to look up?")
         return plugin.NOLIMIT
 
@@ -317,61 +369,69 @@
     if args is not None:
         lang = args.group(1)
         query = args.group(2)
 
     if not query:
         bot.reply('What do you want me to look up?')
         return plugin.NOLIMIT
+
+    if query.startswith("Special:"):
+        bot.reply("Sorry, the MediaWiki API doesn't support querying the Special: namespace.")
+        return False
+
     server = lang + '.wikipedia.org'
     query = mw_search(server, query, 1)
     if not query:
         bot.reply("I can't find any results for that.")
         return plugin.NOLIMIT
     else:
         query = query[0]
-    say_snippet(bot, trigger, server, query)
+    say_snippet(bot, trigger, server, query, commanded=True)
 
 
 @plugin.command('wplang')
 @plugin.example('.wplang pl')
 def wplang(bot, trigger):
     if not trigger.group(3):
         bot.reply(
             "Your current Wikipedia language is: {}"
             .format(
                 bot.db.get_nick_value(
                     trigger.nick, 'wikipedia_lang',
                     bot.config.wikipedia.default_lang)
             )
         )
-    else:
-        bot.db.set_nick_value(trigger.nick, 'wikipedia_lang', trigger.group(3))
-        bot.reply(
-            "Set your Wikipedia language to: {}"
-            .format(trigger.group(3))
-        )
+        return
+
+    bot.db.set_nick_value(trigger.nick, 'wikipedia_lang', trigger.group(3))
+    bot.reply(
+        "Set your Wikipedia language to: {}"
+        .format(trigger.group(3))
+    )
 
 
 @plugin.command('wpclang')
 @plugin.example('.wpclang ja')
 @plugin.require_chanmsg()
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def wpclang(bot, trigger):
     if not (trigger.admin or bot.channels[trigger.sender.lower()].privileges[trigger.nick.lower()] >= plugin.OP):
         bot.reply("You don't have permission to change this channel's Wikipedia language setting.")
         return plugin.NOLIMIT
+
     if not trigger.group(3):
         bot.say(
             "{}'s current Wikipedia language is: {}"
             .format(
                 trigger.sender,
                 bot.db.get_nick_value(
                     trigger.nick, 'wikipedia_lang',
                     bot.config.wikipedia.default_lang)
             )
         )
-    else:
-        bot.db.set_channel_value(trigger.sender, 'wikipedia_lang', trigger.group(3))
-        bot.say(
-            "Set {}'s Wikipedia language to: {}"
-            .format(trigger.sender, trigger.group(3))
-        )
+        return
+
+    bot.db.set_channel_value(trigger.sender, 'wikipedia_lang', trigger.group(3))
+    bot.say(
+        "Set {}'s Wikipedia language to: {}"
+        .format(trigger.sender, trigger.group(3))
+    )
```

### Comparing `sopel-7.1.9/sopel/modules/wiktionary.py` & `sopel-8.0.0/sopel/builtins/wiktionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# coding=utf-8
 """
 wiktionary.py - Sopel Wiktionary Plugin
 Copyright 2009, Sean B. Palmer, inamidst.com
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import re
 
 import requests
 
 from sopel import plugin
 from sopel.tools import web
@@ -55,15 +54,15 @@
 
 def wikt(word):
     bytes = requests.get(uri % web.quote(word)).text
     bytes = r_ul.sub('', bytes)
 
     mode = None
     etymology = None
-    definitions = {}
+    definitions: dict[str, list[str]] = {}
     for line in bytes.splitlines():
         is_new_mode = False
         if 'id="Etymology' in line:
             mode = 'etymology'
             is_new_mode = True
         else:
             for pos in PARTS_OF_SPEECH:
```

### Comparing `sopel-7.1.9/sopel/modules/xkcd.py` & `sopel-8.0.0/sopel/builtins/xkcd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-# coding=utf-8
 """
 xkcd.py - Sopel xkcd Plugin
 Copyright 2010, Michael Yanovich (yanovich.net), and Morgan Goose
 Copyright 2012, Lior Ramati
 Copyright 2013, Elsie Powell (embolalia.com)
 Licensed under the Eiffel Forum License 2.
 
 https://sopel.chat
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+from json import JSONDecodeError
+import logging
 import random
 import re
 
 import requests
 
 from sopel import plugin
-from sopel.modules.search import bing_search
+from sopel.builtins.search import duck_search
 
+LOGGER = logging.getLogger(__name__)
 PLUGIN_OUTPUT_PREFIX = '[xkcd] '
 
+# used with permission of site owner
+# https://twitter.com/Dmdboi/status/1589202274999767041
+SEARCHXKCD_API = 'https://gq67pznq1k.execute-api.eu-west-1.amazonaws.com/search'
+
 ignored_sites = [
     # For searching the web
     'almamater.xkcd.com',
     'blog.xkcd.com',
     'blag.xkcd.com',
     'forums.xkcd.com',
     'fora.xkcd.com',
@@ -42,20 +48,47 @@
         url = 'https://xkcd.com/info.0.json'
     data = requests.get(url).json()
     data['url'] = 'https://xkcd.com/' + str(data['num'])
     return data
 
 
 def web_search(query):
-    url = bing_search(query + sites_query)
+    url = duck_search(query + sites_query)
     if not url:
         return None
     match = re.match(r'(?:https?://)?(?:m\.)?xkcd\.com/(\d+)/?', url)
     if match:
         return match.group(1)
+    return None
+
+
+def searchxkcd_search(query):
+    parameters = {
+        'q': query,
+        'page': 0,
+    }
+    try:
+        response = requests.post(SEARCHXKCD_API, params=parameters)
+    except requests.exceptions.ConnectionError as e:
+        LOGGER.debug("Unable to reach searchxkcd API: %s", e)
+        return None
+    except Exception as e:
+        LOGGER.debug("Unexpected error calling searchxkcd API: %s", e)
+        return None
+
+    try:
+        hits = response.json()['results']['hits']
+        if not hits:
+            return None
+        first = hits[0]['objectID']
+    except (JSONDecodeError, LookupError):
+        LOGGER.debug("Data format from searchxkcd API could not be understood.")
+        return None
+
+    return first
 
 
 @plugin.command('xkcd')
 @plugin.example(".xkcd 1782", user_help=True)
 @plugin.example(".xkcd", user_help=True)
 @plugin.output_prefix(PLUGIN_OUTPUT_PREFIX)
 def xkcd(bot, trigger):
@@ -87,15 +120,18 @@
                 query = -query
             return numbered_result(bot, query, latest)
         else:
             # Non-number: search the web.
             if (query.lower() == "latest" or query.lower() == "newest"):
                 requested = latest
             else:
-                number = web_search(query)
+                number = searchxkcd_search(query)
+                if number is None:
+                    # generic web-search engine as fallback
+                    number = web_search(query)
                 if not number:
                     bot.reply('Could not find any comics for that query.')
                     return
                 requested = get_info(number)
 
     say_result(bot, requested)
```

### Comparing `sopel-7.1.9/sopel/plugin.py` & `sopel-8.0.0/sopel/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,56 @@
-# coding=utf-8
 """This contains decorators and other tools for creating Sopel plugins."""
 # Copyright 2013, Ari Koivula, <ari@koivu.la>
 # Copyright © 2013, Elad Alfassa <elad@fedoraproject.org>
 # Copyright 2013, Lior Ramati <firerogue517@gmail.com>
 # Copyright 2019, deathbybandaid, deathbybandaid.net
 # Copyright 2019, dgw, technobabbl.es
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 # Licensed under the Eiffel Forum License 2.
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+import enum
 import functools
+import logging
 import re
+from typing import (
+    Callable,
+    Literal,
+    Optional,
+    Pattern,
+    Protocol,
+    TYPE_CHECKING,
+    Union,
+)
+
+# import and expose privileges as shortcut
+from sopel.privileges import AccessLevel
+
+VOICE = AccessLevel.VOICE
+HALFOP = AccessLevel.HALFOP
+OP = AccessLevel.OP
+ADMIN = AccessLevel.ADMIN
+OWNER = AccessLevel.OWNER
+OPER = AccessLevel.OPER
+
+
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+    from sopel.bot import SopelWrapper
 
 __all__ = [
     # constants
     'NOLIMIT', 'VOICE', 'HALFOP', 'OP', 'ADMIN', 'OWNER', 'OPER',
     # decorators
     'action_command',
     'action_commands',
+    'allow_bots',
+    'capability',
+    'CapabilityNegotiation',
     'command',
     'commands',
     'ctcp',
     'echo',
     'event',
     'example',
     'find',
@@ -30,14 +58,17 @@
     'interval',
     'label',
     'nickname_command',
     'nickname_commands',
     'output_prefix',
     'priority',
     'rate',
+    'rate_user',
+    'rate_channel',
+    'rate_global',
     'require_account',
     'require_admin',
     'require_bot_privilege',
     'require_chanmsg',
     'require_owner',
     'require_privilege',
     'require_privmsg',
@@ -48,120 +79,313 @@
     'thread',
     'unblockable',
     'url',
     'url_lazy',
 ]
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 NOLIMIT = 1
 """Return value for ``callable``\\s, which suppresses rate limiting.
 
 Returning this value means the triggering user will not be prevented from
 triggering the same callable again within the rate limit. This can be used,
 for example, to allow a user to retry a failed command immediately.
 
 .. versionadded:: 4.0
 """
 
-VOICE = 1
-"""Privilege level for the +v channel permission
 
-.. versionadded:: 4.1
-"""
+class CapabilityNegotiation(enum.Enum):
+    """Capability Negotiation status."""
 
-HALFOP = 2
-"""Privilege level for the +h channel permission
+    DONE = enum.auto()
+    """The capability negotiation can end.
 
-.. versionadded:: 4.1
+    This must be returned by a capability request handler to signify to the bot
+    that the capability has been properly negotiated and negotiation can end if
+    all other conditions are met.
+    """
 
-.. important::
+    CONTINUE = enum.auto()
+    """The capability negotiation must continue.
 
-    Not all IRC networks support this privilege mode. If you are writing a
-    plugin for public distribution, ensure your code behaves sensibly if only
-    ``+v`` (voice) and ``+o`` (op) modes exist.
+    This must be returned by a capability request handler to signify to the bot
+    that the capability requires further processing (e.g. SASL
+    authentication) and negotiation must not end yet.
 
-"""
+    The plugin author MUST signal the bot once the negotiation is done.
+    """
 
-OP = 4
-"""Privilege level for the +o channel permission
+    ERROR = enum.auto()
+    """The capability negotiation callback was improperly executed.
 
-.. versionadded:: 4.1
-"""
+    If a capability request's handler returns this status, or if it raises an
+    exception, the bot will mark the request as errored. A handler can use this
+    return value to inform the bot that something wrong happened, without being
+    an error in the code itself.
+    """
 
-ADMIN = 8
-"""Privilege level for the +a channel permission
 
-.. versionadded:: 4.1
+class CapabilityHandler(Protocol):
+    """:class:`~typing.Protocol` definition for capability handler.
 
-.. important::
+    When a plugin requests a capability, it can define a callback handler for
+    that request using :class:`capability` as a decorator. That handler will be
+    called upon Sopel receiving either an ``ACK`` (capability enabled) or a
+    ``NAK`` (capability denied) CAP message.
 
-    Not all IRC networks support this privilege mode. If you are writing a
-    plugin for public distribution, ensure your code behaves sensibly if only
-    ``+v`` (voice) and ``+o`` (op) modes exist.
+    Example::
 
-"""
+        from sopel import plugin
+        from sopel.bot import SopelWrapper
 
-OWNER = 16
-"""Privilege level for the +q channel permission
+        @plugin.capability('example/cap-name')
+        def capability_handler(
+            cap_req: tuple[str, ...],
+            bot: SopelWrapper,
+            acknowledged: bool,
+        ) -> plugin.CapabilityNegotiation:
+            if acknowledged:
+                # do something if acknowledged
+                # i.e.
+                # activate a plugin's feature
+                pass
+            else:
+                # do something else if not
+                # i.e. use a fallback mechanism
+                # or deactivate a plugin's feature if needed
+                pass
+
+            # always return if Sopel can send "CAP END" (DONE)
+            # or if the plugin must notify the bot for that later (CONTINUE)
+            return plugin.CapabilityNegotiation.DONE
 
-.. versionadded:: 4.1
+    .. note::
 
-.. important::
+        This protocol class should be used for type checking and documentation
+        purposes only.
 
-    Not all IRC networks support this privilege mode. If you are writing a
-    plugin for public distribution, ensure your code behaves sensibly if only
-    ``+v`` (voice) and ``+o`` (op) modes exist.
+    """
+    def __call__(
+        self,
+        cap_req: tuple[str, ...],
+        bot: SopelWrapper,
+        acknowledged: bool,
+    ) -> CapabilityNegotiation:
+        """A capability handler must be a callable with this signature.
+
+        :param cap_req: the capability request, as a tuple of string
+        :param bot: the bot instance
+        :param acknowledged: that flag that tells if the capability is enabled
+                             or denied
+        :return: the return value indicates if the capability negotiation is
+                 complete for this request or not
+        """
+
+
+class capability:
+    """Decorate a function to request a capability and handle the result.
+
+    :param name: name of the capability to negotiate with the server; this
+                 positional argument can be used multiple times to form a
+                 single ``CAP REQ``
+    :param handler: optional keyword argument, acknowledgement handler
+
+    The Client Capability Negotiation is a feature of IRCv3 that exposes a
+    mechanism for a server to advertise a list of features and for clients to
+    request them when they are available.
+
+    This decorator will register a capability request, allowing the bot to
+    request capabilities if they are available. You can request more than one
+    at a time, which will make for one single request.
 
-"""
+    The handler must follow the :class:`CapabilityHandler` protocol.
 
-OPER = 32
-"""Privilege level for the +y/+Y channel permissions
+    .. note::
 
-Note: Except for these (non-standard) channel modes, Sopel does not monitor or
-store any user's OPER status.
+        Due to how Capability Negotiation works, a request will be acknowledged
+        or denied all at once. This means that this may succeed::
 
-.. versionadded:: 7.0.0
+            @plugin.capability('away-notify')
 
-.. important::
+        But this may not::
 
-    Not all IRC networks support this privilege mode. If you are writing a
-    plugin for public distribution, ensure your code behaves sensibly if only
-    ``+v`` (voice) and ``+o`` (op) modes exist.
+            @plugin.capability('away-notify', 'example/incompatible-cap')
 
-"""
+        Even though the ``away-notify`` capability is available and can be
+        enabled, the second ``CAP REQ`` will be denied because the server won't
+        acknowledge a request that contains an incompatible capability.
+
+        In that case, if you don't need both at the same time, you should use
+        two different handlers::
+
+            @plugin.capability('away-notify')
+            def cap_away_notify(cap_req, bot, ack):
+                # handle away-notify acknowledgement
+
+            @plugin.capability('example/incompatible-cap')
+            def cap_example_incompatible_cap(cap_req, bot, ack):
+                # handle example/incompatible-cap acknowledgement
+                # or, most probably, lack thereof
+
+        This will allow the server to acknowledge or deny each capability
+        independently.
+
+    .. warning::
 
+        A function cannot be decorated more than once by this decorator, as
+        the result is an instance of :class:`capability`.
 
-def unblockable(function):
-    """Decorate a function to exempt it from the ignore/blocks system.
+        If you want to handle a ``CAP`` message without requesting the
+        capability, you should use the :func:`event` decorator instead.
+
+    .. warning::
+
+        The list of ``cap_req`` is limited in size to prevent the bot from
+        separating the ``CAP REQ`` in multiple lines as the bot does not know
+        how to call back the capability handler upon receiving the multi-line
+        ``ACK * REQ``.
+
+    .. seealso::
+
+        The IRCv3 specification on `Client Capability Negotiation`__.
+
+    .. __: https://ircv3.net/specs/extensions/capability-negotiation
+    """
+    def __init__(
+        self,
+        *cap_req: str,
+        handler: Optional[CapabilityHandler] = None,
+    ) -> None:
+        cap_req_text = ' '.join(cap_req)
+        if len(cap_req_text.encode('utf-8')) > 500:
+            # "CAP * ACK " is 10 bytes, leaving 500 bytes for the capabilities.
+            # Sopel cannot allow multi-line requests, as it won't know how to
+            # deal properly with multi-line ACK.
+            # The spec says a client SHOULD send multiple requests; however
+            # the spec also says that a server will ACK or NAK a whole request
+            # at once. So technically, multiple REQs are not the same as a
+            # single REQ.
+            raise ValueError('Capability request too long: %s' % cap_req_text)
+
+        self._cap_req: tuple[str, ...] = tuple(sorted(cap_req))
+        self._handler: Optional[CapabilityHandler] = handler
+
+    def __str__(self) -> str:
+        caps = ", ".join(repr(cap) for cap in self._cap_req)
+        handler = ""
+        if self._handler and hasattr(self._handler, "__name__"):
+            handler = " ({}())".format(self._handler.__name__)
+        return "<capability {}{}>".format(caps, handler)
+
+    @property
+    def cap_req(self) -> tuple[str, ...]:
+        """Capability request as a sorted tuple.
+
+        This is the capability request that will be sent to the server as is.
+        A request is acknowledged or denied for all the capabilities it
+        contains, so the request ``(example/cap1, example/cap2)`` is not the
+        same as two requests, one for ``example/cap1`` and the other for
+        ``example/cap2``. This makes each request unique.
+        """
+        return self._cap_req
+
+    def callback(
+        self,
+        bot: SopelWrapper,
+        acknowledged: bool,
+    ) -> tuple[bool, Optional[CapabilityNegotiation]]:
+        """Execute the acknowlegement callback of a capability request.
+
+        :param bot: a Sopel instance
+        :param acknowledged: tell if the capability request is acknowledged
+                             (``True``) or deny (``False``)
+        :return: a 2-value tuple that contains if the request is done and the
+                 result of the handler (if any)
+
+        It executes the handler when the capability request receives an
+        acknowledgement (either positive or negative), and returns the result.
+        The handler's return value is used to know if the capability
+        request is done, or if the bot must wait for resolution from the plugin
+        that requested the capability.
+
+        This method returns a 2-value tuple:
+
+        * the first value tells if the negotiation is done for this request
+        * the second is the handler's return value (if any)
+
+        If no handler is registered, this automatically returns
+        ``(True, None)``, as the negotiation is considered done (without any
+        result).
+
+        This doesn't prevent the handler from raising an exception.
+        """
+        result: Optional[CapabilityNegotiation] = None
+        if self._handler is not None:
+            result = self._handler(self.cap_req, bot, acknowledged)
+            LOGGER.debug(
+                'Cap request "%s" got "%s", '
+                'executed successfuly with status: %s',
+                ' '.join(self.cap_req),
+                'ACK' if acknowledged else 'NAK',
+                result.name,
+            )
+        return (result is None or result == CapabilityNegotiation.DONE, result)
+
+    def __call__(
+        self,
+        handler: CapabilityHandler,
+    ) -> capability:
+        """Register a capability negotiation callback."""
+        if self._handler is not None:
+            raise RuntimeError("Cannot re-use capability decorator")
+        self._handler = handler
+        return self
+
+
+def unblockable(
+    function: Optional[Callable] = None,
+) -> Callable:
+    """Decorate a function to exempt it from Sopel's ignore system.
 
     For example, this can be used to ensure that important events such as
-    ``JOIN`` are always recorded::
+    ``JOIN`` are always recorded even if the user's nickname or hostname is
+    :ref:`ignored <Ignoring Users>`::
 
         from sopel import plugin
 
         @plugin.event('JOIN')
         @plugin.unblockable
         def on_join_callable(bot, trigger):
-            # do something when a user JOIN a channel
+            # do something when a user JOINs a channel
             # a blocked nickname or hostname *will* trigger this
             pass
 
     .. seealso::
 
         Sopel's :meth:`~sopel.bot.Sopel.dispatch` method.
 
     """
-    function.unblockable = True
-    return function
+    def add_attribute(function):
+        function.unblockable = True
+        return function
 
+    # hack to allow both @unblockable and @unblockable() to work
+    if callable(function):
+        return add_attribute(function)
+    return add_attribute
 
-def interval(*intervals):
+
+def interval(*intervals: Union[int, float]) -> Callable:
     """Decorate a function to be called by the bot every *n* seconds.
 
-    :param int intervals: one or more duration(s), in seconds
+    :param intervals: one or more duration(s), in seconds
 
     This decorator can be used multiple times for multiple intervals, or
     multiple intervals can be given in multiple arguments. The first time the
     function will be called is *n* seconds after the bot was started.
 
     Plugin functions decorated by ``interval`` must only take
     :class:`bot <sopel.bot.Sopel>` as their argument; they do not get a ``trigger``.
@@ -189,18 +413,18 @@
             if arg not in function.interval:
                 function.interval.append(arg)
         return function
 
     return add_attribute
 
 
-def rule(*patterns):
+def rule(*patterns: Union[str, Pattern]) -> Callable:
     """Decorate a function to be called when a line matches the given pattern.
 
-    :param str patterns: one or more regular expression(s)
+    :param patterns: one or more regular expression(s)
 
     Each argument is a regular expression which will trigger the function::
 
         @rule('hello', 'how')
             # will trigger once on "how are you?"
             # will trigger once on "hello, what's up?"
 
@@ -244,20 +468,19 @@
             if value not in function.rule:
                 function.rule.append(value)
         return function
 
     return add_attribute
 
 
-def rule_lazy(*loaders):
+def rule_lazy(*loaders: Callable) -> Callable:
     """Decorate a callable as a rule with lazy loading.
 
     :param loaders: one or more functions to generate a list of **compiled**
                     regexes to match URLs
-    :type loaders: :term:`function`
 
     Each ``loader`` function must accept a ``settings`` parameter and return a
     list (or tuple) of **compiled** regular expressions::
 
         import re
 
         def loader(settings):
@@ -292,18 +515,18 @@
         if not hasattr(function, 'rule_lazy_loaders'):
             function.rule_lazy_loaders = []
         function.rule_lazy_loaders.extend(loaders)
         return function
     return decorator
 
 
-def find(*patterns):
+def find(*patterns: Union[str, Pattern]) -> Callable:
     """Decorate a function to be called for each time a pattern is found in a line.
 
-    :param str patterns: one or more regular expression(s)
+    :param patterns: one or more regular expression(s)
 
     Each argument is a regular expression which will trigger the function::
 
         @find('hello', 'here')
             # will trigger once on "hello you"
             # will trigger twice on "hello here"
             # will trigger once on "I'm right here!"
@@ -347,20 +570,19 @@
             if value not in function.find_rules:
                 function.find_rules.append(value)
         return function
 
     return add_attribute
 
 
-def find_lazy(*loaders):
+def find_lazy(*loaders: Callable) -> Callable:
     """Decorate a callable as a find rule with lazy loading.
 
     :param loaders: one or more functions to generate a list of **compiled**
                     regexes to match patterns in a line
-    :type loaders: :term:`function`
 
     Each ``loader`` function must accept a ``settings`` parameter and return a
     list (or tuple) of **compiled** regular expressions::
 
         import re
 
         def loader(settings):
@@ -395,18 +617,18 @@
         if not hasattr(function, 'find_rules_lazy_loaders'):
             function.find_rules_lazy_loaders = []
         function.find_rules_lazy_loaders.extend(loaders)
         return function
     return decorator
 
 
-def search(*patterns):
+def search(*patterns: Union[str, Pattern]) -> Callable:
     """Decorate a function to be called when a pattern matches anywhere in a line.
 
-    :param str patterns: one or more regular expression(s)
+    :param patterns: one or more regular expression(s)
 
     Each argument is a regular expression which will trigger the function::
 
         @search('hello', 'here')
             # will trigger once on "hello you"
             # will trigger twice on "hello here"
             # will trigger once on "I'm right here!"
@@ -453,20 +675,19 @@
             if value not in function.search_rules:
                 function.search_rules.append(value)
         return function
 
     return add_attribute
 
 
-def search_lazy(*loaders):
+def search_lazy(*loaders: Callable) -> Callable:
     """Decorate a callable as a search rule with lazy loading.
 
     :param loaders: one or more functions to generate a list of **compiled**
                     regexes to match patterns in a line
-    :type loaders: :term:`function`
 
     Each ``loader`` function must accept a ``settings`` parameter and return a
     list (or tuple) of **compiled** regular expressions::
 
         import re
 
         def loader(settings):
@@ -501,19 +722,19 @@
         if not hasattr(function, 'search_rules_lazy_loaders'):
             function.search_rules_lazy_loaders = []
         function.search_rules_lazy_loaders.extend(loaders)
         return function
     return decorator
 
 
-def thread(value):
+def thread(value: bool) -> Callable:
     """Decorate a function to specify if it should be run in a separate thread.
 
-    :param bool value: if ``True``, the function is called in a separate thread;
-                       otherwise, from the bot's main thread
+    :param value: if ``True``, the function is called in a separate thread;
+                  otherwise, from the bot's main thread
 
     Functions run in a separate thread (as is the default) will not prevent the
     bot from executing other functions at the same time. Functions not run in a
     separate thread may be started while other functions are still running, but
     additional functions will not start until it is completed.
     """
     threaded = bool(value)
@@ -521,34 +742,65 @@
     def add_attribute(function):
         function.thread = threaded
         return function
 
     return add_attribute
 
 
-def echo(function=None):
+def allow_bots(
+    function: Optional[Callable] = None,
+) -> Callable:
+    """Decorate a function to specify that it should receive events from bots.
+
+    On networks implementing the `Bot Mode specification`__, messages and
+    other events from other clients that have identified themselves as bots
+    will be tagged as such, and Sopel will ignore them by default. This
+    decorator allows a function to opt into receiving these events.
+
+    .. __: https://ircv3.net/specs/extensions/bot-mode
+    """
+    def add_attribute(function):
+        function.allow_bots = True
+        return function
+
+    # hack to allow both @allow_bots and @allow_bots() to work
+    if callable(function):
+        return add_attribute(function)
+    return add_attribute
+
+
+def echo(
+    function: Optional[Callable] = None,
+) -> Callable:
     """Decorate a function to specify that it should receive echo messages.
 
     This decorator can be used to listen in on the messages that Sopel is
     sending and react accordingly.
+
+    .. important::
+
+        The decorated callable will receive *all* matching messages that Sopel
+        sends, including output from the same callable. Take care to avoid
+        creating feedback loops when using this feature.
+
     """
     def add_attribute(function):
         function.echo = True
         return function
 
     # hack to allow both @echo and @echo() to work
     if callable(function):
         return add_attribute(function)
     return add_attribute
 
 
-def command(*command_list):
+def command(*command_list: str) -> Callable:
     """Decorate a function to set one or more commands that should trigger it.
 
-    :param str command_list: one or more command name(s) to match
+    :param command_list: one or more command name(s) to match
 
     This decorator can be used to add multiple commands to one callable in a
     single line. The resulting match object will have the command as the first
     group; the rest of the line, excluding leading whitespace, as the second
     group; and parameters 1 through 4, separated by whitespace, as groups 3-6.
 
     Example::
@@ -606,25 +858,24 @@
         See also the `Function Definitions`__ chapter from the Python
         documentation for more information about functions and decorators.
 
         .. __: https://docs.python.org/3/reference/compound_stmts.html#function-definitions
 
     .. note::
 
-        You can use a regular expression for the command name(s), but this is
-        **not recommended** since version 7.1. For backward compatibility,
-        this behavior will be kept until version 8.0.
-
-        Regex patterns are confusing for your users; please don't use them in
-        command names!
-
-        If you still want to use a regex pattern, please use the :func:`rule`
-        decorator instead. For extra arguments and subcommands based on a regex
-        pattern, you should handle these inside your decorated function, by
-        using the ``trigger`` object.
+        The command name will be escaped for use in a regular expression.
+        As such it is not possible to use something like ``.command\\d+`` to
+        catch something like ``.command1`` or ``.command2``.
+
+        You have several options at your disposal to replace a regex in the
+        command name:
+
+        * use a command alias
+        * parse the arguments with your own regex within your plugin callable
+        * use a :func:`rule` instead
 
     """
     def add_attribute(function):
         function._sopel_callable = True
         if not hasattr(function, "commands"):
             function.commands = []
         for command in command_list:
@@ -634,18 +885,18 @@
     return add_attribute
 
 
 commands = command
 """Alias to :func:`command`."""
 
 
-def nickname_command(*command_list):
+def nickname_command(*command_list: str) -> Callable:
     """Decorate a function to trigger on lines starting with "$nickname: command".
 
-    :param str command_list: one or more command name(s) to match
+    :param command_list: one or more command name(s) to match
 
     This decorator can be used to add multiple commands to one callable in a
     single line. The resulting match object will have the command as the first
     group; the rest of the line, excluding leading whitespace, as the second
     group; and parameters 1 through 4, separated by whitespace, as groups 3-6.
 
     Example::
@@ -653,23 +904,26 @@
         @nickname_command("hello!")
             # Would trigger on "$nickname: hello!", "$nickname,   hello!",
             # "$nickname hello!", "$nickname hello! parameter1" and
             # "$nickname hello! p1 p2 p3 p4 p5 p6 p7 p8 p9".
 
     .. note::
 
-        You can use a regular expression for the command name(s), but this is
-        **not recommended** since version 7.1. For backward compatibility,
-        this behavior will be kept until version 8.0.
+        The command name will be escaped to be used in a regex command. As such
+        it is not possible to use something like ``command\\d+`` to catch
+        something like ``Bot: command1`` or ``Bot: command2``.
+
+        You have several options at your disposal to replace a regex in the
+        command name:
+
+        * use a command alias
+        * parse the arguments with your own regex within your plugin callable
+        * use a :func:`rule`
 
-        Regex patterns are confusing for your users; please don't use them in
-        command names!
-
-        If you need to use a regex pattern, please use the :func:`rule`
-        decorator instead, with the ``$nick`` variable::
+        The :func:`rule` can be used with a ``$nick`` variable::
 
             @rule(r'$nick .*')
                 # Would trigger on anything starting with "$nickname[:,]? ",
                 # and would never have any additional parameters, as the
                 # command would match the rest of the line.
 
     """
@@ -684,18 +938,18 @@
     return add_attribute
 
 
 nickname_commands = nickname_command
 """Alias to :func:`nickname_command`."""
 
 
-def action_command(*command_list):
+def action_command(*command_list: str) -> Callable:
     """Decorate a function to trigger on CTCP ACTION lines.
 
-    :param str command_list: one or more command name(s) to match
+    :param command_list: one or more command name(s) to match
 
     This decorator can be used to add multiple commands to one callable in a
     single line. The resulting match object will have the command as the first
     group; the rest of the line, excluding leading whitespace, as the second
     group; and parameters 1 through 4, separated by whitespace, as groups 3-6.
 
     Example::
@@ -703,23 +957,26 @@
         @action_command("hello!")
             # Would trigger on "/me hello!"
 
     .. versionadded:: 7.0
 
     .. note::
 
-        You can use a regular expression for the command name(s), but this is
-        **not recommended** since version 7.1. For backward compatibility,
-        this behavior will be kept until version 8.0.
-
-        Regex patterns are confusing for your users; please don't use them in
-        command names!
+        The command name will be escaped for use in a regular expression.
+        As such it is not possible to use something like ``/me command\\d+``
+        to catch something like ``/me command1`` or ``/me command2``.
+
+        You have several options at your disposal to replace a regex in the
+        command name:
+
+        * use a command alias
+        * parse the arguments with your own regex within your plugin callable
+        * use a :func:`rule`
 
-        If you need to use a regex pattern, please use the :func:`rule`
-        decorator instead, with the :func:`ctcp` decorator::
+        The :func:`rule` must be used with the :func:`ctcp` decorator::
 
             @rule(r'hello!?')
             @ctcp('ACTION')
                 # Would trigger on "/me hello!" and "/me hello"
 
     """
     def add_attribute(function):
@@ -733,18 +990,18 @@
     return add_attribute
 
 
 action_commands = action_command
 """Alias to :func:`action_command`."""
 
 
-def label(value):
+def label(value: str) -> Callable:
     """Decorate a function to add a rule label.
 
-    :param str value: a label for the rule
+    :param value: a label for the rule
 
     The rule label allows the documentation and the logging system to refer
     to this function by its label. A function can have one and only one label::
 
         @label('on_hello')
         @rule('hello')
             # will trigger on hello, and be labelled as "on_hello"
@@ -759,33 +1016,33 @@
     """
     def add_attribute(function):
         function.rule_label = value
         return function
     return add_attribute
 
 
-def priority(value):
+def priority(value: Literal['low', 'medium', 'high']) -> Callable:
     """Decorate a function to be executed with higher or lower priority.
 
-    :param str value: one of ``high``, ``medium``, or ``low``;
-                      defaults to ``medium``
+    :param value: one of ``high``, ``medium``, or ``low``
 
-    The priority allows you to control the order of callable execution, if your
-    plugin needs it.
+    The priority allows you some control over the order of callable execution,
+    if your plugin needs it. If a callable does not specify its ``priority``,
+    Sopel assumes ``medium``.
     """
     def add_attribute(function):
         function.priority = value
         return function
     return add_attribute
 
 
-def event(*event_list):
+def event(*event_list: str) -> Callable:
     """Decorate a function to be triggered on specific IRC events.
 
-    :param str event_list: one or more event name(s) on which to trigger
+    :param event_list: one or more event name(s) on which to trigger
 
     This is one of a number of events, such as 'JOIN', 'PART', 'QUIT', etc.
     (More details can be found in RFC 1459.) When the Sopel bot is sent one of
     these events, the function will execute. Note that the default
     :meth:`rule` (``.*``) will match *any* line of the correct event type(s).
     If any rule is explicitly specified, it overrides the default.
 
@@ -802,31 +1059,56 @@
         for name in event_list:
             if name not in function.event:
                 function.event.append(name)
         return function
     return add_attribute
 
 
-def ctcp(function=None, *command_list):
+def ctcp(
+    function: Union[Callable, Optional[str]] = None,
+    *command_list: str,
+) -> Callable:
     """Decorate a callable to trigger on CTCP commands (mostly, ``ACTION``).
 
-    :param str command_list: one or more CTCP command(s) on which to trigger
+    :param command_list: one or more CTCP command(s) on which to trigger
+
+    There are `various CTCP commands`__ to handle with this decorator, such as
+    ``ACTION``, ``CLIENTINFO``, ``TIME``, and ``VERSION``::
+
+        from sopel import plugin
+
+        @plugin.ctcp('TIME')
+        @plugin.rule('.*')
+        def ctcp_time(bot, trigger):
+            bot.say('Sorry, not a clock.')
+
+    This decorator also works without parentheses, in which case it will trigger
+    on CTCP ``ACTION``::
+
+        from sopel import plugin
+
+        @plugin.ctcp
+        @plugin.rule('.*')
+        def ctcp_action(bot, trigger):
+            bot.reply('Why would you do that?!')
 
     .. versionadded:: 7.1
 
         This is now ``ctcp`` instead of ``intent``, and it can be called
         without argument, in which case it will assume ``ACTION``.
 
     .. note::
 
         This used to be ``@intent``, for a long dead feature in the IRCv3 spec.
         It is now replaced by ``@ctcp``, which can be used without arguments.
         In that case, Sopel will assume it should trigger on ``ACTION``.
 
         As ``sopel.module`` will be removed in Sopel 9, so will ``@intent``.
+
+    .. __: https://datatracker.ietf.org/doc/html/draft-oakley-irc-ctcp-02#appendix-A
     """
     default_commands = ('ACTION',) + command_list
     if function is None:
         return ctcp(*default_commands)  # called as ``@ctcp()``
     elif callable(function):
         # called as ``@ctcp`` or ``@ctcp(function)``
         # or even ``@ctcp(function, 'ACTION', ...)``
@@ -834,65 +1116,283 @@
 
     # function is not None, and it is not a callable
     # called as ``@ctcp('ACTION', ...)``
     ctcp_commands = (function,) + command_list
 
     def add_attribute(function):
         function._sopel_callable = True
-        if not hasattr(function, "intents"):
-            function.intents = []
+        if not hasattr(function, "ctcp"):
+            function.ctcp = []
         for name in ctcp_commands:
-            if name not in function.intents:
-                function.intents.append(name)
+            if name not in function.ctcp:
+                function.ctcp.append(name)
         return function
     return add_attribute
 
 
-def rate(user=0, channel=0, server=0):
+def rate(
+    user: int = 0,
+    channel: int = 0,
+    server: int = 0,
+    *,
+    message: Optional[str] = None,
+) -> Callable:
     """Decorate a function to be rate-limited.
 
-    :param int user: seconds between permitted calls of this function by the
-                     same user
-    :param int channel: seconds between permitted calls of this function in
-                        the same channel, regardless of triggering user
-    :param int server: seconds between permitted calls of this function no
-                       matter who triggered it or where
+    :param user: seconds between permitted calls of this function by the same
+                 user
+    :param channel: seconds between permitted calls of this function in the
+                    same channel, regardless of triggering user
+    :param server: seconds between permitted calls of this function no matter
+                   who triggered it or where
+    :param message: optional keyword argument; default message sent as NOTICE
+                    when a rate limit is reached
 
     How often a function can be triggered on a per-user basis, in a channel,
     or across the server (bot) can be controlled with this decorator. A value
     of ``0`` means no limit. If a function is given a rate of 20, that
     function may only be used once every 20 seconds in the scope corresponding
-    to the parameter. Users on the admin list in Sopel’s configuration are
-    exempted from rate limits.
+    to the parameter::
+
+        from sopel import plugin
+
+        @plugin.rate(10)
+            # won't trigger if used more than once per 10s by a user
+
+        @plugin.rate(10, 10)
+            # won't trigger if used more than once per 10s by a user/channel
+
+        @plugin.rate(10, 10, 2)
+            # won't trigger if used more than once per 10s by a user/channel
+            # and never more than once every 2s
+
+    If a ``message`` is provided, it will be used as the default message sent
+    as a ``NOTICE`` to the user who hit the rate limit::
+
+        @rate(10, 10, 10, message='Hit the rate limit for this function.')
+            # will send a NOTICE
+
+    The message can contain placeholders which will be filled in:
+
+    * ``nick``: the nick that hit the rate limit
+    * ``channel``: the channel in which the rate limit was hit (will be
+      ``'private-message'`` for private messages)
+    * ``sender``: the sender (nick or channel) of the message which hit
+      the rate limit
+    * ``plugin``: the name of the plugin that hit the rate limit
+    * ``label``: the label of the plugin handler that hit the rate limit
+    * ``time_left``: the time remaining before the rate limit expires, as
+      a string
+    * ``time_left_sec``: the time remaining before the rate limit expires,
+      expressed in number of seconds
+    * ``rate_limit``: the rate limit, as a string
+    * ``rate_limit_sec``: the rate limit, expressed in number of seconds
+    * ``rate_limit_type``: the type of rate limit that was hit (one of
+      ``user, group, global``)
+
+    For example::
+
+        @rate(10, 10, 2, message='Sorry {nick}, you hit the {rate_limit_type} rate limit!')
 
     Rate-limited functions that use scheduled future commands should import
     :class:`threading.Timer` instead of :mod:`sched`, or rate limiting will
     not work properly.
+
+    .. versionchanged:: 8.0
+
+        Optional keyword argument ``message`` was added in Sopel 8.
+
+    .. note::
+
+        Users on the admin list in Sopel's configuration are exempted from rate
+        limits.
+
+    .. seealso::
+
+        You can control each rate limit separately, with their own custom
+        message using :func:`rate_user`, :func:`rate_channel`, or
+        :func:`rate_global`.
+
+    """
+    def add_attribute(function):
+        if not hasattr(function, 'user_rate'):
+            function.user_rate = user
+        if not hasattr(function, 'channel_rate'):
+            function.channel_rate = channel
+        if not hasattr(function, 'global_rate'):
+            function.global_rate = server
+        function.default_rate_message = message
+        return function
+    return add_attribute
+
+
+def rate_user(
+    rate: int,
+    message: Optional[str] = None,
+) -> Callable:
+    """Decorate a function to be rate-limited for a user.
+
+    :param rate: seconds between permitted calls of this function by the same
+                 user
+    :param message: optional; message sent as NOTICE when a user hits the limit
+
+    This decorator can be used alone or with the :func:`rate` decorator, as it
+    will always take precedence::
+
+        @rate(10, 10, 10)
+        @rate_user(20, 'You hit your rate limit for this function.')
+            # user limit will be set to 20, other to 10
+            # will send a NOTICE only when a user hits their own limit
+            # as other rate limits don't have any message set
+
+    The message can contain the same placeholders supported by :func:`rate`::
+
+        @rate_user(5, 'Sorry {nick}, you hit your {rate_limit_sec}s limit!')
+
+    If you don't provide a message, the default message set by :func:`rate`
+    (if any) will be used instead.
+
+    .. versionadded:: 8.0
+
+    .. note::
+
+        Users on the admin list in Sopel's configuration are exempted from rate
+        limits.
+
+    """
+    def add_attribute(function):
+        function.user_rate = rate
+        function.user_rate_message = message
+        return function
+    return add_attribute
+
+
+def rate_channel(
+    rate: int,
+    message: Optional[str] = None,
+) -> Callable:
+    """Decorate a function to be rate-limited for a channel.
+
+    :param rate: seconds between permitted calls of this function in the same
+                 channel, regardless of triggering user
+    :param message: optional; message sent as NOTICE when a user hits the limit
+
+    This decorator can be used alone or with the :func:`rate` decorator, as it
+    will always take precedence::
+
+        @rate(10, 10, 10)
+        @rate_channel(5, 'You hit the channel rate limit for this function.')
+            # channel limit will be set to 5, other to 10
+            # will send a NOTICE only when a user hits the channel limit
+            # as other rate limits don't have any message set
+
+    If you don't provide a message, the default message set by :func:`rate`
+    (if any) will be used instead.
+
+    The message can contain the same placeholders supported by :func:`rate`::
+
+        @rate_channel(
+            5,
+            'Sorry {nick}, you hit the {rate_limit_sec}s limit for the {channel} channel!',
+        )
+
+    .. versionadded:: 8.0
+
+    .. note::
+
+        Users on the admin list in Sopel's configuration are exempted from rate
+        limits.
+
+    """
+    def add_attribute(function):
+        function.channel_rate = rate
+        function.channel_rate_message = message
+        return function
+    return add_attribute
+
+
+def rate_global(
+    rate: int,
+    message: Optional[str] = None,
+) -> Callable:
+    """Decorate a function to be rate-limited for the whole server.
+
+    :param rate: seconds between permitted calls of this function no matter who
+                 triggered it or where
+    :param message: optional; message sent as NOTICE when a user hits the limit
+
+    This decorator can be used alone or with the :func:`rate` decorator, as it
+    will always take precedence.
+
+    For example::
+
+        @rate(10, 10, 10)
+        @rate_global(5, 'You hit the global rate limit for this function.')
+            # global limit will be set to 5, other to 10
+            # will send a NOTICE only when a user hits the global limit
+            # as other rate limits don't have any message set
+
+    If you don't provide a message, the default message set by :func:`rate`
+    (if any) will be used instead.
+
+    The message can contain the same placeholders supported by :func:`rate`::
+
+        @rate_global(5, 'Sorry {nick}, you hit the 5s limit!')
+
+    .. versionadded:: 8.0
+
+    .. note::
+
+        Users on the admin list in Sopel's configuration are exempted from rate
+        limits.
+
     """
     def add_attribute(function):
-        function.rate = user
-        function.channel_rate = channel
-        function.global_rate = server
+        function.global_rate = rate
+        function.global_rate_message = message
         return function
     return add_attribute
 
 
-def require_privmsg(message=None, reply=False):
+def require_privmsg(
+    message: Union[Callable, Optional[str]] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to only be triggerable from a private message.
 
-    :param str message: optional message said if triggered in a channel
-    :param bool reply: use :meth:`~sopel.bot.Sopel.reply` instead of
-                       :meth:`~sopel.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param message: optional message said if triggered in a channel
+    :param reply: use :meth:`~sopel.bot.Sopel.reply` instead of
+                  :meth:`~sopel.bot.Sopel.say` when ``True``; defaults to
+                  ``False``
+
+    A decorated plugin callable will be triggered only by messages sent to the
+    bot in private::
+
+        from sopel import plugin
+
+        @plugin.command('.shh')
+        @plugin.require_privmsg('PM only command.')
+        def confidential_command(bot, trigger):
+            # trigger on private messages only
 
-    If the decorated function is triggered by a channel message, ``message``
+    If the decorated function is triggered by a channel message, the ``message``
     will be said if given. By default, it uses :meth:`bot.say()
-    <.bot.Sopel.say>`, but when ``reply`` is true, then it uses
+    <.bot.Sopel.say>`, but when ``reply`` is ``True``, then it uses
     :meth:`bot.reply() <.bot.Sopel.reply>` instead.
 
+    This decorator also works without parentheses, if you want its default (no
+    arguments) behavior::
+
+        from sopel import plugin
+
+        @plugin.command('.shh')
+        @plugin.require_privmsg
+        def confidential_command(bot, trigger):
+            # trigger on private messages only
+
     .. versionchanged:: 7.0
         Added the ``reply`` parameter.
     """
     def actual_decorator(function):
         @functools.wraps(function)
         def guarded(bot, trigger, *args, **kwargs):
             if trigger.is_privmsg:
@@ -907,37 +1407,49 @@
 
     # Hack to allow decorator without parens
     if callable(message):
         return actual_decorator(message)
     return actual_decorator
 
 
-def require_chanmsg(message=None, reply=False):
+def require_chanmsg(
+    message: Union[Callable, Optional[str]] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to only be triggerable from a channel message.
 
-    :param str message: optional message said if triggered in private message
-    :param bool reply: use :meth:`~.bot.Sopel.reply` instead of
-                       :meth:`~.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param message: optional message said if triggered in private message
+    :param reply: use :meth:`~.bot.Sopel.reply` instead of
+                  :meth:`~.bot.Sopel.say` when ``True``; defaults to ``False``
 
     A decorated plugin callable will be triggered only by messages from a
     channel::
 
         from sopel import plugin
 
-        @plugin.command('.mycommand')
+        @plugin.command('.mtopic')
         @plugin.require_chanmsg('Channel only command.')
         def manage_topic(bot, trigger):
             # trigger on channel messages only
 
-    If the decorated function is triggered by a private message, ``message``
+    If the decorated function is triggered by a private message, the ``message``
     will be said if given. By default, it uses :meth:`bot.say()
-    <.bot.Sopel.say>`, but when ``reply`` is true, then it uses
+    <.bot.Sopel.say>`, but when ``reply`` is ``True`` it uses
     :meth:`bot.reply() <.bot.Sopel.reply>` instead.
 
+    This decorator also works without parentheses, if you want its default (no
+    arguments) behavior::
+
+        from sopel import plugin
+
+        @plugin.command('.mtopic')
+        @plugin.require_chanmsg
+        def manage_topic(bot, trigger):
+            # trigger on channel messages only
+
     .. versionchanged:: 7.0
         Added the ``reply`` parameter.
     """
     def actual_decorator(function):
         @functools.wraps(function)
         def guarded(bot, trigger, *args, **kwargs):
             if not trigger.is_privmsg:
@@ -952,22 +1464,49 @@
 
     # Hack to allow decorator without parens
     if callable(message):
         return actual_decorator(message)
     return actual_decorator
 
 
-def require_account(message=None, reply=False):  # lgtm [py/similar-function]
+def require_account(
+    message: Union[Callable, Optional[str]] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to require services/NickServ authentication.
 
-    :param str message: optional message to say if a user without
-                        authentication tries to trigger this function
-    :param bool reply: use :meth:`~.bot.Sopel.reply` instead of
-                       :meth:`~.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param message: optional message to say if a user without authentication
+                    tries to trigger this function
+    :param reply: use :meth:`~.bot.Sopel.reply` instead of
+                  :meth:`~.bot.Sopel.say` when ``True``; defaults to ``False``
+
+    A decorated plugin callable will be triggered only if the triggering user is
+    logged into a network services account::
+
+        from sopel import plugin
+
+        @plugin.command('.regonly')
+        @plugin.require_account('Registered users only.')
+        def logged_in_command(bot, trigger):
+            # trigger only if user is logged in to services
+
+    If an unauthenticated user triggers the decorated function, the ``message``
+    will be said if given. By default, it uses :meth:`bot.say()
+    <.bot.Sopel.say>`, but when ``reply`` is ``True`` it uses :meth:`bot.reply()
+    <.bot.Sopel.reply>` instead.
+
+    This decorator also works without parentheses, if you want its default (no
+    arguments) behavior::
+
+        from sopel import plugin
+
+        @plugin.command('.regonly')
+        @plugin.require_account
+        def logged_in_command(bot, trigger):
+            # trigger only if user is logged in to services
 
     .. versionadded:: 7.0
     .. note::
 
         Only some networks support services authentication, and not all of
         those implement the standards required for clients like Sopel to
         determine authentication status. This decorator will block *all* use
@@ -998,66 +1537,96 @@
     # Hack to allow decorator without parens
     if callable(message):
         return actual_decorator(message)
 
     return actual_decorator
 
 
-def require_privilege(level, message=None, reply=False):
+def require_privilege(
+    level: AccessLevel,
+    message: Optional[str] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to require at least the given channel permission.
 
-    :param int level: required privilege level to use this command
-    :param str message: optional message said to insufficiently privileged user
-    :param bool reply: use :meth:`~.bot.Sopel.reply` instead of
-                       :meth:`~.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param level: required privilege level to use this command
+    :param message: optional message said to insufficiently privileged user
+    :param reply: use :meth:`~.bot.Sopel.reply` instead of
+                  :meth:`~.bot.Sopel.say` when ``True``; defaults to ``False``
 
     ``level`` can be one of the privilege level constants defined in this
-    module. If the user does not have the privilege, the bot will say
+    module. If the user does not have at least that privilege, the bot will say
     ``message`` if given. By default, it uses :meth:`bot.say()
-    <.bot.Sopel.say>`, but when ``reply`` is true, then it uses
-    :meth:`bot.reply() <.bot.Sopel.reply>` instead.
+    <.bot.Sopel.say>`, but when ``reply`` is ``True`` it uses :meth:`bot.reply()
+    <.bot.Sopel.reply>` instead.
 
-    Privilege requirements are ignored in private messages.
+    Use of ``require_privilege()`` implies :func:`require_chanmsg`.
 
     .. versionchanged:: 7.0
         Added the ``reply`` parameter.
+
+    .. versionchanged:: 8.0
+        Decorated callables no longer run in response to private messages.
     """
     def actual_decorator(function):
         @functools.wraps(function)
         def guarded(bot, trigger, *args, **kwargs):
-            # If this is a privmsg, ignore privilege requirements
+            # If this is a privmsg, do not trigger
             if trigger.is_privmsg:
-                return function(bot, trigger, *args, **kwargs)
+                return
             channel_privs = bot.channels[trigger.sender].privileges
             allowed = channel_privs.get(trigger.nick, 0) >= level
             if not trigger.is_privmsg and not allowed:
                 if message and not callable(message):
                     if reply:
                         bot.reply(message)
                     else:
                         bot.say(message)
             else:
                 return function(bot, trigger, *args, **kwargs)
         return guarded
     return actual_decorator
 
 
-def require_admin(message=None, reply=False):  # lgtm [py/similar-function]
+def require_admin(
+    message: Union[Callable, Optional[str]] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to require the triggering user to be a bot admin.
 
-    :param str message: optional message said to non-admin user
-    :param bool reply: use :meth:`~.bot.Sopel.reply` instead of
-                       :meth:`~.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param message: optional message said to non-admin user
+    :param reply: use :meth:`~.bot.Sopel.reply` instead of
+                  :meth:`~.bot.Sopel.say` when ``True``; defaults to ``False``
+
+    A decorated plugin callable will be triggered only if the triggering user is
+    an admin of the bot, according to its configuration::
+
+        from sopel import plugin
+
+        @plugin.command('.adminonly')
+        @plugin.require_admin('Bot admin only command.')
+        def admin_command(bot, trigger):
+            # trigger only if user is a bot admin
+
+    The bot's :attr:`~.config.core_section.CoreSection.owner` is also an admin.
 
     When the triggering user is not an admin, the command is not run, and the
-    bot will say the ``message`` if given. By default, it uses
-    :meth:`bot.say() <.bot.Sopel.say>`, but when ``reply`` is true, then it
-    uses :meth:`bot.reply() <.bot.Sopel.reply>` instead.
+    bot will say the ``message`` if given. By default, it uses :meth:`bot.say()
+    <.bot.Sopel.say>`, but when ``reply`` is ``True`` it uses :meth:`bot.reply()
+    <.bot.Sopel.reply>` instead.
+
+    This decorator also works without parentheses, if you want its default (no
+    arguments) behavior::
+
+        from sopel import plugin
+
+        @plugin.command('.adminonly')
+        @plugin.require_admin
+        def admin_command(bot, trigger):
+            # trigger only if user is a bot admin
 
     .. versionchanged:: 7.0
         Added the ``reply`` parameter.
     """
     def actual_decorator(function):
         @functools.wraps(function)
         def guarded(bot, trigger, *args, **kwargs):
@@ -1074,26 +1643,48 @@
     # Hack to allow decorator without parens
     if callable(message):
         return actual_decorator(message)
 
     return actual_decorator
 
 
-def require_owner(message=None, reply=False):  # lgtm [py/similar-function]
+def require_owner(
+    message: Union[Callable, Optional[str]] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to require the triggering user to be the bot owner.
 
-    :param str message: optional message said to non-owner user
-    :param bool reply: use :meth:`~.bot.Sopel.reply` instead of
-                       :meth:`~.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param message: optional message said to non-owner user
+    :param reply: use :meth:`~.bot.Sopel.reply` instead of
+                  :meth:`~.bot.Sopel.say` when ``True``; defaults to ``False``
+
+    A decorated plugin callable will be triggered only if the triggering user is
+    recognized as the bot's owner, according to its configuration::
+
+        from sopel import plugin
+
+        @plugin.command('.owneronly')
+        @plugin.require_owner('Bot owner only command.')
+        def owner_command(bot, trigger):
+            # trigger only if user is the bot's owner
 
     When the triggering user is not the bot's owner, the command is not run,
     and the bot will say ``message`` if given. By default, it uses
-    :meth:`bot.say() <.bot.Sopel.say>`, but when ``reply`` is true, then it
-    uses :meth:`bot.reply() <.bot.Sopel.reply>` instead.
+    :meth:`bot.say() <.bot.Sopel.say>`, but when ``reply`` is ``True`` it uses
+    :meth:`bot.reply() <.bot.Sopel.reply>` instead.
+
+    This decorator also works without parentheses, if you want its default (no
+    arguments) behavior::
+
+        from sopel import plugin
+
+        @plugin.command('.owneronly')
+        @plugin.require_owner
+        def owner_command(bot, trigger):
+            # trigger only if user is the bot's owner
 
     .. versionchanged:: 7.0
         Added the ``reply`` parameter.
     """
     def actual_decorator(function):
         @functools.wraps(function)
         def guarded(bot, trigger, *args, **kwargs):
@@ -1109,57 +1700,62 @@
 
     # Hack to allow decorator without parens
     if callable(message):
         return actual_decorator(message)
     return actual_decorator
 
 
-def require_bot_privilege(level, message=None, reply=False):
+def require_bot_privilege(
+    level: AccessLevel,
+    message: Optional[str] = None,
+    reply: bool = False,
+) -> Callable:
     """Decorate a function to require a minimum channel privilege for the bot.
 
-    :param int level: minimum channel privilege the bot needs for this function
-    :param str message: optional message said if the bot's channel privilege
-                        level is insufficient
-    :param bool reply: use :meth:`~.bot.Sopel.reply` instead of
-                       :meth:`~.bot.Sopel.say` when ``True``; defaults to
-                       ``False``
+    :param level: minimum channel privilege the bot needs for this function
+    :param message: optional message said if the bot's channel privilege level
+                    is insufficient
+    :param reply: use :meth:`~.bot.Sopel.reply` instead of
+                  :meth:`~.bot.Sopel.say` when ``True``; defaults to ``False``
 
     ``level`` can be one of the privilege level constants defined in this
     module. If the bot does not have the privilege, the bot will say
     ``message`` if given. By default, it uses :meth:`bot.say()
-    <.bot.Sopel.say>`, but when ``reply`` is true, then it uses
-    :meth:`bot.reply() <.bot.Sopel.reply>` instead.
+    <.bot.Sopel.say>`, but when ``reply`` is ``True`` it uses :meth:`bot.reply()
+    <.bot.Sopel.reply>` instead.
 
-    Privilege requirements are ignored in private messages.
+    Use of ``require_bot_privilege()`` implies :func:`require_chanmsg`.
 
     .. versionadded:: 7.1
+    .. versionchanged:: 8.0
+        Decorated callables no longer run in response to private messages.
     """
     def actual_decorator(function):
         @functools.wraps(function)
         def guarded(bot, trigger, *args, **kwargs):
-            # If this is a privmsg, ignore privilege requirements
+            # If this is a privmsg, do not trigger
             if trigger.is_privmsg:
-                return function(bot, trigger, *args, **kwargs)
+                return
 
             if not bot.has_channel_privilege(trigger.sender, level):
                 if message and not callable(message):
                     if reply:
                         bot.reply(message)
                     else:
                         bot.say(message)
             else:
                 return function(bot, trigger, *args, **kwargs)
         return guarded
     return actual_decorator
 
 
-def url(*url_rules):
+def url(*url_rules: str) -> Callable:
     """Decorate a function to handle URLs.
 
-    :param str url_rules: one or more regex pattern(s) to match URLs
+    :param url_rules: one or more regex pattern(s) to match URLs
 
     This decorator takes a regex string that will be matched against URLs in a
     message. The function it decorates is like any other callable::
 
         from sopel import plugin
 
         @plugin.url(r'https://example.com/bugs/([a-z0-9]+)')
@@ -1207,20 +1803,19 @@
             url_regex = re.compile(url_rule)
             if url_regex not in function.url_regex:
                 function.url_regex.append(url_regex)
         return function
     return actual_decorator
 
 
-def url_lazy(*loaders):
+def url_lazy(*loaders: Callable) -> Callable:
     """Decorate a function to handle URL, using lazy-loading for its regex.
 
     :param loaders: one or more functions to generate a list of **compiled**
                     regexes to match URLs.
-    :type loaders: :term:`function`
 
     Each ``loader`` function must accept a ``settings`` parameter and return a
     list (or tuple) of **compiled** regular expressions::
 
         import re
 
         def loader(settings):
@@ -1239,15 +1834,14 @@
         from sopel import plugin
 
         @plugin.url_lazy(loader)
         def my_url_handler(bot, trigger):
             bot.say('URL found: %s' % trigger.group(0))
 
     .. versionadded:: 7.1
-
     .. seealso::
 
         When more than one loader is provided, they will be chained together
         with the :func:`sopel.tools.chain_loaders` function.
 
     """
     def decorator(function):
@@ -1255,41 +1849,41 @@
         if not hasattr(function, 'url_lazy_loaders'):
             function.url_lazy_loaders = []
         function.url_lazy_loaders.extend(loaders)
         return function
     return decorator
 
 
-class example(object):
+class example:
     """Decorate a function with an example, and optionally test output.
 
-    :param str msg: the example command (required; see below)
-    :param str result: the command's expected output (optional; see below)
-    :param bool privmsg: if ``True``, the example will be tested as if it was
-                         received in a private message to the bot; otherwise,
-                         in a channel (optional; default ``False``)
-    :param bool admin: whether to treat the test message as having come from a
-                       bot admin (optional; default ``False``)
-    :param bool owner: whether to treat the test message as having come from
-                       the bot's owner (optional; default ``False``)
-    :param int repeat: how many times to repeat the test; useful for commands
-                       that return random results (optional; default ``1``)
-    :param bool re: if ``True``, the ``result`` is interpreted as a regular
-                    expression and used to match the command's output
-                    (optional; see below)
-    :param list ignore: :class:`list` of regular expression patterns to match
-                        ignored output (optional; see below)
-    :param bool user_help: whether this example should be included in
-                           user-facing help output such as `.help command`
-                           (optional; default ``False``; see below)
-    :param bool online: if ``True``, |pytest|_ will mark this example as
-                        "online" (optional; default ``False``; see below)
-    :param bool vcr: if ``True``, this example's HTTP requests & responses will
-                     be recorded for later reuse (optional; default ``False``;
-                     see below)
+    :param msg: the example command (required; see below)
+    :param result: the command's expected output (optional; see below)
+    :param privmsg: if ``True``, the example will be tested as if it was
+                    received in a private message to the bot; otherwise,
+                    in a channel (optional; default ``False``)
+    :param admin: whether to treat the test message as having come from a
+                  bot admin (optional; default ``False``)
+    :param owner: whether to treat the test message as having come from
+                  the bot's owner (optional; default ``False``)
+    :param repeat: how many times to repeat the test; useful for commands
+                   that return random results (optional; default ``1``)
+    :param re: if ``True``, the ``result`` is interpreted as a regular
+               expression and used to match the command's output
+               (optional; see below)
+    :param ignore: list of regular expression patterns to match ignored
+                   output (optional; see below)
+    :param user_help: whether this example should be included in
+                      user-facing help output such as `.help command`
+                      (optional; default ``False``; see below)
+    :param online: if ``True``, |pytest|_ will mark this example as "online"
+                   (optional; default ``False``; see below)
+    :param vcr: if ``True``, this example's HTTP requests & responses will
+                be recorded for later reuse (optional; default ``False``;
+                see below)
 
     .. |pytest| replace:: ``pytest``
     .. _pytest: https://pypi.org/project/pytest/
 
     For compatibility with the built-in help plugin, ``msg`` must use the
     default :attr:`~sopel.config.core_section.CoreSection.help_prefix` if it
     is a prefixed command. Other command types should give example invocations
@@ -1321,43 +1915,59 @@
     replaying during later test runs. It can be an alternative (or complement)
     to ``online``, and is especially useful for testing plugin code that calls
     on inconsistent or flaky remote APIs. The recorded "cassettes" of responses
     can be committed alongside the code for use by CI services, etc. (See
     `VCR.py <https://github.com/kevin1024/vcrpy>`_ & `pytest-vcr
     <https://github.com/ktosiek/pytest-vcr>`_)
     """
-    def __init__(self, msg, result=None, privmsg=False, admin=False,
-                 owner=False, repeat=1, re=False, ignore=None,
-                 user_help=False, online=False, vcr=False):
+    def __init__(
+        self,
+        msg: str,
+        result: Optional[Union[str, Iterable[str]]] = None,
+        privmsg: bool = False,
+        admin: bool = False,
+        owner: bool = False,
+        repeat: int = 1,
+        re: bool = False,
+        ignore: Optional[Union[str, Iterable[str]]] = None,
+        user_help: bool = False,
+        online: bool = False,
+        vcr: bool = False,
+    ):
         # Wrap result into a list for get_example_test
-        if isinstance(result, list):
-            self.result = result
-        elif result is not None:
+        self.result: Optional[list[str]] = None
+        if isinstance(result, str):
             self.result = [result]
-        else:
-            self.result = None
+        elif result is not None:
+            self.result = list(result)
+
         self.use_re = re
         self.msg = msg
         self.privmsg = privmsg
         self.admin = admin
         self.owner = owner
         self.repeat = repeat
         self.online = online
         self.vcr = vcr
 
-        if isinstance(ignore, list):
-            self.ignore = ignore
-        elif ignore is not None:
+        self.ignore: list[str] = []
+        if isinstance(ignore, str):
             self.ignore = [ignore]
-        else:
-            self.ignore = []
+        elif ignore is not None:
+            self.ignore = list(ignore)
 
         self.user_help = user_help
 
     def __call__(self, func):
+        # mypy (as of v1.4) doesn't recognize the below check as adding an
+        # "example" attribute to `func` if it's missing, so the `func`
+        # argument isn't typed yet.
+        # When we're ready to type-hint `loader`, we can make a TypeVar like
+        # `Callable[[SopelWrapper, Trigger], Any]` (but with the attributes
+        # the loader adds) for use in places like this.
         if not hasattr(func, "example"):
             func.example = []
 
         import sys
 
         # only inject test-related stuff if we're running tests
         # see https://stackoverflow.com/a/44595269/5991
@@ -1394,29 +2004,24 @@
             "result": self.result,
             # flags
             "is_private_message": self.privmsg,
             "is_help": self.user_help,
             "is_pattern": self.use_re,
             "is_admin": self.admin,
             "is_owner": self.owner,
-            # old-style flags
-            # TODO: to be removed in Sopel 8.0
-            "privmsg": self.privmsg,
-            "admin": self.admin,
-            "help": self.user_help,
         }
         func.example.append(record)
         return func
 
 
-def output_prefix(prefix):
+def output_prefix(prefix: str) -> Callable:
     """Decorate a function to add a prefix on its output.
 
-    :param str prefix: the prefix to add (must include trailing whitespace if
-                       desired; Sopel does not assume it should add anything)
+    :param prefix: the prefix to add (must include trailing whitespace if
+                   desired; Sopel does not assume it should add anything)
 
     Prefix will be added to text sent through:
 
     * :meth:`bot.say <sopel.bot.SopelWrapper.say>`
     * :meth:`bot.notice <sopel.bot.SopelWrapper.notice>`
 
     """
```

### Comparing `sopel-7.1.9/sopel/plugins/__init__.py` & `sopel-8.0.0/sopel/plugins/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,131 @@
-# coding=utf-8
 """Sopel's plugins interface.
 
 .. versionadded:: 7.0
 
 Sopel uses what are called Plugin Handlers as an interface between the bot and
 its plugins (formerly called "modules"). This interface is defined by the
 :class:`~.handlers.AbstractPluginHandler` abstract class.
 
 Plugins that can be used by Sopel are provided by :func:`~.get_usable_plugins`
 in an :class:`ordered dict<collections.OrderedDict>`. This dict contains one
 and only one plugin per unique name, using a specific order:
 
 * extra directories defined in the settings
 * homedir's ``plugins`` directory
-* homedir's ``modules`` directory
-* ``sopel.plugins`` setuptools entry points
+* ``sopel.plugins`` entry point group
 * ``sopel_modules``'s subpackages
-* ``sopel.modules``'s core plugins
+* ``sopel.builtins``'s core plugins
 
 (The ``coretasks`` plugin is *always* the one from ``sopel.coretasks`` and
 cannot be overridden.)
 
 To find all plugins (no matter their sources), the :func:`~.enumerate_plugins`
 function can be used. For a more fine-grained search, ``find_*`` functions
 exist for each type of plugin.
 """
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import collections
-import imp
+import importlib
 import itertools
+import logging
 import os
+from typing import TYPE_CHECKING, Union
 
-import pkg_resources
+# TODO: use stdlib importlib.metadata when possible, after dropping py3.9.
+# Stdlib does not support `entry_points(group='filter')` until py3.10, but
+# fallback logic is more trouble than it's worth when e.g. clean Ubuntu
+# py3.10 envs include old versions of this backport.
+import importlib_metadata
 
 from . import exceptions, handlers, rules  # noqa
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
 
-def _list_plugin_filenames(directory):
+
+LOGGER = logging.getLogger(__name__)
+
+
+def _list_plugin_filenames(directory: Union[str, os.PathLike]) -> Iterable[tuple[str, str]]:
     # list plugin filenames from a directory
     # yield 2-value tuples: (name, absolute path)
     base = os.path.abspath(directory)
     for filename in os.listdir(base):
-        abspath = os.path.join(base, filename)
+        abspath = os.path.realpath(os.path.join(base, filename))
+        if not os.path.exists(abspath):
+            LOGGER.warning("Plugin path does not exist, skipping: %r", abspath)
+            continue
 
         if os.path.isdir(abspath):
             if os.path.isfile(os.path.join(abspath, '__init__.py')):
                 yield os.path.basename(filename), abspath
         else:
             name, ext = os.path.splitext(filename)
             if ext == '.py' and name != '__init__':
                 yield name, abspath
 
 
 def find_internal_plugins():
     """List internal plugins.
 
     :return: yield instances of :class:`~.handlers.PyModulePlugin`
-             configured for ``sopel.modules.*``
+             configured for ``sopel.builtins.*``
 
-    Internal plugins can be found under ``sopel.modules``. This list does not
+    Internal plugins can be found under ``sopel.builtins``. This list does not
     include the ``coretasks`` plugin.
     """
-    plugin_dir = imp.find_module(
-        'modules',
-        [imp.find_module('sopel')[1]]
-    )[1]
+    builtins = importlib.util.find_spec('sopel.builtins')
+    if builtins is None or builtins.submodule_search_locations is None:
+        raise RuntimeError('Cannot resolve internal plugins')
+    plugin_list = itertools.chain.from_iterable(
+        _list_plugin_filenames(path)
+        for path in builtins.submodule_search_locations
+    )
 
-    for name, _ in _list_plugin_filenames(plugin_dir):
-        yield handlers.PyModulePlugin(name, 'sopel.modules')
+    for name, _ in set(plugin_list):
+        yield handlers.PyModulePlugin(name, 'sopel.builtins')
 
 
 def find_sopel_modules_plugins():
     """List plugins from ``sopel_modules.*``.
 
     :return: yield instances of :class:`~.handlers.PyModulePlugin`
              configured for ``sopel_modules.*``
 
     Before entry point plugins, the only way to package a plugin was to follow
     :pep:`382` by using the ``sopel_modules`` namespace. This function is
     responsible to load such plugins.
     """
     try:
-        import sopel_modules
+        import sopel_modules  # type: ignore[import]
     except ImportError:
         return
 
     for plugin_dir in set(sopel_modules.__path__):
         for name, _ in _list_plugin_filenames(plugin_dir):
             yield handlers.PyModulePlugin(name, 'sopel_modules')
 
 
 def find_entry_point_plugins(group='sopel.plugins'):
-    """List plugins from a setuptools entry point group.
+    """List plugins from an entry point group.
 
-    :param str group: setuptools entry point group to look for
-                      (defaults to ``sopel.plugins``)
+    :param str group: entry point group to search in (defaults to
+                      ``sopel.plugins``)
     :return: yield instances of :class:`~.handlers.EntryPointPlugin`
-             created from setuptools entry point given ``group``
+             created from each entry point in the ``group``
 
-    This function finds plugins declared under a setuptools entry point; by
-    default it uses the ``sopel.plugins`` entry point.
+    This function finds plugins declared under an entry point group; by
+    default it looks in the ``sopel.plugins`` group.
     """
-    for entry_point in pkg_resources.iter_entry_points(group):
+    for entry_point in importlib_metadata.entry_points(group=group):
         yield handlers.EntryPointPlugin(entry_point)
 
 
 def find_directory_plugins(directory):
     """List plugins from a ``directory``.
 
     :param str directory: directory path to search
@@ -133,41 +149,38 @@
 
     This function uses the find functions to find all of Sopel's available
     plugins. It uses the bot's ``settings`` to determine if the plugin is
     enabled or disabled.
 
     .. seealso::
 
-       The find functions used are:
+        The find functions used are:
+
+        * :func:`find_internal_plugins` for internal plugins
+        * :func:`find_sopel_modules_plugins` for ``sopel_modules.*`` plugins
+        * :func:`find_entry_point_plugins` for plugins exposed via packages'
+          entry points
+        * :func:`find_directory_plugins` for plugins in ``$homedir/plugins``,
+          and in extra directories as defined by ``settings.core.extra``
+
+    .. versionchanged:: 8.0
 
-       * :func:`find_internal_plugins` for internal plugins
-       * :func:`find_sopel_modules_plugins` for ``sopel_modules.*`` plugins
-       * :func:`find_entry_point_plugins` for plugins exposed by setuptools
-         entry points
-       * :func:`find_directory_plugins` for plugins in ``$homedir/modules``,
-         ``$homedir/plugins``, and in extra directories, as defined by
-         ``settings.core.extra``
-
-    .. versionchanged:: 7.0
-
-       Previously, plugins were called "modules", so this would load plugins
-       from the ``$homedir/modules`` directory. Now it also loads plugins
-       from the ``$homedir/plugins`` directory.
+        Looks in ``$homedir/plugins`` instead of the ``$homedir/modules``
+        directory, reflecting Sopel's shift away from calling them "modules".
 
     """
     from_internals = find_internal_plugins()
     from_sopel_modules = find_sopel_modules_plugins()
     from_entry_points = find_entry_point_plugins()
     # load from directories
     source_dirs = [
-        os.path.join(settings.homedir, 'modules'),
         os.path.join(settings.homedir, 'plugins'),
     ]
     if settings.core.extra:
-        source_dirs = source_dirs + list(settings.core.extra)
+        source_dirs = source_dirs + settings.core.extra
 
     from_directories = [
         find_directory_plugins(source_dir)
         for source_dir in source_dirs
         if os.path.isdir(source_dir)
     ]
 
@@ -201,18 +214,18 @@
     :rtype: collections.OrderedDict
 
     This function provides the plugins Sopel can use to load, enable,
     or disable, as an :class:`ordered dict<collections.OrderedDict>`. This dict
     contains one and only one plugin per unique name, using a specific order:
 
     * extra directories defined in the settings
-    * homedir's ``modules`` directory
-    * ``sopel.plugins`` setuptools entry points
+    * homedir's ``plugins`` directory
+    * ``sopel.plugins`` entry point group
     * ``sopel_modules``'s subpackages
-    * ``sopel.modules``'s core plugins
+    * ``sopel.builtins``'s core plugins
 
     (The ``coretasks`` plugin is *always* the one from ``sopel.coretasks`` and
     cannot be overridden.)
 
     .. seealso::
 
         The :func:`~.enumerate_plugins` function is used to generate a list
@@ -223,13 +236,10 @@
     # Use an OrderedDict to get one and only one plugin per name
     # based on what plugins.enumerate_plugins does, external plugins are
     # allowed to override internal plugins
     plugins_info = collections.OrderedDict(
         (plugin.name, (plugin, is_enabled))
         for plugin, is_enabled in enumerate_plugins(settings))
     # reset coretasks's position at the end of the loading queue
-    # Python 2's OrderedDict does not have a `move_to_end` method
-    # TODO: replace by plugins_info.move_to_end('coretasks') for Python 3
-    core_info = plugins_info.pop('coretasks')
-    plugins_info['coretasks'] = core_info
+    plugins_info.move_to_end('coretasks')
 
     return plugins_info
```

### Comparing `sopel-7.1.9/sopel/plugins/exceptions.py` & `sopel-8.0.0/sopel/plugins/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# coding=utf-8
 """Sopel's plugins exceptions."""
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 
 class PluginError(Exception):
     """Base class for plugin related exceptions."""
 
 
 class PluginNotRegistered(PluginError):
     """Exception raised when a plugin is not registered."""
     def __init__(self, name):
         message = 'Plugin "%s" not registered' % name
         self.plugin_name = name
-        super(PluginNotRegistered, self).__init__(message)
+        super().__init__(message)
 
 
 class PluginSettingsError(PluginError):
     """Exception raised when a plugin is not properly configured.
 
     This can be used in any place where a plugin requires a specific config,
     for example in its ``setup`` function, in any of its rules or commands,
```

### Comparing `sopel-7.1.9/sopel/plugins/handlers.py` & `sopel-8.0.0/sopel/plugins/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 """Sopel's plugin handlers.
 
 .. versionadded:: 7.0
 
 Between a plugin (or "module") and Sopel's core, Plugin Handlers are used. It
 is an interface (defined by the :class:`AbstractPluginHandler` abstract class),
 that acts as a proxy between Sopel and the plugin, making a clear separation
@@ -15,21 +14,21 @@
 * and eventually registered using :meth:`~AbstractPluginHandler.register`
 
 Each subclass of :class:`AbstractPluginHandler` must implement its methods in
 order to be used in the application.
 
 At the moment, three types of plugin are handled:
 
-* :class:`PyModulePlugin`: manage plugins that can be imported as Python
+* :class:`PyModulePlugin`: manages plugins that can be imported as Python
   module from a Python package, i.e. where ``from package import name`` works
-* :class:`PyFilePlugin`: manage plugins that are Python files on the filesystem
+* :class:`PyFilePlugin`: manages plugins that are Python files on the filesystem
   or Python directory (with an ``__init__.py`` file inside), that cannot be
   directly imported and extra steps are necessary
-* :class:`EntryPointPlugin`: manage plugins that are declared by a setuptools
-  entry point; other than that, it behaves like a :class:`PyModulePlugin`
+* :class:`EntryPointPlugin`: manages plugins that are declared by an entry
+  point; it otherwise behaves like a :class:`PyModulePlugin`
 
 All expose the same interface and thereby abstract the internal implementation
 away from the rest of the application.
 
 .. important::
 
     This is all relatively new. Its usage and documentation is for Sopel core
@@ -38,192 +37,221 @@
 
     Do **not** build your plugin based on what is here, you do **not** need to.
 
 """
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
-import imp
+import abc
 import importlib
+import importlib.util
 import inspect
 import itertools
 import os
+import sys
+from typing import Optional, TYPE_CHECKING, TypedDict
 
-from sopel import loader
+from sopel import __version__ as release, loader, plugin as plugin_decorators
 from . import exceptions
 
-try:
-    reload = importlib.reload
-except AttributeError:
-    # py2: no reload function
-    # TODO: imp is deprecated, to be removed when py2 support is dropped
-    reload = imp.reload
+
+if TYPE_CHECKING:
+    from sopel.bot import Sopel
+    from types import ModuleType
+
+
+class PluginMetaDescription(TypedDict):
+    """Meta description of a plugin, as a dictionary.
+
+    This dictionary is expected to contain specific keys:
+
+    * name: a short name for the plugin
+    * label: a descriptive label for the plugin; see
+      :meth:`~sopel.plugins.handlers.AbstractPluginHandler.get_label`
+    * type: the plugin's type
+    * source: the plugin's source
+      (filesystem path, python module/import path, etc.)
+    * version: the plugin's version string if available, otherwise ``None``
+    """
+    name: str
+    label: str
+    type: str
+    source: str
+    version: Optional[str]
 
 
-class AbstractPluginHandler(object):
+class AbstractPluginHandler(abc.ABC):
     """Base class for plugin handlers.
 
     This abstract class defines the interface Sopel uses to
     configure, load, shutdown, etc. a Sopel plugin (or "module").
 
     It is through this interface that Sopel will interact with its plugins,
-    whether internal (from ``sopel.modules``) or external (from the Python
+    whether internal (from ``sopel.builtins``) or external (from the Python
     files in a directory, to ``sopel_modules.*`` subpackages).
 
     Sopel's loader will create a "Plugin Handler" for each plugin it finds, to
     which it then delegates loading the plugin, listing its functions
     (commands, jobs, etc.), configuring it, and running any required actions
     on shutdown (either upon exiting Sopel or unloading that plugin).
     """
+
+    @abc.abstractmethod
     def load(self):
         """Load the plugin.
 
         This method must be called first, in order to setup, register, shutdown,
         or configure the plugin later.
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
     def reload(self):
         """Reload the plugin.
 
         This method can be called once the plugin is already loaded. It will
         take care of reloading the plugin from its source.
         """
-        raise NotImplementedError
 
-    def get_label(self):
+    @abc.abstractmethod
+    def get_label(self) -> str:
         """Retrieve a display label for the plugin.
 
         :return: a human readable label for display purpose
         :rtype: str
 
         This method should, at least, return ``<module_name> plugin``.
         """
-        raise NotImplementedError
 
-    def get_meta_description(self):
+    @abc.abstractmethod
+    def get_meta_description(self) -> PluginMetaDescription:
         """Retrieve a meta description for the plugin.
 
-        :return: meta description information
+        :return: Metadata about the plugin
         :rtype: :class:`dict`
 
-        The expected keys are:
+        The expected keys are detailed in :class:`PluginMetaDescription`.
+        """
+
+    @abc.abstractmethod
+    def get_version(self):
+        """Retrieve the plugin's version.
 
-        * name: a short name for the plugin
-        * label: a descriptive label for the plugin
-        * type: the plugin's type
-        * source: the plugin's source
-          (filesystem path, python import path, etc.)
+        :return: the plugin's version string
+        :rtype: str
         """
         raise NotImplementedError
 
-    def is_loaded(self):
+    @abc.abstractmethod
+    def is_loaded(self) -> bool:
         """Tell if the plugin is loaded or not.
 
         :return: ``True`` if the plugin is loaded, ``False`` otherwise
         :rtype: bool
 
         This must return ``True`` if the :meth:`load` method has been called
         with success.
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
     def setup(self, bot):
         """Run the plugin's setup action.
 
         :param bot: instance of Sopel
         :type bot: :class:`sopel.bot.Sopel`
         """
-        raise NotImplementedError
 
-    def has_setup(self):
+    @abc.abstractmethod
+    def has_setup(self) -> bool:
         """Tell if the plugin has a setup action.
 
         :return: ``True`` if the plugin has a setup, ``False`` otherwise
         :rtype: bool
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
+    def get_capability_requests(self) -> list[plugin_decorators.capability]:
+        """Retrieve the plugin's list of capability requests."""
+
+    @abc.abstractmethod
     def register(self, bot):
         """Register the plugin with the ``bot``.
 
         :param bot: instance of Sopel
         :type bot: :class:`sopel.bot.Sopel`
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
     def unregister(self, bot):
         """Unregister the plugin from the ``bot``.
 
         :param bot: instance of Sopel
         :type bot: :class:`sopel.bot.Sopel`
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
     def shutdown(self, bot):
         """Run the plugin's shutdown action.
 
         :param bot: instance of Sopel
         :type bot: :class:`sopel.bot.Sopel`
         """
-        raise NotImplementedError
 
-    def has_shutdown(self):
+    @abc.abstractmethod
+    def has_shutdown(self) -> bool:
         """Tell if the plugin has a shutdown action.
 
         :return: ``True`` if the plugin has a ``shutdown`` action, ``False``
                  otherwise
         :rtype: bool
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
     def configure(self, settings):
         """Configure Sopel's ``settings`` for this plugin.
 
         :param settings: Sopel's configuration
         :type settings: :class:`sopel.config.Config`
 
         This method will be called by Sopel's configuration wizard.
         """
-        raise NotImplementedError
 
-    def has_configure(self):
+    @abc.abstractmethod
+    def has_configure(self) -> bool:
         """Tell if the plugin has a configure action.
 
         :return: ``True`` if the plugin has a ``configure`` action, ``False``
                  otherwise
         :rtype: bool
         """
-        raise NotImplementedError
 
 
 class PyModulePlugin(AbstractPluginHandler):
     """Sopel plugin loaded from a Python module or package.
 
     A :class:`PyModulePlugin` represents a Sopel plugin that is a Python
     module (or package) that can be imported directly.
 
     This::
 
         >>> import sys
         >>> from sopel.plugins.handlers import PyModulePlugin
-        >>> plugin = PyModulePlugin('xkcd', 'sopel.modules')
+        >>> plugin = PyModulePlugin('xkcd', 'sopel.builtins')
         >>> plugin.module_name
-        'sopel.modules.xkcd'
+        'sopel.builtins.xkcd'
         >>> plugin.load()
         >>> plugin.module_name in sys.modules
         True
 
     Is the same as this::
 
         >>> import sys
-        >>> from sopel.modules import xkcd
-        >>> 'sopel.modules.xkcd' in sys.modules
+        >>> from sopel.builtins import xkcd
+        >>> 'sopel.builtins.xkcd' in sys.modules
         True
 
     """
 
     PLUGIN_TYPE = 'python-module'
     """The plugin's type.
 
@@ -237,148 +265,180 @@
         if package:
             self.module_name = self.package + '.' + self.name
         else:
             self.module_name = name
 
         self._module = None
 
+    @property
+    def module(self) -> ModuleType:
+        if self._module is None:
+            raise RuntimeError('No module for plugin %s' % self.name)
+        return self._module
+
     def get_label(self):
         """Retrieve a display label for the plugin.
 
         :return: a human readable label for display purpose
         :rtype: str
 
         By default, this is ``<name> plugin``. If the plugin's module has a
         docstring, its first line is used as the plugin's label.
         """
         default_label = '%s plugin' % self.name
-        module_doc = getattr(self._module, '__doc__', None)
 
-        if not self.is_loaded() or not module_doc:
+        if not self.is_loaded() or not hasattr(self.module, '__doc__'):
             return default_label
 
+        module_doc = self.module.__doc__ or ""
         lines = inspect.cleandoc(module_doc).splitlines()
         return default_label if not lines else lines[0]
 
-    def get_meta_description(self):
+    def get_meta_description(self) -> PluginMetaDescription:
         """Retrieve a meta description for the plugin.
 
-        :return: meta description information
+        :return: Metadata about the plugin
         :rtype: :class:`dict`
 
-        The keys are:
+        The expected keys are detailed in :class:`PluginMetaDescription`.
 
-        * name: the plugin's name
-        * label: see :meth:`~sopel.plugins.handlers.PyModulePlugin.get_label`
-        * type: see :attr:`PLUGIN_TYPE`
-        * source: the name of the plugin's module
-
-        Example::
+        This implementation uses its module's dotted import path as the
+        ``source`` value::
 
             {
                 'name': 'example',
-                'type: 'python-module',
-                'label: 'example plugin',
+                'type': 'python-module',
+                'label': 'example plugin',
                 'source': 'sopel_modules.example',
+                'version': '3.1.2',
             }
 
         """
         return {
             'label': self.get_label(),
             'type': self.PLUGIN_TYPE,
             'name': self.name,
             'source': self.module_name,
+            'version': self.get_version(),
         }
 
+    def get_version(self) -> Optional[str]:
+        """Retrieve the plugin's version.
+
+        :return: the plugin's version string
+        :rtype: Optional[str]
+        """
+        version: Optional[str] = None
+        if self.is_loaded() and hasattr(self.module, "__version__"):
+            version = str(self.module.__version__)
+        elif self.module_name.startswith("sopel."):
+            version = release
+
+        return version
+
     def load(self):
         """Load the plugin's module using :func:`importlib.import_module`.
 
         This method assumes the module is available through ``sys.path``.
         """
         self._module = importlib.import_module(self.module_name)
 
     def reload(self):
         """Reload the plugin's module using :func:`importlib.reload`.
 
         This method assumes the plugin is already loaded.
         """
-        self._module = reload(self._module)
+        self._module = importlib.reload(self.module)
 
     def is_loaded(self):
         return self._module is not None
 
     def setup(self, bot):
         if self.has_setup():
-            self._module.setup(bot)
+            self.module.setup(bot)
 
     def has_setup(self):
         """Tell if the plugin has a setup action.
 
         :return: ``True`` if the plugin has a setup, ``False`` otherwise
         :rtype: bool
 
         The plugin has a setup action if its module has a ``setup`` attribute.
         This attribute is expected to be a callable.
         """
-        return hasattr(self._module, 'setup')
+        return hasattr(self.module, 'setup')
 
-    def register(self, bot):
-        relevant_parts = loader.clean_module(self._module, bot.config)
+    def get_capability_requests(self) -> list[plugin_decorators.capability]:
+        return [
+            module_attribute
+            for module_attribute in vars(self.module).values()
+            if isinstance(module_attribute, plugin_decorators.capability)
+        ]
+
+    def register(self, bot: Sopel) -> None:
+        # capabilities are directly registered
+        for cap_request in self.get_capability_requests():
+            bot.cap_requests.register(self.name, cap_request)
+
+        # plugin callables go through ``bot.add_plugin``
+        relevant_parts = loader.clean_module(self.module, bot.config)
         for part in itertools.chain(*relevant_parts):
             # annotate all callables in relevant_parts with `plugin_name`
             # attribute to make per-channel config work; see #1839
             setattr(part, 'plugin_name', self.name)
+
+        # TODO: replace add_plugin to direct call to register_* methods
         bot.add_plugin(self, *relevant_parts)
 
     def unregister(self, bot):
-        relevant_parts = loader.clean_module(self._module, bot.config)
+        relevant_parts = loader.clean_module(self.module, bot.config)
         bot.remove_plugin(self, *relevant_parts)
 
     def shutdown(self, bot):
         if self.has_shutdown():
-            self._module.shutdown(bot)
+            self.module.shutdown(bot)
 
     def has_shutdown(self):
         """Tell if the plugin has a shutdown action.
 
         :return: ``True`` if the plugin has a ``shutdown`` action, ``False``
                  otherwise
         :rtype: bool
 
         The plugin has a shutdown action if its module has a ``shutdown``
         attribute. This attribute is expected to be a callable.
         """
-        return hasattr(self._module, 'shutdown')
+        return hasattr(self.module, 'shutdown')
 
     def configure(self, settings):
         if self.has_configure():
-            self._module.configure(settings)
+            self.module.configure(settings)
 
     def has_configure(self):
         """Tell if the plugin has a configure action.
 
         :return: ``True`` if the plugin has a ``configure`` action, ``False``
                  otherwise
         :rtype: bool
 
         The plugin has a configure action if its module has a ``configure``
         attribute. This attribute is expected to be a callable.
         """
-        return hasattr(self._module, 'configure')
+        return hasattr(self.module, 'configure')
 
 
 class PyFilePlugin(PyModulePlugin):
     """Sopel plugin loaded from the filesystem outside of the Python path.
 
     This plugin handler can be used to load a Sopel plugin from the
     filesystem, either a Python ``.py`` file or a directory containing an
     ``__init__.py`` file, and behaves like a :class:`PyModulePlugin`::
 
         >>> from sopel.plugins.handlers import PyFilePlugin
-        >>> plugin = PyFilePlugin('/home/sopel/.sopel/modules/custom.py')
+        >>> plugin = PyFilePlugin('/home/sopel/.sopel/plugins/custom.py')
         >>> plugin.load()
         >>> plugin.name
         'custom'
 
     In this example, the plugin ``custom`` is loaded from its filename despite
     not being in the Python path.
     """
@@ -398,74 +458,66 @@
         good_dir = (
             os.path.isdir(filename) and
             os.path.isfile(os.path.join(filename, '__init__.py'))
         )
 
         if good_file:
             name = os.path.basename(filename)[:-3]
-            module_type = imp.PY_SOURCE
+            spec = importlib.util.spec_from_file_location(
+                name,
+                filename,
+            )
         elif good_dir:
             name = os.path.basename(filename)
-            module_type = imp.PKG_DIRECTORY
+            spec = importlib.util.spec_from_file_location(
+                name,
+                os.path.join(filename, '__init__.py'),
+                submodule_search_locations=filename,
+            )
         else:
             raise exceptions.PluginError('Invalid Sopel plugin: %s' % filename)
 
+        if spec is None:
+            raise exceptions.PluginError('Could not determine spec for plugin: %s' % filename)
+
         self.filename = filename
         self.path = filename
-        self.module_type = module_type
+        self.module_spec = spec
 
-        super(PyFilePlugin, self).__init__(name)
+        super().__init__(name)
 
     def _load(self):
-        # The current implementation uses `imp.load_module` to perform the
-        # load action, which also reloads the module. However, `imp` is
-        # deprecated in Python 3, so that might need to be changed when the
-        # support for Python 2 is dropped.
-        #
-        # However, the solution for Python 3 is non-trivial, since the
-        # `importlib` built-in module does not have a similar function,
-        # therefore requires to dive into its public internals
-        # (``importlib.machinery`` and ``importlib.util``).
-        #
-        # All of that is doable, but represents a lot of work. As long as
-        # Python 2 is supported, we can keep it for now.
-        #
-        # TODO: switch to ``importlib`` when Python2 support is dropped.
-        if self.module_type == imp.PY_SOURCE:
-            with open(self.path) as mod:
-                description = ('.py', 'U', self.module_type)
-                mod = imp.load_module(self.name, mod, self.path, description)
-        elif self.module_type == imp.PKG_DIRECTORY:
-            description = ('', '', self.module_type)
-            mod = imp.load_module(self.name, None, self.path, description)
-        else:
-            raise TypeError('Unsupported module type')
-
-        return mod
+        module = importlib.util.module_from_spec(self.module_spec)
+        sys.modules[self.name] = module
+        if not self.module_spec.loader:
+            raise exceptions.PluginError('Could not determine loader for plugin: %s' % self.filename)
+        self.module_spec.loader.exec_module(module)
+        return module
 
-    def get_meta_description(self):
+    def get_meta_description(self) -> PluginMetaDescription:
         """Retrieve a meta description for the plugin.
 
-        :return: meta description information
+        :return: Metadata about the plugin
         :rtype: :class:`dict`
 
-        This returns the same keys as
-        :meth:`PyModulePlugin.get_meta_description`; the ``source`` key is
-        modified to contain the source file's path instead of its Python module
-        dotted path::
+        The expected keys are detailed in :class:`PluginMetaDescription`.
+
+        This implementation uses its source file's path as the ``source``
+        value::
 
             {
                 'name': 'example',
-                'type: 'python-file',
-                'label: 'example plugin',
+                'type': 'python-file',
+                'label': 'example plugin',
                 'source': '/home/username/.sopel/plugins/example.py',
+                'version': '3.1.2',
             }
 
         """
-        data = super(PyFilePlugin, self).get_meta_description()
+        data = super().get_meta_description()
         data.update({
             'source': self.path,
         })
         return data
 
     def load(self):
         self._module = self._load()
@@ -477,95 +529,123 @@
         ``reload`` function (either from `imp` or `importlib`), because the
         module might not be available through ``sys.path``.
         """
         self._module = self._load()
 
 
 class EntryPointPlugin(PyModulePlugin):
-    """Sopel plugin loaded from a ``setuptools`` entry point.
+    """Sopel plugin loaded from an entry point.
 
-    :param entry_point: a ``setuptools`` entry point object
+    :param entry_point: an entry point object
 
-    This handler loads a Sopel plugin exposed by a ``setuptools`` entry point.
-    It expects to be able to load a module object from the entry point, and to
+    This handler loads a Sopel plugin exposed by a package's entry point. It
+    expects to be able to load a module object from the entry point, and to
     work as a :class:`~.PyModulePlugin` from that module.
 
-    By default, Sopel uses the entry point ``sopel.plugins``. To use that for
-    their plugin, developers must define an entry point either in their
-    ``setup.py`` file or their ``setup.cfg`` file::
+    By default, Sopel searches within the entry point group ``sopel.plugins``.
+    To use that for their own plugins, developers must define an entry point
+    either in their ``setup.py`` file or their ``setup.cfg`` file::
 
         # in setup.py file
         setup(
             name='my_plugin',
             version='1.0',
             entry_points={
                 'sopel.plugins': [
                     'custom = my_plugin.path.to.plugin',
                 ],
             }
         )
 
     And this plugin can be loaded with::
 
-        >>> from pkg_resources import iter_entry_points
+        >>> from importlib_metadata import entry_points
         >>> from sopel.plugins.handlers import EntryPointPlugin
         >>> plugin = [
         ...     EntryPointPlugin(ep)
-        ...     for ep in iter_entry_points('sopel.plugins', 'custom')
+        ...     for ep in entry_points(group='sopel.plugins', name='custom')
         ... ][0]
         >>> plugin.load()
         >>> plugin.name
         'custom'
 
     In this example, the plugin ``custom`` is loaded from an entry point.
     Unlike the :class:`~.PyModulePlugin`, the name is not derived from the
     actual Python module, but from its entry point's name.
 
     .. seealso::
 
         Sopel uses the :func:`~sopel.plugins.find_entry_point_plugins` function
         internally to search entry points.
 
-        Entry point is a `standard feature of setuptools`__ for Python, used
-        by other applications (like ``pytest``) for their plugins.
+        Entry points are a `standard packaging mechanism`__ for Python, used by
+        other applications (such as ``pytest``) for their plugins.
+
+        The ``importlib_metadata`` backport package is used for consistency
+        across all of Sopel's supported Python versions. Its API matches that
+        of :mod:`importlib.metadata` from Python 3.10 and up; Sopel will drop
+        this external requirement when practical.
 
-        .. __: https://setuptools.readthedocs.io/en/stable/setuptools.html#dynamic-discovery-of-services-and-plugins
+        .. __: https://packaging.python.org/en/latest/specifications/entry-points/
 
     """
 
     PLUGIN_TYPE = 'setup-entrypoint'
     """The plugin's type.
 
     Metadata for the plugin; this should be considered to be a constant and
     should not be modified at runtime.
     """
 
     def __init__(self, entry_point):
         self.entry_point = entry_point
-        super(EntryPointPlugin, self).__init__(entry_point.name)
+        super().__init__(entry_point.name)
 
     def load(self):
         self._module = self.entry_point.load()
 
-    def get_meta_description(self):
+    def get_version(self) -> Optional[str]:
+        """Retrieve the plugin's version.
+
+        :return: the plugin's version string
+        :rtype: Optional[str]
+        """
+        version: Optional[str] = super().get_version()
+
+        if (
+            version is None
+            and hasattr(self.module, "__package__")
+            and self.module.__package__ is not None
+        ):
+            try:
+                version = importlib.metadata.version(self.module.__package__)
+            except ValueError:
+                # package name is probably empty-string; just give up
+                pass
+
+        return version
+
+    def get_meta_description(self) -> PluginMetaDescription:
         """Retrieve a meta description for the plugin.
 
-        :return: meta description information
+        :return: Metadata about the plugin
         :rtype: :class:`dict`
 
-        This returns the same keys as
-        :meth:`PyModulePlugin.get_meta_description`; the ``source`` key is
-        modified to contain the setuptools entry point::
+        The expected keys are detailed in :class:`PluginMetaDescription`.
+
+        This implementation uses its entry point definition as the ``source``
+        value::
 
             {
                 'name': 'example',
-                'type: 'setup-entrypoint',
-                'label: 'example plugin',
+                'type': 'setup-entrypoint',
+                'label': 'example plugin',
                 'source': 'example = my_plugin.example',
+                'version': '3.1.2',
             }
 
         """
-        data = super(EntryPointPlugin, self).get_meta_description()
+        data = super().get_meta_description()
         data.update({
-            'source': str(self.entry_point),
+            'source': self.entry_point.name + ' = ' + self.entry_point.value,
         })
         return data
```

### Comparing `sopel-7.1.9/sopel/plugins/jobs.py` & `sopel-8.0.0/sopel/plugins/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 """Sopel's plugin jobs management.
 
 .. versionadded:: 7.1
 
 .. important::
 
     This is all fresh and new. Its usage and documentation is for Sopel core
@@ -11,15 +10,15 @@
 
     Do **not** build your plugin based on what is here, you do **not** need to.
 
 """
 # Copyright 2020, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import itertools
 import logging
 
 from sopel import tools
 from sopel.tools import jobs
 
@@ -47,16 +46,17 @@
     .. important::
 
         This is an internal tool used by Sopel to manage its jobs. To register
         a job, plugin authors should use :func:`sopel.plugin.interval`.
 
     """
     def __init__(self, manager):
-        super(Scheduler, self).__init__(manager)
-        self._jobs = tools.SopelMemoryWithDefault(list)
+        super().__init__(manager)
+        # NOTE:the annotation and type-ignore here resolves conflict with the same attribute on the base class
+        self._jobs: tools.SopelMemoryWithDefault = tools.SopelMemoryWithDefault(list)  # type: ignore[assignment]
 
     def register(self, job):
         with self._mutex:
             self._jobs[job.get_plugin_name()].append(job)
         LOGGER.debug('Job registered: %s', str(job))
 
     def unregister_plugin(self, plugin_name):
```

### Comparing `sopel-7.1.9/sopel/plugins/rules.py` & `sopel-8.0.0/sopel/plugins/rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 """Sopel's plugin rules management.
 
 .. versionadded:: 7.1
 
 .. important::
 
     This is all fresh and new. Its usage and documentation is for Sopel core
@@ -11,55 +10,66 @@
 
     Do **not** build your plugin based on what is here, you do **not** need to.
 
 """
 # Copyright 2020, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
-
+from __future__ import annotations
 
+import abc
 import datetime
 import functools
 import inspect
 import itertools
 import logging
 import re
 import threading
-
+from typing import (
+    Any,
+    Optional,
+    Type,
+    TYPE_CHECKING,
+    TypeVar,
+)
+from urllib.parse import urlparse
 
 from sopel import tools
 from sopel.config.core_section import (
     COMMAND_DEFAULT_HELP_PREFIX, COMMAND_DEFAULT_PREFIX, URL_DEFAULT_SCHEMES)
 
-
-try:
-    from urllib.parse import urlparse
-except ImportError:
-    # TODO: remove when dropping Python 2.7
-    from urlparse import urlparse
-
-try:
-    from inspect import getfullargspec as inspect_getargspec
-except ImportError:
-    # TODO: remove when dropping Python 2.7
-    from inspect import getargspec as inspect_getargspec
+if TYPE_CHECKING:
+    from collections.abc import Generator, Iterable
+    from sopel.tools.identifiers import Identifier
 
 
 __all__ = [
     'Manager',
     'Rule',
     'FindRule',
     'SearchRule',
     'Command',
     'NickCommand',
     'ActionCommand',
     'URLCallback',
 ]
 
+TypedRule = TypeVar('TypedRule', bound='AbstractRule')
+"""A :class:`~typing.TypeVar` bound to :class:`AbstractRule`.
+
+When used in the :meth:`AbstractRule.from_callable` class method, it means the
+return value must be an instance of the class used to call that method and not
+a different subclass of ``AbstractRule``.
+
+.. versionadded:: 8.0
+
+    This ``TypeVar`` was added as part of a goal to start type-checking
+    Sopel and is not used at runtime.
+
+"""
 
 LOGGER = logging.getLogger(__name__)
 
 IGNORE_RATE_LIMIT = 1  # equivalent to sopel.plugin.NOLIMIT
 """Return value used to indicate that rate-limiting should be ignored."""
 PRIORITY_HIGH = 'high'
 """Highest rule priority."""
@@ -85,18 +95,15 @@
             yield pattern
         else:
             yield _compile_pattern(pattern, nick, aliases)
 
 
 def _compile_pattern(pattern, nick, aliases=None):
     if aliases:
-        nicks = list(aliases)  # alias_nicks.copy() doesn't work in py2
-        nicks.append(nick)
-        nicks = map(re.escape, nicks)
-        nick = '(?:%s)' % '|'.join(nicks)
+        nick = '(?:%s)' % '|'.join(re.escape(n) for n in (nick, *aliases))
     else:
         nick = re.escape(nick)
 
     pattern = pattern.replace('$nickname', nick)
     pattern = pattern.replace('$nick ', r'{}[,:]\s*'.format(nick))  # @rule('$nick hi')
     pattern = pattern.replace('$nick', r'{}[,:]\s+'.format(nick))  # @rule('$nickhi')
     flags = re.IGNORECASE
@@ -150,15 +157,15 @@
             for key, value in example.items()
             if key in valid_keys
         )
         for example in examples
     )
 
 
-class Manager(object):
+class Manager:
     """Manager of plugin rules.
 
     This manager stores plugin rules and can then provide the matching rules
     for a given trigger.
 
     To register a rule:
 
@@ -452,35 +459,93 @@
         return any(
             any(rule.parse(url))
             for plugin_rules in self._url_callbacks.values()
             for rule in plugin_rules
         )
 
 
-class AbstractRule(object):
+class RuleMetrics:
+    """Tracker of a rule's usage."""
+    def __init__(self) -> None:
+        self.started_at: Optional[datetime.datetime] = None
+        self.ended_at: Optional[datetime.datetime] = None
+        self.last_return_value: Any = None
+
+    def start(self) -> None:
+        """Record a starting time (before execution)."""
+        self.started_at = datetime.datetime.now(datetime.timezone.utc)
+
+    def end(self) -> None:
+        """Record a ending time (after execution)."""
+        self.ended_at = datetime.datetime.now(datetime.timezone.utc)
+
+    def set_return_value(self, value: Any) -> None:
+        """Set the last return value of a rule."""
+        self.last_return_value = value
+
+    @property
+    def last_time(self) -> Optional[datetime.datetime]:
+        """Last recorded start/end time for the associated rule."""
+        # detect if we just started something or if it ended
+        if (self.started_at and self.ended_at) and (self.started_at < self.ended_at):
+            return self.ended_at
+
+        return self.started_at
+
+    def is_limited(
+        self,
+        time_limit: datetime.datetime,
+    ) -> bool:
+        """Determine if the rule hits the time limit."""
+        if not self.started_at:
+            # not even started, so not limited
+            return False
+
+        if self.ended_at and self.started_at < self.ended_at:
+            # since it ended, check the return value
+            if self.last_return_value == IGNORE_RATE_LIMIT:
+                return False
+
+        return self.last_time > time_limit if self.last_time else False
+
+    def __enter__(self) -> RuleMetrics:
+        self.start()
+        return self
+
+    def __exit__(
+        self,
+        type: Optional[Any],
+        value: Optional[Any],
+        traceback: Optional[Any],
+    ) -> None:
+        self.end()
+
+
+class AbstractRule(abc.ABC):
     """Abstract definition of a plugin's rule.
 
     Any rule class must be an implementation of this abstract class, as it
     defines the Rule interface:
 
     * plugin name
     * priority
     * label
     * doc, usages, and tests
     * output prefix
-    * matching patterns, events, and intents
+    * matching patterns, events, and CTCP commands
     * allow echo-message
     * threaded execution or not
     * rate limiting feature
     * text parsing
     * and finally, trigger execution (i.e. actually doing something)
 
     """
     @classmethod
-    def from_callable(cls, settings, handler):
+    @abc.abstractmethod
+    def from_callable(cls: Type[TypedRule], settings, handler) -> TypedRule:
         """Instantiate a rule object from ``settings`` and ``handler``.
 
         :param settings: Sopel's settings
         :type settings: :class:`sopel.config.Config`
         :param callable handler: a function-based rule handler
         :return: an instance of this class created from the ``handler``
         :rtype: :class:`AbstractRule`
@@ -491,15 +556,14 @@
         to load these functions as rule objects, this class method can be used;
         it takes the bot's ``settings`` and a cleaned ``handler``.
 
         A "cleaned handler" is a function, decorated appropriately, and passed
         through the filter of the
         :func:`loader's clean<sopel.loader.clean_callable>` function.
         """
-        raise NotImplementedError
 
     @property
     def priority_scale(self):
         """Rule's priority on a numeric scale.
 
         This attribute can be used to sort rules between each other, the
         highest priority rules coming first. The default priority for a rule
@@ -508,48 +572,49 @@
         priority_key = self.get_priority()
 
         return (
             PRIORITY_SCALES.get(priority_key) or
             PRIORITY_SCALES[PRIORITY_MEDIUM]
         )
 
-    def get_plugin_name(self):
+    @abc.abstractmethod
+    def get_plugin_name(self) -> str:
         """Get the rule's plugin name.
 
         :rtype: str
 
         The rule's plugin name will be used in various places to select,
         register, unregister, and manipulate the rule based on its plugin,
         which is referenced by its name.
         """
-        raise NotImplementedError
 
-    def get_rule_label(self):
+    @abc.abstractmethod
+    def get_rule_label(self) -> str:
         """Get the rule's label.
 
         :rtype: str
 
         A rule can have a label, which can identify the rule by string, the
         same way a plugin can be identified by its name. This label can be used
         to select, register, unregister, and manipulate the rule based on its
         own label. Note that the label has no effect on the rule's execution.
         """
-        raise NotImplementedError
 
-    def get_usages(self):
+    @abc.abstractmethod
+    def get_usages(self) -> tuple:
         """Get the rule's usage examples.
 
         :rtype: tuple
 
         A rule can have usage examples, i.e. a list of examples showing how
         the rule can be used, or in what context it can be triggered.
         """
-        raise NotImplementedError
 
-    def get_test_parameters(self):
+    @abc.abstractmethod
+    def get_test_parameters(self) -> tuple:
         """Get parameters for automated tests.
 
         :rtype: tuple
 
         A rule can have automated tests attached to it, and this method must
         return the test parameters:
 
@@ -559,28 +624,28 @@
         * if the results should be used as regex pattern
 
         .. seealso::
 
             :meth:`sopel.plugin.example` for more about test parameters.
 
         """
-        raise NotImplementedError
 
-    def get_doc(self):
+    @abc.abstractmethod
+    def get_doc(self) -> str:
         """Get the rule's documentation.
 
         :rtype: str
 
         A rule's documentation is a short text that can be displayed to a user
         on IRC upon asking for help about this rule. The equivalent of Python
         docstrings, but for IRC rules.
         """
-        raise NotImplementedError
 
-    def get_priority(self):
+    @abc.abstractmethod
+    def get_priority(self) -> str:
         """Get the rule's priority.
 
         :rtype: str
 
         A rule can have a priority, based on the three pre-defined priorities
         used by Sopel: ``PRIORITY_HIGH``, ``PRIORITY_MEDIUM``, and
         ``PRIORITY_LOW``.
@@ -588,132 +653,223 @@
         .. seealso::
 
             The :attr:`AbstractRule.priority_scale` property uses this method
             to look up the numeric priority value, which is used to sort rules
             by priority.
 
         """
-        raise NotImplementedError
 
-    def get_output_prefix(self):
+    @abc.abstractmethod
+    def get_output_prefix(self) -> str:
         """Get the rule's output prefix.
 
         :rtype: str
 
         .. seealso::
 
             See the :class:`sopel.bot.SopelWrapper` class for more information
             on how the output prefix can be used.
         """
-        raise NotImplementedError
 
-    def match(self, bot, pretrigger):
+    @abc.abstractmethod
+    def match(self, bot, pretrigger) -> Iterable:
         """Match a pretrigger according to the rule.
 
         :param bot: Sopel instance
         :type bot: :class:`sopel.bot.Sopel`
         :param pretrigger: line to match
         :type pretrigger: :class:`sopel.trigger.PreTrigger`
 
         This method must return a list of `match objects`__.
 
-        .. __: https://docs.python.org/3.6/library/re.html#match-objects
+        .. __: https://docs.python.org/3.11/library/re.html#match-objects
         """
-        raise NotImplementedError
 
-    def match_event(self, event):
+    @abc.abstractmethod
+    def match_event(self, event) -> bool:
         """Tell if the rule matches this ``event``.
 
         :param str event: potential matching event
         :return: ``True`` when ``event`` matches the rule, ``False`` otherwise
         :rtype: bool
         """
-        raise NotImplementedError
 
-    def match_intent(self, intent):
-        """Tell if the rule matches this ``intent``.
+    @abc.abstractmethod
+    def match_ctcp(self, command: Optional[str]) -> bool:
+        """Tell if the rule matches this CTCP ``command``.
 
-        :param str intent: potential matching intent
-        :return: ``True`` when ``intent`` matches the rule, ``False`` otherwise
-        :rtype: bool
+        :param command: potential matching CTCP command
+        :return: ``True`` when ``command`` matches the rule,
+                 ``False`` otherwise
         """
-        raise NotImplementedError
 
-    def allow_echo(self):
+    @abc.abstractmethod
+    def allow_bots(self) -> bool:
+        """Tell if the rule should match bot commands.
+
+        :return: ``True`` when the rule allows bot commands,
+                 ``False`` otherwise
+
+        A "bot command" is any IRC protocol command or numeric that has been
+        tagged as ``bot`` (or ``draft/bot``) by the IRC server.
+
+        .. seealso::
+
+            The `IRCv3 Bot Mode specification`__.
+
+        .. __: https://ircv3.net/specs/extensions/bot-mode
+        """
+
+    @abc.abstractmethod
+    def allow_echo(self) -> bool:
         """Tell if the rule should match echo messages.
 
         :return: ``True`` when the rule allows echo messages,
                  ``False`` otherwise
         :rtype: bool
         """
-        raise NotImplementedError
 
-    def is_threaded(self):
+    @abc.abstractmethod
+    def is_threaded(self) -> bool:
         """Tell if the rule's execution should be in a thread.
 
         :return: ``True`` if the execution should be in a thread,
                  ``False`` otherwise
         :rtype: bool
         """
-        raise NotImplementedError
 
-    def is_unblockable(self):
+    @abc.abstractmethod
+    def is_unblockable(self) -> bool:
         """Tell if the rule is unblockable.
 
         :return: ``True`` when the rule is unblockable, ``False`` otherwise
-        :rtype: bool
         """
-        raise NotImplementedError
 
-    def is_rate_limited(self, nick):
+    @abc.abstractmethod
+    def get_user_metrics(self, nick: Identifier) -> RuleMetrics:
+        """Get the rule's usage metrics for the given user."""
+
+    @abc.abstractmethod
+    def get_channel_metrics(self, channel: Identifier) -> RuleMetrics:
+        """Get the rule's usage metrics for the given channel."""
+
+    @abc.abstractmethod
+    def get_global_metrics(self) -> RuleMetrics:
+        """Get the rule's global usage metrics."""
+
+    @property
+    @abc.abstractmethod
+    def user_rate_limit(self) -> datetime.timedelta:
+        """The rule's user rate limit."""
+
+    @property
+    @abc.abstractmethod
+    def channel_rate_limit(self) -> datetime.timedelta:
+        """The rule's channel rate limit."""
+
+    @property
+    @abc.abstractmethod
+    def global_rate_limit(self) -> datetime.timedelta:
+        """The rule's global rate limit."""
+
+    @abc.abstractmethod
+    def is_user_rate_limited(
+        self,
+        nick: Identifier,
+        at_time: Optional[datetime.datetime] = None,
+    ) -> bool:
         """Tell when the rule reached the ``nick``'s rate limit.
 
-        :return: ``True`` when the rule reached the limit, ``False`` otherwise
-        :rtype: bool
+        :param nick: the nick associated with this check
+        :param at_time: optional aware datetime for the rate limit check;
+                        if not given, ``utcnow`` will be used
+        :return: ``True`` when the rule reached the limit, ``False`` otherwise.
         """
-        raise NotImplementedError
 
-    def is_channel_rate_limited(self, channel):
+    @abc.abstractmethod
+    def is_channel_rate_limited(
+        self,
+        channel: Identifier,
+        at_time: Optional[datetime.datetime] = None,
+    ) -> bool:
         """Tell when the rule reached the ``channel``'s rate limit.
 
-        :return: ``True`` when the rule reached the limit, ``False`` otherwise
-        :rtype: bool
+        :param channel: the channel associated with this check
+        :param at_time: optional aware datetime for the rate limit check;
+                        if not given, ``utcnow`` will be used
+        :return: ``True`` when the rule reached the limit, ``False`` otherwise.
+        """
+
+    @abc.abstractmethod
+    def is_global_rate_limited(
+        self,
+        at_time: Optional[datetime.datetime] = None,
+    ) -> bool:
+        """Tell when the rule reached the global rate limit.
+
+        :param at_time: optional aware datetime for the rate limit check;
+                        if not given, ``utcnow`` will be used
+        :return: ``True`` when the rule reached the limit, ``False`` otherwise.
         """
-        raise NotImplementedError
 
-    def is_global_rate_limited(self):
-        """Tell when the rule reached the server's rate limit.
+    @property
+    @abc.abstractmethod
+    def user_rate_template(self) -> Optional[str]:
+        """Give the message template to send with a NOTICE to ``nick``.
 
-        :return: ``True`` when the rule reached the limit, ``False`` otherwise
-        :rtype: bool
+        :return: A formatted string, or ``None`` if no message is set.
+
+        This property is accessed by the bot when a trigger hits the user rate
+        limit (i.e. for the specificed ``nick``).
         """
-        raise NotImplementedError
 
-    def parse(self, text):
+    @property
+    @abc.abstractmethod
+    def channel_rate_template(self) -> Optional[str]:
+        """Give the message template to send with a NOTICE to ``nick``.
+
+        :return: A formatted string, or ``None`` if no message is set.
+
+        This method is called by the bot when a trigger hits the channel rate
+        limit (i.e. for the specified ``channel``).
+        """
+
+    @property
+    @abc.abstractmethod
+    def global_rate_template(self) -> Optional[str]:
+        """Give the message to send with a NOTICE to ``nick``.
+
+        :return: A formatted string, or ``None`` if no message is set.
+
+        This method is called by the bot when a trigger hits the global rate
+        limit (i.e. for any nick/channel).
+        """
+
+    @abc.abstractmethod
+    def parse(self, text) -> Generator:
         """Parse ``text`` and yield matches.
 
         :param str text: text to parse by the rule
         :return: yield a list of match object
         :rtype: generator of `re.match`__
 
-        .. __: https://docs.python.org/3.6/library/re.html#match-objects
+        .. __: https://docs.python.org/3.11/library/re.html#match-objects
         """
-        raise NotImplementedError
 
+    @abc.abstractmethod
     def execute(self, bot, trigger):
         """Execute the triggered rule.
 
         :param bot: Sopel wrapper
         :type bot: :class:`sopel.bot.SopelWrapper`
         :param trigger: IRC line
         :type trigger: :class:`sopel.trigger.Trigger`
 
         This is the method called by the bot when a rule matches a ``trigger``.
         """
-        raise NotImplementedError
 
 
 class Rule(AbstractRule):
     """Generic rule definition.
 
     A generic rule (or simply "a rule") uses regular expressions to match
     at most once per IRC line per regular expression, i.e. you can trigger
@@ -764,22 +920,31 @@
         tests = tuple(example for example in examples if example.get('result'))
 
         return {
             'plugin': getattr(handler, 'plugin_name', None),
             'label': getattr(handler, 'rule_label', None),
             'priority': getattr(handler, 'priority', PRIORITY_MEDIUM),
             'events': getattr(handler, 'event', []),
-            'intents': getattr(handler, 'intents', []),
+            'ctcp': getattr(handler, 'ctcp', []),
+            'allow_bots': getattr(handler, 'allow_bots', False),
             'allow_echo': getattr(handler, 'echo', False),
             'threaded': getattr(handler, 'thread', True),
             'output_prefix': getattr(handler, 'output_prefix', ''),
             'unblockable': getattr(handler, 'unblockable', False),
-            'rate_limit': getattr(handler, 'rate', 0),
+            'user_rate_limit': getattr(handler, 'user_rate', 0),
             'channel_rate_limit': getattr(handler, 'channel_rate', 0),
             'global_rate_limit': getattr(handler, 'global_rate', 0),
+            'user_rate_message': getattr(
+                handler, 'user_rate_message', None),
+            'channel_rate_message': getattr(
+                handler, 'channel_rate_message', None),
+            'global_rate_message': getattr(
+                handler, 'global_rate_message', None),
+            'default_rate_message': getattr(
+                handler, 'default_rate_message', None),
             'usages': usages or tuple(),
             'tests': tests,
             'doc': inspect.getdoc(handler),
         }
 
     @classmethod
     def regex_from_callable(cls, settings, handler):
@@ -853,51 +1018,61 @@
     def __init__(self,
                  regexes,
                  plugin=None,
                  label=None,
                  priority=PRIORITY_MEDIUM,
                  handler=None,
                  events=None,
-                 intents=None,
+                 ctcp=None,
+                 allow_bots=False,
                  allow_echo=False,
                  threaded=True,
                  output_prefix=None,
                  unblockable=False,
-                 rate_limit=0,
+                 user_rate_limit=0,
                  channel_rate_limit=0,
                  global_rate_limit=0,
+                 user_rate_message=None,
+                 channel_rate_message=None,
+                 global_rate_message=None,
+                 default_rate_message=None,
                  usages=None,
                  tests=None,
                  doc=None):
         # core
         self._regexes = regexes
         self._plugin_name = plugin
         self._label = label
         self._priority = priority or PRIORITY_MEDIUM
         self._handler = handler
 
         # filters
         self._events = events or ['PRIVMSG']
-        self._intents = intents or []
+        self._ctcp = ctcp or []
+        self._allow_bots = bool(allow_bots)
         self._allow_echo = bool(allow_echo)
 
         # execution
         self._threaded = bool(threaded)
         self._output_prefix = output_prefix or ''
 
         # rate limiting
         self._unblockable = bool(unblockable)
-        self._rate_limit = rate_limit
+        self._user_rate_limit = user_rate_limit
         self._channel_rate_limit = channel_rate_limit
         self._global_rate_limit = global_rate_limit
+        self._user_rate_message = user_rate_message
+        self._channel_rate_message = channel_rate_message
+        self._global_rate_message = global_rate_message
+        self._default_rate_message = default_rate_message
 
         # metrics
-        self._metrics_nick = {}
-        self._metrics_sender = {}
-        self._metrics_global = None
+        self._metrics_nick: dict[Identifier, RuleMetrics] = {}
+        self._metrics_sender: dict[Identifier, RuleMetrics] = {}
+        self._metrics_global = RuleMetrics()
 
         # docs & tests
         self._usages = usages or tuple()
         self._tests = tests or tuple()
         self._doc = doc or ''
 
     def __str__(self):
@@ -966,119 +1141,163 @@
             return []
 
         # parse text
         return self.parse(text)
 
     def match_preconditions(self, bot, pretrigger):
         event = pretrigger.event
-        intent = pretrigger.tags.get('intent')
+        ctcp_command = pretrigger.ctcp
         nick = pretrigger.nick
+        is_bot_message = (
+            'bot' in pretrigger.tags and
+            event in ["PRIVMSG", "NOTICE"]
+        )
         is_echo_message = (
             nick.lower() == bot.nick.lower() and
             event in ["PRIVMSG", "NOTICE"]
         )
 
         return (
             self.match_event(event) and
-            self.match_intent(intent) and
-            (not is_echo_message or self.allow_echo())
+            self.match_ctcp(ctcp_command) and
+            (
+                (not is_bot_message or self.allow_bots()) or
+                (is_echo_message and self.allow_echo())
+            ) and (not is_echo_message or self.allow_echo())
         )
 
     def parse(self, text):
         for regex in self._regexes:
             result = regex.match(text)
             if result:
                 yield result
 
-    def match_event(self, event):
+    def match_event(self, event) -> bool:
         return bool(event and event in self._events)
 
-    def match_intent(self, intent):
-        if not self._intents:
+    def match_ctcp(self, command: Optional[str]) -> bool:
+        if not self._ctcp:
             return True
 
-        return bool(intent and any(
-            regex.match(intent)
-            for regex in self._intents
+        return bool(command and any(
+            regex.match(command)
+            for regex in self._ctcp
         ))
 
+    def allow_bots(self):
+        return self._allow_bots
+
     def allow_echo(self):
         return self._allow_echo
 
     def is_threaded(self):
         return self._threaded
 
     def is_unblockable(self):
         return self._unblockable
 
-    def is_rate_limited(self, nick):
-        metrics = self._metrics_nick.get(nick)
-        if metrics is None:
-            return False
-        last_usage_at, exit_code = metrics
+    def get_user_metrics(self, nick: Identifier) -> RuleMetrics:
+        return self._metrics_nick.get(nick, RuleMetrics())
 
-        if exit_code == IGNORE_RATE_LIMIT:
-            return False
+    def get_channel_metrics(self, channel: Identifier) -> RuleMetrics:
+        return self._metrics_sender.get(channel, RuleMetrics())
 
-        now = datetime.datetime.utcnow()
-        rate_limit = datetime.timedelta(seconds=self._rate_limit)
-        return (now - last_usage_at) <= rate_limit
-
-    def is_channel_rate_limited(self, channel):
-        metrics = self._metrics_sender.get(channel)
-        if metrics is None:
-            return False
-        last_usage_at, exit_code = metrics
+    def get_global_metrics(self) -> RuleMetrics:
+        return self._metrics_global
 
-        if exit_code == IGNORE_RATE_LIMIT:
-            return False
+    @property
+    def user_rate_limit(self) -> datetime.timedelta:
+        return datetime.timedelta(seconds=self._user_rate_limit)
 
-        now = datetime.datetime.utcnow()
-        rate_limit = datetime.timedelta(seconds=self._channel_rate_limit)
-        return (now - last_usage_at) <= rate_limit
-
-    def is_global_rate_limited(self):
-        metrics = self._metrics_global
-        if metrics is None:
-            return False
-        last_usage_at, exit_code = metrics
+    @property
+    def channel_rate_limit(self) -> datetime.timedelta:
+        return datetime.timedelta(seconds=self._channel_rate_limit)
 
-        if exit_code == IGNORE_RATE_LIMIT:
-            return False
+    @property
+    def global_rate_limit(self) -> datetime.timedelta:
+        return datetime.timedelta(seconds=self._global_rate_limit)
 
-        now = datetime.datetime.utcnow()
-        rate_limit = datetime.timedelta(seconds=self._global_rate_limit)
-        return (now - last_usage_at) <= rate_limit
+    def is_user_rate_limited(
+        self,
+        nick: Identifier,
+        at_time: Optional[datetime.datetime] = None,
+    ) -> bool:
+        if at_time is None:
+            at_time = datetime.datetime.now(datetime.timezone.utc)
+        metrics = self.get_user_metrics(nick)
+        return metrics.is_limited(at_time - self.user_rate_limit)
+
+    def is_channel_rate_limited(
+        self,
+        channel: Identifier,
+        at_time: Optional[datetime.datetime] = None,
+    ) -> bool:
+        if at_time is None:
+            at_time = datetime.datetime.now(datetime.timezone.utc)
+        metrics = self.get_channel_metrics(channel)
+        return metrics.is_limited(at_time - self.channel_rate_limit)
+
+    def is_global_rate_limited(
+        self,
+        at_time: Optional[datetime.datetime] = None,
+    ) -> bool:
+        if at_time is None:
+            at_time = datetime.datetime.now(datetime.timezone.utc)
+        metrics = self.get_global_metrics()
+        return metrics.is_limited(at_time - self.global_rate_limit)
+
+    @property
+    def user_rate_template(self) -> Optional[str]:
+        template = self._user_rate_message or self._default_rate_message
+        return template
+
+    @property
+    def channel_rate_template(self) -> Optional[str]:
+        template = self._channel_rate_message or self._default_rate_message
+        return template
+
+    @property
+    def global_rate_template(self) -> Optional[str]:
+        template = self._global_rate_message or self._default_rate_message
+        return template
 
     def execute(self, bot, trigger):
         if not self._handler:
             raise RuntimeError('Improperly configured rule: no handler')
 
-        # execute the handler
-        exit_code = self._handler(bot, trigger)
+        user_metrics: RuleMetrics = self._metrics_nick.setdefault(
+            trigger.nick, RuleMetrics())
+        sender_metrics: RuleMetrics = self._metrics_sender.setdefault(
+            trigger.sender, RuleMetrics())
 
-        # register metrics
-        now = datetime.datetime.utcnow()
-        self._metrics_nick[trigger.nick] = (now, exit_code)
-        self._metrics_sender[trigger.sender] = (now, exit_code)
-        self._metrics_global = (now, exit_code)
+        # execute the handler
+        with user_metrics, sender_metrics, self._metrics_global:
+            exit_code = self._handler(bot, trigger)
+            user_metrics.set_return_value(exit_code)
+            sender_metrics.set_return_value(exit_code)
+            self._metrics_global.set_return_value(exit_code)
 
         # return exit code
         return exit_code
 
 
-class NamedRuleMixin(object):
-    """Mixin for named rules.
+class AbstractNamedRule(Rule):
+    """Abstract base class for named rules.
 
     A named rule is invoked by using a specific word, and is usually known
     as a "command". For example, the command "hello" is triggered by using
     the word "hello" with some sort of prefix or context.
 
     A named rule can be invoked by using one of its aliases, also.
     """
+    def __init__(self, name, aliases=None, **kwargs):
+        super().__init__([], **kwargs)
+        self._name = name
+        self._aliases = tuple(aliases) if aliases is not None else tuple()
+
     @property
     def name(self):
         return self._name
 
     @property
     def aliases(self):
         return self._aliases
@@ -1097,51 +1316,23 @@
 
         :param str name: potential alias name
         :return: ``True`` when ``name`` is an alias, ``False`` otherwise
         :rtype: bool
         """
         return name in self._aliases
 
-    def escape_name(self, name):
-        """Escape the provided name if needed.
-
-        .. note::
-
-            Until now, Sopel has allowed command name to be regex pattern.
-            It was mentioned in the documentation without much details, and
-            there were no tests for it.
-
-            In order to ensure backward compatibility with previous versions of
-            Sopel, we make sure to escape command name only when it's needed.
-
-            **It is not recommended to use a regex pattern for your command
-            name. This feature will be removed in Sopel 8.0.**
+    @abc.abstractmethod
+    def get_rule_regex(self):
+        """Make the rule regex for this named rule.
 
+        :return: a compiled regex for this named rule and its aliases
         """
-        if set('.^$*+?{}[]\\|()') & set(name):
-            # the name contains a regex pattern special character
-            # we assume the user knows what they are doing
-            try:
-                # make sure it compiles properly
-                # (nobody knows what they are doing)
-                re.compile(name)
-            except re.error as error:
-                original_name = name
-                name = re.escape(name)
-                LOGGER.warning(
-                    'Command name "%s" is an invalid regular expression '
-                    'and will be replaced by "%s": %s',
-                    original_name, name, error)
-        else:
-            name = re.escape(name)
 
-        return name
 
-
-class Command(NamedRuleMixin, Rule):
+class Command(AbstractNamedRule):
     """Command rule definition.
 
     A command rule (or simply "a command") is a named rule, i.e. it has a known
     name and must be invoked using that name (or one of its aliases, if any).
     Apart from that, it behaves exactly like a :class:`generic rule <Rule>`.
 
     Here is an example with the ``dummy`` command:
@@ -1195,19 +1386,17 @@
 
     def __init__(self,
                  name,
                  prefix=COMMAND_DEFAULT_PREFIX,
                  help_prefix=COMMAND_DEFAULT_HELP_PREFIX,
                  aliases=None,
                  **kwargs):
-        super(Command, self).__init__([], **kwargs)
-        self._name = name
+        super().__init__(name, aliases=aliases, **kwargs)
         self._prefix = prefix
         self._help_prefix = help_prefix
-        self._aliases = tuple(aliases) if aliases is not None else tuple()
         self._regexes = (self.get_rule_regex(),)
 
     def __str__(self):
         label = self.get_rule_label()
         plugin = self.get_plugin_name() or '(no-plugin)'
         aliases = '|'.join(self._aliases)
 
@@ -1246,27 +1435,27 @@
 
         * the prefix regular expression,
         * the rule's name (escaped for regex if needed),
         * all of its aliases (escaped for regex if needed),
 
         to create a compiled regex to return.
         """
-        name = [self.escape_name(self._name)]
-        aliases = [self.escape_name(alias) for alias in self._aliases]
+        name = [re.escape(self._name)]
+        aliases = [re.escape(alias) for alias in self._aliases]
         pattern = r'|'.join(name + aliases)
 
         # Escape all whitespace with a single backslash.
         # This ensures that regexp in the prefix is treated as it was before
         # the actual regexp was changed to use the verbose syntax.
         prefix = re.sub(r"(\s)", r"\\\1", self._prefix)
         pattern = self.PATTERN_TEMPLATE.format(prefix=prefix, command=pattern)
         return re.compile(pattern, re.IGNORECASE | re.VERBOSE)
 
 
-class NickCommand(NamedRuleMixin, Rule):
+class NickCommand(AbstractNamedRule):
     """Nickname Command rule definition.
 
     A nickname command rule is a named rule with a twist: instead of a prefix,
     the rule is triggered when the line starts with a registered nickname (or
     one of its aliases). The command's name itself can have aliases too.
 
     Here is an example with the ``dummy`` nickname command:
@@ -1318,21 +1507,19 @@
             'aliases': aliases,
             'handler': handler,
         })
 
         return cls(**kwargs)
 
     def __init__(self, nick, name, nick_aliases=None, aliases=None, **kwargs):
-        super(NickCommand, self).__init__([], **kwargs)
+        super().__init__(name, aliases=aliases, **kwargs)
         self._nick = nick
-        self._name = name
         self._nick_aliases = (tuple(nick_aliases)
                               if nick_aliases is not None
                               else tuple())
-        self._aliases = tuple(aliases) if aliases is not None else tuple()
         self._regexes = (self.get_rule_regex(),)
 
     def __str__(self):
         label = self.get_rule_label()
         plugin = self.get_plugin_name() or '(no-plugin)'
         aliases = '|'.join(self._aliases)
         nick = self._nick
@@ -1370,43 +1557,43 @@
 
         * the nicks to react to,
         * the rule's name (escaped for regex),
         * all of its aliases (escaped for regex),
 
         to create a compiled regex to return.
         """
-        name = [self.escape_name(self._name)]
-        aliases = [self.escape_name(alias) for alias in self._aliases]
+        name = [re.escape(self._name)]
+        aliases = [re.escape(alias) for alias in self._aliases]
         pattern = r'|'.join(name + aliases)
 
         return _compile_pattern(
             self.PATTERN_TEMPLATE.format(command=pattern),
             self._nick,
             self._nick_aliases)
 
 
-class ActionCommand(NamedRuleMixin, Rule):
+class ActionCommand(AbstractNamedRule):
     """Action Command rule definition.
 
     An action command rule is a named rule that can be triggered only when the
-    trigger's intent is an ``ACTION``. Like the :class:`Command` rule, it
+    trigger's CTCP command is an ``ACTION``. Like the :class:`Command` rule, it
     allows command aliases.
 
     Here is an example with the ``dummy`` action command:
 
     .. code-block:: irc
 
         > user dummy
         <Bot> You just invoked the action command 'dummy'
         > user dummy-alias
         <Bot> You just invoked the action command 'dummy' (as 'dummy-alias')
 
     Apart from that, it behaves exactly like a :class:`generic rule <Rule>`.
     """
-    INTENT_REGEX = re.compile(r'ACTION', re.IGNORECASE)
+    CTCP_REGEX = re.compile(r'ACTION', re.IGNORECASE)
     PATTERN_TEMPLATE = r"""
         ({command})         # Command as group 1.
         (?:\s+              # Whitespace to end command.
         (                   # Rest of the line as group 2.
         (?:(\S+))?          # Parameters 1-4 as groups 3-6.
         (?:\s+(\S+))?
         (?:\s+(\S+))?
@@ -1433,17 +1620,15 @@
             'aliases': aliases,
             'handler': handler,
         })
 
         return cls(**kwargs)
 
     def __init__(self, name, aliases=None, **kwargs):
-        super(ActionCommand, self).__init__([], **kwargs)
-        self._name = name
-        self._aliases = tuple(aliases) if aliases is not None else tuple()
+        super().__init__(name, aliases=aliases, **kwargs)
         self._regexes = (self.get_rule_regex(),)
 
     def __str__(self):
         label = self.get_rule_label()
         plugin = self.get_plugin_name() or '(no-plugin)'
         aliases = '|'.join(self._aliases)
 
@@ -1457,29 +1642,28 @@
         The command regex factors in:
 
         * the rule's name (escaped for regex if needed),
         * all of its aliases (escaped for regex if needed),
 
         to create a compiled regex to return.
         """
-        name = [self.escape_name(self._name)]
-        aliases = [self.escape_name(alias) for alias in self._aliases]
+        name = [re.escape(self._name)]
+        aliases = [re.escape(alias) for alias in self._aliases]
         pattern = r'|'.join(name + aliases)
         pattern = self.PATTERN_TEMPLATE.format(command=pattern)
         return re.compile(pattern, re.IGNORECASE | re.VERBOSE)
 
-    def match_intent(self, intent):
-        """Tell if ``intent`` is an ``ACTION``.
+    def match_ctcp(self, command: Optional[str]) -> bool:
+        """Tell if ``command`` is an ``ACTION``.
 
-        :param str intent: potential matching intent
-        :return: ``True`` when ``intent`` matches ``ACTION``,
+        :param command: potential matching CTCP command
+        :return: ``True`` when ``command`` matches ``ACTION``,
                  ``False`` otherwise
-        :rtype: bool
         """
-        return bool(intent and self.INTENT_REGEX.match(intent))
+        return bool(command and self.CTCP_REGEX.match(command))
 
 
 class FindRule(Rule):
     """Anonymous find rule definition.
 
     A find rule is like an anonymous rule with a twist: instead of matching
     only once per IRC line, a find rule will execute for each non-overlapping
@@ -1584,33 +1768,38 @@
 
     """
     REGEX_ATTRIBUTE = 'url_regex'
     LAZY_ATTRIBUTE = 'url_lazy_loaders'
 
     @classmethod
     def from_callable(cls, settings, handler):
-        execute_handler = handler
         regexes = cls.regex_from_callable(settings, handler)
         kwargs = cls.kwargs_from_callable(handler)
 
         # do we need to handle the match parameter?
         # old style URL callback: callable(bot, trigger, match)
         # new style: callable(bot, trigger)
         match_count = 3
         if inspect.ismethod(handler):
             # account for the 'self' parameter when the handler is a method
             match_count = 4
 
-        argspec = inspect_getargspec(handler)
+        execute_handler = handler
+        argspec = inspect.getfullargspec(handler)
 
         if len(argspec.args) >= match_count:
             @functools.wraps(handler)
-            def execute_handler(bot, trigger):
+            def handler_match_wrapper(bot, trigger):
                 return handler(bot, trigger, match=trigger)
 
+            # don't directly `def execute_handler` to override it;
+            # doing incurs the wrath of pyflakes in the form of
+            # "F811: Redefinition of unused name"
+            execute_handler = handler_match_wrapper
+
         kwargs.update({
             'handler': execute_handler,
             'schemes': settings.core.auto_url_schemes,
         })
 
         return cls(regexes, **kwargs)
 
@@ -1648,15 +1837,15 @@
 
         return cls(regexes, **kwargs)
 
     def __init__(self,
                  regexes,
                  schemes=None,
                  **kwargs):
-        super(URLCallback, self).__init__(regexes, **kwargs)
+        super().__init__(regexes, **kwargs)
         # prevent mutability of registered schemes
         self._schemes = tuple(schemes or URL_DEFAULT_SCHEMES)
 
     def match(self, bot, pretrigger):
         """Match URL(s) in a pretrigger according to the rule.
 
         :param bot: Sopel instance
@@ -1684,16 +1873,14 @@
                 if urlparse(url).scheme not in self._schemes:
                     # skip URLs with unwanted scheme
                     continue
             except ValueError:
                 # skip invalid URLs
                 continue
 
-            # TODO: convert to 'yield from' when dropping Python 2.7
-            for result in self.parse(url):
-                yield result
+            yield from self.parse(url)
 
     def parse(self, text):
         for regex in self._regexes:
             result = regex.search(text)
             if result:
                 yield result
```

### Comparing `sopel-7.1.9/sopel/tests/__init__.py` & `sopel-8.0.0/sopel/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# coding=utf-8
 """Test tools, factories, pytest fixtures, and mocks.
 
 .. versionadded:: 7.0
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 
 def rawlist(*args):
     """Build a list of raw IRC messages from the lines given as ``*args``.
 
     :return: a list of raw IRC messages as seen by the bot
     :rtype: list
```

### Comparing `sopel-7.1.9/sopel/tests/mocks.py` & `sopel-8.0.0/sopel/tests/mocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# coding=utf-8
 """Test mocks: they fake objects for testing.
 
 .. versionadded:: 7.0
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 
 from sopel.irc.abstract_backends import AbstractIRCBackend
 
 
 class MockIRCBackend(AbstractIRCBackend):
     """Fake IRC connection backend for testing purpose.
@@ -36,15 +35,15 @@
 
         The
         :class:`parent class <sopel.irc.abstract_backends.AbstractIRCBackend>`
         contains all the methods that can be used on this test backend.
 
     """
     def __init__(self, *args, **kwargs):
-        super(MockIRCBackend, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.message_sent = []
         """List of raw messages sent by the bot.
 
         This list will be populated each time the :meth:`irc_send` method is
         used: it will contain the raw IRC lines the bot wanted to send.
 
         You can clear this list with the :meth:`clear_message_sent` method, or
@@ -52,14 +51,17 @@
         """
         self.connected = False
         """Convenient status flag.
 
         Set to ``True`` to make the bot think it is connected.
         """
 
+    def run_forever(self):
+        raise RuntimeError('MockIRCBackend cannot be used to run the client.')
+
     def is_connected(self):
         return self.connected
 
     def irc_send(self, data):
         """Store ``data`` into :attr:`message_sent`."""
         self.message_sent.append(data)
 
@@ -73,16 +75,20 @@
         """
         # make a copy
         sent = list(self.message_sent)
         # clear the message sent
         self.message_sent = []
         return sent
 
+    def on_irc_error(self, pretrigger):
+        # implement abstract method
+        pass
+
 
-class MockIRCServer(object):
+class MockIRCServer:
     """Fake IRC Server that can send messages to a test bot.
 
     :param bot: test bot instance to send messages to
     :type bot: :class:`sopel.bot.Sopel`
     :param bool join_threads: whether message functions should join running
                               threads before returning (default: ``True``)
 
@@ -98,32 +104,31 @@
 
     .. note::
 
         You can override ``join_threads`` on a per-method-call basis with the
         ``blocking`` arguments to the instance methods below.
 
     The :class:`~sopel.tests.factories.IRCFactory` factory can be used to
-    create such mock object, either directly or by using ``py.test`` and the
+    create such mock object, either directly or by using ``pytest`` and the
     :func:`~sopel.tests.pytest_plugin.ircfactory` fixture.
 
     .. versionadded:: 7.1
 
         The ``join_threads`` parameter.
     """
     def __init__(self, bot, join_threads=True):
         self.bot = bot
         self.join_threads = join_threads
-        # TODO: `blocking` method args below should be made kwarg-ONLY in py3
 
     @property
     def chanserv(self):
         """ChanServ's message prefix."""
         return 'ChanServ!ChanServ@services.'
 
-    def channel_joined(self, channel, users=None, blocking=None):
+    def channel_joined(self, channel, users=None, *, blocking=None):
         """Send events as if the bot just joined a channel.
 
         :param str channel: channel to send message for
         :param list users: list (or tuple) of nicknames that will be present
                            in the ``RPL_NAMREPLY`` event
         :param bool blocking: whether to block until all triggered threads
                               have finished (optional)
@@ -185,15 +190,15 @@
         )
         self.bot.on_message(message)
 
         if (blocking is None and self.join_threads) or blocking:
             for t in self.bot.running_triggers:
                 t.join()
 
-    def mode_set(self, channel, flags, users, blocking=None):
+    def mode_set(self, channel, flags, users, *, blocking=None):
         """Send a MODE event for a ``channel``
 
         :param str channel: channel receiving the MODE event
         :param str flags: MODE flags set
         :param list users: users getting the MODE flags
         :param bool blocking: whether to block until all triggered threads
                               have finished (optional)
@@ -227,15 +232,15 @@
         )
         self.bot.on_message(message)
 
         if (blocking is None and self.join_threads) or blocking:
             for t in self.bot.running_triggers:
                 t.join()
 
-    def join(self, user, channel, blocking=None):
+    def join(self, user, channel, *, blocking=None):
         """Send a ``channel`` JOIN event from ``user``.
 
         :param user: factory for the user who joins the ``channel``
         :type user: :class:`MockUser`
         :param str channel: channel the ``user`` joined
         :param bool blocking: whether to block until all triggered threads
                               have finished (optional)
@@ -265,15 +270,15 @@
         """
         self.bot.on_message(user.join(channel))
 
         if (blocking is None and self.join_threads) or blocking:
             for t in self.bot.running_triggers:
                 t.join()
 
-    def say(self, user, channel, text, blocking=None):
+    def say(self, user, channel, text, *, blocking=None):
         """Send a ``PRIVMSG`` to ``channel`` by ``user``.
 
         :param user: factory for the user who sends a message to ``channel``
         :type user: :class:`MockUser`
         :param str channel: recipient of the ``user``'s ``PRIVMSG``
         :param str text: content of the message sent to the ``channel``
         :param bool blocking: whether to block until all triggered threads
@@ -304,15 +309,15 @@
         """
         self.bot.on_message(user.privmsg(channel, text))
 
         if (blocking is None and self.join_threads) or blocking:
             for t in self.bot.running_triggers:
                 t.join()
 
-    def pm(self, user, text, blocking=None):
+    def pm(self, user, text, *, blocking=None):
         """Send a ``PRIVMSG`` to the bot by a ``user``.
 
         :param user: factory for the user object who sends a message
         :type user: :class:`MockUser`
         :param str text: content of the message sent to the bot
         :param bool blocking: whether to block until all triggered threads
                               have finished (optional)
@@ -344,23 +349,23 @@
         self.bot.on_message(user.privmsg(self.bot.nick, text))
 
         if (blocking is None and self.join_threads) or blocking:
             for t in self.bot.running_triggers:
                 t.join()
 
 
-class MockUser(object):
+class MockUser:
     """Fake user that can generate messages to send to a bot.
 
     :param str nick: nickname
     :param str user: IRC username
     :param str host: user's host
 
     The :class:`~sopel.tests.factories.UserFactory` factory can be used to
-    create such mock object, either directly or by using ``py.test`` and the
+    create such mock object, either directly or by using ``pytest`` and the
     :func:`~sopel.tests.pytest_plugin.userfactory` fixture.
     """
     def __init__(self, nick=None, user=None, host=None):
         self.nick = nick or 'Test'
         self.user = user or self.nick.lower()
         self.host = host or 'example.com'
```

### Comparing `sopel-7.1.9/sopel/tests/pytest_plugin.py` & `sopel-8.0.0/sopel/tests/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# coding=utf-8
 """Pytest plugin for Sopel.
 
 .. versionadded:: 7.0
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import re
 import sys
 
 import pytest
 
 from sopel import bot, loader, plugins, trigger
@@ -87,15 +86,20 @@
         match = parse_results[0]
         sender = mockbot.nick if privmsg else "#channel"
         hostmask = "%s!%s@%s" % (mockbot.nick, "UserName", "example.com")
 
         # TODO enable message tags
         full_message = ':{} PRIVMSG {} :{}'.format(hostmask, sender, msg)
         pretrigger = trigger.PreTrigger(
-            mockbot.nick, full_message, url_schemes=url_schemes)
+            mockbot.nick,
+            full_message,
+            url_schemes=url_schemes,
+            identifier_factory=mockbot.make_identifier,
+            statusmsg_prefixes=mockbot.isupport.get('STATUSMSG'),
+        )
         test_trigger = trigger.Trigger(mockbot.settings, pretrigger, match)
         pattern = re.compile(r'^%s: ' % re.escape(mockbot.nick))
 
         # setup module
         module = sys.modules[tested_func.__module__]
         if hasattr(module, 'setup'):
             module.setup(mockbot)
@@ -113,14 +117,16 @@
             tested_func(wrapper, test_trigger)
 
             output_triggers = (
                 trigger.PreTrigger(
                     mockbot.nick,
                     message.decode('utf-8'),
                     url_schemes=url_schemes,
+                    identifier_factory=mockbot.make_identifier,
+                    statusmsg_prefixes=mockbot.isupport.get('STATUSMSG'),
                 )
                 for message in wrapper.backend.message_sent
             )
             output_texts = (
                 # subtract "Sopel: " when necessary
                 pattern.sub('', output_trigger.args[-1])
                 for output_trigger in output_triggers
```

### Comparing `sopel-7.1.9/sopel/tools/_events.py` & `sopel-8.0.0/sopel/tools/_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# coding=utf-8
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+from enum import Enum
 
-class events(object):
+
+class events(str, Enum):
     """An enumeration of all the standardized and notable IRC numeric events
 
     This allows you to do, for example, ``@plugin.event(events.RPL_WELCOME)``
     rather than ``@plugin.event('001')``
     """
     # ###################################################### Non-RFC / Non-IRCv3
     # Only add things here if they're actually in common use across multiple
     # ircds.
     RPL_ISUPPORT = '005'
     RPL_WHOSPCRPL = '354'
+    RPL_INVITELIST = '336'
+    RPL_ENDOFINVITELIST = '337'
 
     # ################################################################### IRC v3
     # ## 3.1
     # CAP
     ERR_INVALIDCAPCMD = '410'
     # SASL
     RPL_LOGGEDIN = '900'
@@ -28,14 +31,16 @@
     ERR_SASLABORTED = '906'
     ERR_SASLALREADY = '907'
     RPL_SASLMECHS = '908'
     # TLS
     RPL_STARTTLS = '670'
     ERR_STARTTLS = '691'
     # ## 3.2
+    # Bot Mode
+    RPL_WHOISBOT = '335'
     # Metadata
     RPL_WHOISKEYVALUE = '760'
     RPL_KEYVALUE = '761'
     RPL_METADATAEND = '762'
     ERR_METADATALIMIT = '764'
     ERR_TARGETINVALID = '765'
     ERR_NOMATCHINGKEY = '766'
@@ -76,15 +81,15 @@
     ERR_USERONCHANNEL = '443'
     ERR_NOLOGIN = '444'
     ERR_SUMMONDISABLED = '445'
     ERR_USERSDISABLED = '446'
     ERR_NOTREGISTERED = '451'
     ERR_NEEDMOREPARAMS = '461'
     ERR_ALREADYREGISTRED = '462'
-    ERR_ALREADYREGISTERED = '462'  # corrected spelling used in some tutorials
+    ERR_ALREADYREGISTERED = ERR_ALREADYREGISTRED  # corrected spelling used in some tutorials
     ERR_NOPERMFORHOST = '463'
     ERR_PASSWDMISMATCH = '464'
     ERR_YOUREBANNEDCREEP = '465'
     ERR_KEYSET = '467'
     ERR_CHANNELISFULL = '471'
     ERR_UNKNOWNMODE = '472'
     ERR_INVITEONLYCHAN = '473'
@@ -176,16 +181,16 @@
     # ## 5.1 Command responses
     RPL_WELCOME = '001'
     RPL_YOURHOST = '002'
     RPL_CREATED = '003'
     RPL_MYINFO = '004'
     RPL_BOUNCE = '005'
     RPL_UNIQOPIS = '325'
-    RPL_INVITELIST = '346'
-    RPL_ENDOFINVITELIST = '347'
+    RPL_INVEXLIST = '346'
+    RPL_ENDOFINVEXLIST = '347'
     RPL_EXCEPTLIST = '348'
     RPL_ENDOFEXCEPTLIST = '349'
     RPL_YOURESERVICE = '383'
     RPL_TRACESERVICE = '207'
     RPL_TRACECLASS = '209'
     RPL_TRACERECONNECT = '210'
     RPL_TRACEEND = '262'
```

### Comparing `sopel-7.1.9/sopel/tools/calculation.py` & `sopel-8.0.0/sopel/tools/calculation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-# coding=utf-8
-"""Tools to help safely do calculations from user input"""
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""Tools to help safely do calculations from user input
+
+.. versionadded:: 5.3
+.. note::
+
+    Most of this is internal machinery. :func:`eval_equation` is the "public"
+    part, used by Sopel's built-in ``calc`` plugin.
+
+"""
+from __future__ import annotations
 
 import ast
-import numbers
 import operator
 import time
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Callable, Optional
 
 __all__ = ['eval_equation']
 
 
 class ExpressionEvaluator:
     """A generic class for evaluating limited forms of Python expressions.
 
@@ -19,107 +29,125 @@
     Instances can pass ``binary_ops`` and ``unary_ops`` arguments with dicts of
     the form ``{ast.Node, function}``. When the :class:`ast.Node <ast.AST>` used
     as key is found, it will be evaluated using the given ``function``.
     """
 
     class Error(Exception):
         """Internal exception type for :class:`ExpressionEvaluator`\\s."""
-        pass
 
-    def __init__(self, bin_ops=None, unary_ops=None):
+    def __init__(
+        self,
+        bin_ops: Optional[dict[type[ast.operator], Callable]] = None,
+        unary_ops: Optional[dict[type[ast.unaryop], Callable]] = None
+    ):
         self.binary_ops = bin_ops or {}
         self.unary_ops = unary_ops or {}
 
-    def __call__(self, expression_str, timeout=5.0):
+    def __call__(self, expression_str: str, timeout: float = 5.0):
         """Evaluate a Python expression and return the result.
 
-        :param str expression_str: the expression to evaluate
+        :param expression_str: the expression to evaluate
+        :param timeout: timeout for processing the expression, in seconds
         :raise SyntaxError: if the given ``expression_str`` is not a valid
                             Python statement
         :raise ExpressionEvaluator.Error: if the instance of
             :class:`ExpressionEvaluator` does not have a handler for the
             :class:`ast.Node <ast.AST>`
         """
         ast_expression = ast.parse(expression_str, mode='eval')
         return self._eval_node(ast_expression.body, time.time() + timeout)
 
-    def _eval_node(self, node, timeout):
+    def _eval_node(self, node: ast.AST, timeout: float):
         """Recursively evaluate the given :class:`ast.Node <ast.AST>`.
 
         :param node: the AST node to evaluate
-        :type node: :class:`ast.AST`
         :param timeout: how long the expression is allowed to process before
-                        timing out and failing
-        :type timeout: int or float
+                        timing out and failing, in seconds
         :raise ExpressionEvaluator.Error: if it can't handle the ``node``
 
         Uses :attr:`self.binary_ops` and :attr:`self.unary_ops` for the
         implementation.
 
         A subclass could overwrite this to handle more nodes, calling it only
         for nodes it does not implement itself.
         """
-        if isinstance(node, ast.Num):
-            return node.n
+        if isinstance(node, ast.Constant):
+            if not isinstance(node.value, (int, float)):
+                raise ExpressionEvaluator.Error(
+                    "'{}' values are not supported".format(
+                        type(node.value).__name__,
+                    )
+                )
+
+            return node.value
+
+        elif isinstance(node, ast.BinOp):
+            if type(node.op) not in self.binary_ops:
+                raise ExpressionEvaluator.Error(
+                    "Unsupported binary operator '{}'".format(
+                        type(node.op).__name__,
+                    )
+                )
 
-        elif (isinstance(node, ast.BinOp) and
-                type(node.op) in self.binary_ops):
             left = self._eval_node(node.left, timeout)
             right = self._eval_node(node.right, timeout)
             if time.time() > timeout:
                 raise ExpressionEvaluator.Error(
                     "Time for evaluating expression ran out.")
             return self.binary_ops[type(node.op)](left, right)
 
-        elif (isinstance(node, ast.UnaryOp) and
-                type(node.op) in self.unary_ops):
+        elif isinstance(node, ast.UnaryOp):
+            if type(node.op) not in self.unary_ops:
+                raise ExpressionEvaluator.Error(
+                    "Unsupported unary operator '{}'".format(
+                        type(node.op).__name__,
+                    )
+                )
+
             operand = self._eval_node(node.operand, timeout)
             if time.time() > timeout:
                 raise ExpressionEvaluator.Error(
                     "Time for evaluating expression ran out.")
             return self.unary_ops[type(node.op)](operand)
 
         raise ExpressionEvaluator.Error(
-            "Ast.Node '%s' not implemented." % (type(node).__name__,))
+            "Node type '{}' is not supported.".format(
+                type(node).__name__,
+            )
+        )
 
 
-def guarded_mul(left, right):
+def guarded_mul(left: float, right: float):
     """Multiply two values, guarding against overly large inputs.
 
     :param left: the left operand
-    :type left: int or float
     :param right: the right operand
-    :type right: int or float
     :raise ValueError: if the inputs are too large to handle safely
     """
     # Only handle ints because floats will overflow anyway.
-    if not isinstance(left, numbers.Integral):
-        pass
-    elif not isinstance(right, numbers.Integral):
+    if not isinstance(left, int) or not isinstance(right, int):
         pass
     elif left in (0, 1) or right in (0, 1):
         # Ignore trivial cases.
         pass
     elif left.bit_length() + right.bit_length() > 664386:
         # 664386 is the number of bits (10**100000)**2 has, which is instant on
         # my laptop, while (10**1000000)**2 has a noticeable delay. It could
         # certainly be improved.
         raise ValueError(
             "Value is too large to be handled in limited time and memory.")
 
     return operator.mul(left, right)
 
 
-def pow_complexity(num, exp):
+def pow_complexity(num: int, exp: int):
     """Estimate the worst case time :func:`pow` takes to calculate.
 
     :param num: base
-    :type num: int or float
     :param exp: exponent
-    :type exp: int or float
 
     This function is based on experimental data from the time it takes to
     calculate ``num**exp`` in 32-bit CPython 2.7.6 on an Intel Core i7-2670QM
     laptop running Windows.
 
     It tries to implement this surface: x=exp, y=num
 
@@ -173,63 +201,66 @@
     elif (num & (num - 1)) == 0:
         # For powers of 2 the scaling is a bit different.
         return exp ** 1.092 * num.bit_length() ** 1.65 / 623212911.121
     else:
         return exp ** 1.590 * num.bit_length() ** 1.73 / 36864057619.3
 
 
-def guarded_pow(num, exp):
+def guarded_pow(num: float, exp: float):
     """Raise a number to a power, guarding against overly large inputs.
 
     :param num: base
-    :type num: int or float
     :param exp: exponent
-    :type exp: int or float
     :raise ValueError: if the inputs are too large to handle safely
     """
     # Only handle ints because floats will overflow anyway.
-    if not isinstance(num, numbers.Integral):
-        pass
-    elif not isinstance(exp, numbers.Integral):
+    if not isinstance(num, int) or not isinstance(exp, int):
         pass
     elif pow_complexity(num, exp) < 0.5:
         # Value 0.5 is arbitrary and based on an estimated runtime of 0.5s
         # on a fairly decent laptop processor.
         pass
     else:
         raise ValueError("Pow expression too complex to calculate.")
 
     return operator.pow(num, exp)
 
 
 class EquationEvaluator(ExpressionEvaluator):
-    __bin_ops = {
+    """Specific subclass of :class:`ExpressionEvaluator` for simple math
+
+    This presets the allowed operators to safeguard against user input that
+    could try to do things that will adversely affect the running bot, while
+    still letting users pass arbitrary mathematical expressions using the
+    available (mostly arithmetic) operators.
+    """
+    __bin_ops: dict[type[ast.operator], Callable] = {
         ast.Add: operator.add,
         ast.Sub: operator.sub,
         ast.Mult: guarded_mul,
         ast.Div: operator.truediv,
         ast.Pow: guarded_pow,
         ast.Mod: operator.mod,
         ast.FloorDiv: operator.floordiv,
         ast.BitXor: guarded_pow
     }
-    __unary_ops = {
+    __unary_ops: dict[type[ast.unaryop], Callable] = {
         ast.USub: operator.neg,
         ast.UAdd: operator.pos,
     }
 
     def __init__(self):
         ExpressionEvaluator.__init__(
             self,
             bin_ops=self.__bin_ops,
             unary_ops=self.__unary_ops
         )
 
-    def __call__(self, expression_str):
-        result = ExpressionEvaluator.__call__(self, expression_str)
+    def __call__(self, expression_str: str, timeout: float = 5.0):
+        result = ExpressionEvaluator.__call__(self, expression_str, timeout)
 
         # This wrapper is here so additional sanity checks could be done
         # on the result of the eval, but currently none are done.
 
         return result
```

### Comparing `sopel-7.1.9/sopel/tools/jobs.py` & `sopel-8.0.0/sopel/tools/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# coding=utf-8
 """Sopel's Job Scheduler: internal tool for job management.
 
 .. important::
 
     As of Sopel 5.3, this is an internal tool used by Sopel to manage internal
     jobs and should not be used by plugin authors. Its usage and documentation
     is for Sopel core development and advanced developers. It is subject to
     rapid changes between versions without much (or any) warning.
 
 """
 # Copyright 2019, Florian Strzelecki <florian.strzelecki@gmail.com>
 #
 # Licensed under the Eiffel Forum License 2.
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
 import inspect
 import logging
 import threading
 import time
 
 
@@ -190,15 +189,15 @@
             with job:
                 job.execute(self.manager)
         except Exception as error:  # TODO: Be specific
             LOGGER.error('Error while processing job: %s', error)
             self.manager.on_job_error(self, job, error)
 
 
-class Job(object):
+class Job:
     """Holds information about when a function should be called next.
 
     :param intervals: set of intervals; each is a number of seconds between
                       calls to ``handler``
     :type intervals: :term:`iterable`
     :param str plugin: optional plugin name to which the job belongs
     :param str label: optional label (name) for the job
```

### Comparing `sopel-7.1.9/sopel/tools/target.py` & `sopel-8.0.0/sopel/tools/target.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,171 +1,257 @@
-# coding=utf-8
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""User and channel objects used in state tracking."""
+from __future__ import annotations
 
 import functools
+from typing import Any, Optional, TYPE_CHECKING, Union
 
-from sopel import plugin
-from sopel.tools import Identifier
+from sopel.privileges import AccessLevel
+from sopel.tools import memories
+from sopel.tools.identifiers import Identifier, IdentifierFactory
+
+if TYPE_CHECKING:
+    import datetime
 
 
 @functools.total_ordering
-class User(object):
+class User:
     """A representation of a user Sopel is aware of.
 
     :param nick: the user's nickname
-    :type nick: :class:`~.tools.Identifier`
+    :type nick: :class:`sopel.tools.identifiers.Identifier`
     :param str user: the user's local username ("user" in `user@host.name`)
     :param str host: the user's hostname ("host.name" in `user@host.name`)
     """
-    def __init__(self, nick, user, host):
+    __slots__ = (
+        'nick', 'user', 'host', 'realname', 'channels', 'account', 'away', 'is_bot',
+    )
+
+    def __init__(
+        self,
+        nick: Identifier,
+        user: Optional[str],
+        host: Optional[str],
+    ) -> None:
         assert isinstance(nick, Identifier)
-        self.nick = nick
+        self.nick: Identifier = nick
         """The user's nickname."""
-        self.user = user
-        """The user's local username."""
-        self.host = host
-        """The user's hostname."""
-        self.channels = {}
+        self.user: Optional[str] = user
+        """The user's local username.
+
+        Will be ``None`` if Sopel has not yet received complete user
+        information from the IRC server.
+        """
+        self.host: Optional[str] = host
+        """The user's hostname.
+
+        Will be ``None`` if Sopel has not yet received complete user
+        information from the IRC server.
+        """
+        self.realname: Optional[str] = None
+        """The user's realname.
+
+        Will be ``None`` if Sopel has not yet received complete user
+        information from the IRC server.
+        """
+        self.channels: dict[Identifier, 'Channel'] = {}
         """The channels the user is in.
 
-        This maps channel name :class:`~sopel.tools.Identifier`\\s to
-        :class:`Channel` objects.
+        This maps channel name :class:`~sopel.tools.identifiers.Identifier`\\s
+        to :class:`Channel` objects.
         """
-        self.account = None
+        self.account: Optional[str] = None
         """The IRC services account of the user.
 
         This relies on IRCv3 account tracking being enabled.
+
+        Will be ``None`` if the user is not logged into an account (including
+        when account tracking is not supported by the IRC server.)
         """
-        self.away = None
-        """Whether the user is marked as away."""
+        self.away: Optional[bool] = None
+        """Whether the user is marked as away.
 
-    hostmask = property(lambda self: '{}!{}@{}'.format(self.nick, self.user,
-                                                       self.host))
-    """The user's full hostmask."""
+        Will be ``None`` if the user's current away state hasn't been
+        established yet (via WHO or other means such as ``away-notify``).
+        """
+        self.is_bot: Optional[bool] = None
+        """Whether the user is flagged as a bot.
 
-    def __eq__(self, other):
+        Will be ``None`` if the user hasn't yet been WHOed, or if the IRC
+        server does not support a 'bot' user mode.
+        """
+
+    @property
+    def hostmask(self) -> str:
+        """The user's full hostmask (``nick!user@host``)."""
+        # TODO: this won't work as expected if `user`/`host` is still `None`
+        return '{}!{}@{}'.format(
+            self.nick,
+            self.user,
+            self.host,
+        )
+
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, User):
             return NotImplemented
         return self.nick == other.nick
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any) -> bool:
         if not isinstance(other, User):
             return NotImplemented
         return self.nick < other.nick
 
 
 @functools.total_ordering
-class Channel(object):
+class Channel:
     """A representation of a channel Sopel is in.
 
     :param name: the channel name
-    :type name: :class:`~.tools.Identifier`
+    :type name: :class:`~sopel.tools.identifiers.Identifier`
+    :param identifier_factory: A factory to create
+                               :class:`~sopel.tools.identifiers.Identifier`\\s
     """
-    def __init__(self, name):
+    __slots__ = (
+        'name',
+        'users',
+        'privileges',
+        'topic',
+        'modes',
+        'last_who',
+        'join_time',
+        'make_identifier',
+    )
+
+    def __init__(
+        self,
+        name: Identifier,
+        identifier_factory: IdentifierFactory = Identifier,
+    ) -> None:
         assert isinstance(name, Identifier)
-        self.name = name
+        self.name: Identifier = name
         """The name of the channel."""
-        self.users = {}
+
+        self.make_identifier: IdentifierFactory = identifier_factory
+        """Factory to create :class:`~sopel.tools.identifiers.Identifier`.
+
+        ``Identifier`` is used for :class:`User`'s nick, and the channel
+        needs to translate nicks from string to ``Identifier`` when
+        manipulating data associated to a user by its nickname.
+        """
+
+        self.users: dict[
+            Identifier,
+            User,
+        ] = memories.SopelIdentifierMemory(
+            identifier_factory=self.make_identifier,
+        )
         """The users in the channel.
 
-        This maps nickname :class:`~sopel.tools.Identifier`\\s to :class:`User`
-        objects.
+        This maps nickname :class:`~sopel.tools.identifiers.Identifier`\\s to
+        :class:`User` objects.
         """
-        self.privileges = {}
+        self.privileges: dict[
+            Identifier,
+            int,
+        ] = memories.SopelIdentifierMemory(
+            identifier_factory=self.make_identifier,
+        )
         """The permissions of the users in the channel.
 
-        This maps nickname :class:`~sopel.tools.Identifier`\\s to bitwise
-        integer values. This can be compared to appropriate constants from
-        :mod:`sopel.plugin`.
+        This maps nickname :class:`~sopel.tools.identifiers.Identifier`\\s to
+        bitwise integer values. This can be compared to appropriate constants
+        from :class:`sopel.privileges.AccessLevel`.
         """
-        self.topic = ''
+        self.topic: str = ''
         """The topic of the channel."""
 
-        self.modes = {}
+        self.modes: dict[str, Union[set, str, bool]] = {}
         """The channel's modes.
 
         For type A modes (nick/address list), the value is a set. For type B
         (parameter) or C (parameter when setting), the value is a string. For
         type D, the value is ``True``.
 
         .. note::
 
             Type A modes may only contain changes the bot has observed. Sopel
             does not automatically populate all modes and lists.
         """
 
-        self.last_who = None
+        self.last_who: Optional[datetime.datetime] = None
         """The last time a WHO was requested for the channel."""
 
-    def clear_user(self, nick):
+        self.join_time: Optional[datetime.datetime] = None
+        """The time the server acknowledged our JOIN message.
+
+        Based on server-reported time if the ``server-time`` IRCv3 capability
+        is available, otherwise the time Sopel received it.
+        """
+
+    def clear_user(self, nick: Identifier) -> None:
         """Remove ``nick`` from this channel.
 
         :param nick: the nickname of the user to remove
-        :type nick: :class:`~.tools.Identifier`
 
         Called after a user leaves the channel via PART, KICK, QUIT, etc.
         """
         user = self.users.pop(nick, None)
         self.privileges.pop(nick, None)
         if user is not None:
             user.channels.pop(self.name, None)
 
-    def add_user(self, user, privs=0):
+    def add_user(self, user: User, privs: int = 0) -> None:
         """Add ``user`` to this channel.
 
         :param user: the new user to add
-        :type user: :class:`User`
-        :param int privs: privilege bitmask (see constants in
-                          :mod:`sopel.plugin`)
+        :param privs: privilege bitmask (see constants in
+                      :class:`sopel.privileges.AccessLevel`)
 
         Called when a new user JOINs the channel.
         """
         assert isinstance(user, User)
         self.users[user.nick] = user
         self.privileges[user.nick] = privs or 0
         user.channels[self.name] = self
 
-    def has_privilege(self, nick, privilege):
+    def has_privilege(self, nick: str, privilege: int) -> bool:
         """Tell if a user has a ``privilege`` level or above in this channel.
 
-        :param str nick: a user's nick in this channel
-        :param int privilege: privilege level to check
-        :rtype: bool
+        :param nick: a user's nick in this channel
+        :param privilege: privilege level to check
 
         This method checks the user's privilege level in this channel, i.e. if
         it has this level or higher privileges::
 
             >>> channel.add_user(some_user, plugin.OP)
             >>> channel.has_privilege(some_user.nick, plugin.VOICE)
             True
 
         The ``nick`` argument can be either a :class:`str` or a
-        :class:`sopel.tools.Identifier`. If the user is not in this channel,
-        it will be considered as not having any privilege.
+        :class:`sopel.tools.identifiers.Identifier`. If the user is not in this
+        channel, it will be considered as not having any privilege.
 
         .. seealso::
 
             There are other methods to check the exact privilege level of a
             user, such as :meth:`is_oper`, :meth:`is_owner`, :meth:`is_admin`,
             :meth:`is_op`, :meth:`is_halfop`, and :meth:`is_voiced`.
 
         .. important::
 
             Not all IRC networks support all privilege levels. If you intend
             for your plugin to run on any network, it is safest to rely only
             on the presence of standard modes: ``+v`` (voice) and ``+o`` (op).
 
         """
-        return self.privileges.get(Identifier(nick), 0) >= privilege
+        return self.privileges.get(self.make_identifier(nick), 0) >= privilege
 
-    def is_oper(self, nick):
+    def is_oper(self, nick: str) -> bool:
         """Tell if a user has the OPER (operator) privilege level.
 
-        :param str nick: a user's nick in this channel
-        :rtype: bool
+        :param nick: a user's nick in this channel
 
         Unlike :meth:`has_privilege`, this method checks if the user has been
         explicitly granted the OPER privilege level::
 
             >>> channel.add_user(some_user, plugin.OPER)
             >>> channel.is_oper(some_user.nick)
             True
@@ -183,21 +269,21 @@
         .. important::
 
             Not all IRC networks support this privilege mode. If you are
             writing a plugin for public distribution, ensure your code behaves
             sensibly if only ``+v`` (voice) and ``+o`` (op) modes exist.
 
         """
-        return self.privileges.get(Identifier(nick), 0) & plugin.OPER
+        identifier = self.make_identifier(nick)
+        return bool(self.privileges.get(identifier, 0) & AccessLevel.OPER)
 
-    def is_owner(self, nick):
+    def is_owner(self, nick: str) -> bool:
         """Tell if a user has the OWNER privilege level.
 
-        :param str nick: a user's nick in this channel
-        :rtype: bool
+        :param nick: a user's nick in this channel
 
         Unlike :meth:`has_privilege`, this method checks if the user has been
         explicitly granted the OWNER privilege level::
 
             >>> channel.add_user(some_user, plugin.OWNER)
             >>> channel.is_owner(some_user.nick)
             True
@@ -215,21 +301,21 @@
         .. important::
 
             Not all IRC networks support this privilege mode. If you are
             writing a plugin for public distribution, ensure your code behaves
             sensibly if only ``+v`` (voice) and ``+o`` (op) modes exist.
 
         """
-        return self.privileges.get(Identifier(nick), 0) & plugin.OWNER
+        identifier = self.make_identifier(nick)
+        return bool(self.privileges.get(identifier, 0) & AccessLevel.OWNER)
 
-    def is_admin(self, nick):
+    def is_admin(self, nick: str) -> bool:
         """Tell if a user has the ADMIN privilege level.
 
-        :param str nick: a user's nick in this channel
-        :rtype: bool
+        :param nick: a user's nick in this channel
 
         Unlike :meth:`has_privilege`, this method checks if the user has been
         explicitly granted the ADMIN privilege level::
 
             >>> channel.add_user(some_user, plugin.ADMIN)
             >>> channel.is_admin(some_user.nick)
             True
@@ -247,21 +333,21 @@
         .. important::
 
             Not all IRC networks support this privilege mode. If you are
             writing a plugin for public distribution, ensure your code behaves
             sensibly if only ``+v`` (voice) and ``+o`` (op) modes exist.
 
         """
-        return self.privileges.get(Identifier(nick), 0) & plugin.ADMIN
+        identifier = self.make_identifier(nick)
+        return bool(self.privileges.get(identifier, 0) & AccessLevel.ADMIN)
 
-    def is_op(self, nick):
+    def is_op(self, nick: str) -> bool:
         """Tell if a user has the OP privilege level.
 
-        :param str nick: a user's nick in this channel
-        :rtype: bool
+        :param nick: a user's nick in this channel
 
         Unlike :meth:`has_privilege`, this method checks if the user has been
         explicitly granted the OP privilege level::
 
             >>> channel.add_user(some_user, plugin.OP)
             >>> channel.is_op(some_user.nick)
             True
@@ -273,21 +359,21 @@
             >>> channel.add_user(some_user, plugin.OP | plugin.VOICE)
             >>> channel.is_op(some_user.nick)
             True
             >>> channel.is_voiced(some_user.nick)
             True
 
         """
-        return self.privileges.get(Identifier(nick), 0) & plugin.OP
+        identifier = self.make_identifier(nick)
+        return bool(self.privileges.get(identifier, 0) & AccessLevel.OP)
 
-    def is_halfop(self, nick):
+    def is_halfop(self, nick: str) -> bool:
         """Tell if a user has the HALFOP privilege level.
 
-        :param str nick: a user's nick in this channel
-        :rtype: bool
+        :param nick: a user's nick in this channel
 
         Unlike :meth:`has_privilege`, this method checks if the user has been
         explicitly granted the HALFOP privilege level::
 
             >>> channel.add_user(some_user, plugin.HALFOP)
             >>> channel.is_halfop(some_user.nick)
             True
@@ -305,21 +391,21 @@
         .. important::
 
             Not all IRC networks support this privilege mode. If you are
             writing a plugin for public distribution, ensure your code behaves
             sensibly if only ``+v`` (voice) and ``+o`` (op) modes exist.
 
         """
-        return self.privileges.get(Identifier(nick), 0) & plugin.HALFOP
+        identifier = self.make_identifier(nick)
+        return bool(self.privileges.get(identifier, 0) & AccessLevel.HALFOP)
 
-    def is_voiced(self, nick):
+    def is_voiced(self, nick: str) -> bool:
         """Tell if a user has the VOICE privilege level.
 
-        :param str nick: a user's nick in this channel
-        :rtype: bool
+        :param nick: a user's nick in this channel
 
         Unlike :meth:`has_privilege`, this method checks if the user has been
         explicitly granted the VOICE privilege level::
 
             >>> channel.add_user(some_user, plugin.VOICE)
             >>> channel.is_voiced(some_user.nick)
             True
@@ -332,34 +418,33 @@
             >>> channel.add_user(some_user, plugin.VOICE | plugin.OP)
             >>> channel.is_voiced(some_user.nick)
             True
             >>> channel.is_op(some_user.nick)
             True
 
         """
-        return self.privileges.get(Identifier(nick), 0) & plugin.VOICE
+        identifier = self.make_identifier(nick)
+        return bool(self.privileges.get(identifier, 0) & AccessLevel.VOICE)
 
-    def rename_user(self, old, new):
+    def rename_user(self, old: Identifier, new: Identifier) -> None:
         """Rename a user.
 
         :param old: the user's old nickname
-        :type old: :class:`~.tools.Identifier`
         :param new: the user's new nickname
-        :type new: :class:`~.tools.Identifier`
 
-        Called on NICK events.
+        Called on ``NICK`` events.
         """
         if old in self.users:
             self.users[new] = self.users.pop(old)
             self.users[new].nick = new
         if old in self.privileges:
             self.privileges[new] = self.privileges.pop(old)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Channel):
             return NotImplemented
         return self.name == other.name
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any) -> bool:
         if not isinstance(other, Channel):
             return NotImplemented
         return self.name < other.name
```

### Comparing `sopel-7.1.9/sopel/tools/time.py` & `sopel-8.0.0/sopel/tools/time.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,173 @@
-# coding=utf-8
-"""Tools for getting and displaying the time."""
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""Tools for getting and displaying the time.
+
+.. versionadded:: 5.3
+.. versionchanged:: 6.0
+
+    Moved from ``willie`` namespace to ``sopel`` namespace for project rename.
+
+"""
+from __future__ import annotations
 
 import datetime
+from typing import cast, NamedTuple, Optional, TYPE_CHECKING, Union
 
 import pytz
 
+if TYPE_CHECKING:
+    from sopel.config import Config
+    from sopel.db import SopelDB
+
 
 # various time units measured in seconds; approximated for months and years
 SECONDS = 1
 MINUTES = 60 * SECONDS
 HOURS = 60 * MINUTES
 DAYS = 24 * HOURS
 MONTHS = int(30.5 * DAYS)
 YEARS = 365 * DAYS
 
 
-def validate_timezone(zone):
-    """Return an IETF timezone from the given IETF zone or common abbreviation.
+class Duration(NamedTuple):
+    """Named tuple representation of a duration.
+
+    This can be used as a tuple as well as an object::
+
+        >>> d = Duration(minutes=12, seconds=34)
+        >>> d.minutes
+        12
+        >>> d.seconds
+        34
+        >>> years, months, days, hours, minutes, seconds = d
+        >>> (years, months, days, hours, minutes, seconds)
+        (0, 0, 0, 0, 12, 34)
+
+    """
+    years: int = 0
+    """Years spent."""
+    months: int = 0
+    """Months spent."""
+    days: int = 0
+    """Days spent."""
+    hours: int = 0
+    """Hours spent."""
+    minutes: int = 0
+    """Minutes spent."""
+    seconds: int = 0
+    """Seconds spent."""
+
+
+def validate_timezone(zone: Optional[str]) -> str:
+    """Normalize and validate an IANA timezone name.
 
-    :param str zone: in a strict or a human-friendly format
-    :return: the valid IETF timezone properly formatted
+    :param zone: in a strict or a human-friendly format
+    :return: the valid IANA timezone properly formatted
     :raise ValueError: when ``zone`` is not a valid timezone
+                       (including empty string and ``None`` value)
 
     Prior to checking timezones, two transformations are made to make the zone
     names more human-friendly:
 
     1. the string is split on ``', '``, the pieces reversed, and then joined
        with ``/`` (*"New York, America"* becomes *"America/New York"*)
     2. Remaining spaces are replaced with ``_``
 
     This means ``new york, america`` becomes ``America/New_York``, and ``utc``
     becomes ``UTC``. In the majority of user-facing interactions, such
     case-insensitivity will be expected.
 
-    If the zone is not valid, ``ValueError`` will be raised.
+    If the zone is not valid, :exc:`ValueError` will be raised.
+
+    .. versionadded:: 6.0
+
+    .. versionchanged:: 8.0
+
+        If ``zone`` is ``None``, raises a :exc:`ValueError` as if it was an
+        empty string or an invalid timezone instead of returning ``None``.
+
     """
     if zone is None:
-        return None
+        raise ValueError('Invalid time zone.')
 
     zone = '/'.join(reversed(zone.split(', '))).replace(' ', '_')
     try:
         tz = pytz.timezone(zone)
     except pytz.exceptions.UnknownTimeZoneError:
         raise ValueError('Invalid time zone.')
-    return tz.zone
+
+    return cast(str, tz.zone)
 
 
-def validate_format(tformat):
+def validate_format(tformat: str) -> str:
     """Validate a time format string.
 
-    :param str tformat: the format string to validate
+    :param tformat: the format string to validate
     :return: the format string, if valid
     :raise ValueError: when ``tformat`` is not a valid time format string
+
+    .. versionadded:: 6.0
     """
     try:
-        time = datetime.datetime.utcnow()
+        time = datetime.datetime.now(datetime.timezone.utc)
         time.strftime(tformat)
     except (ValueError, TypeError):
         raise ValueError('Invalid time format.')
     return tformat
 
 
-def get_nick_timezone(db, nick):
+def get_nick_timezone(db: SopelDB, nick: str) -> Optional[str]:
     """Get a nick's timezone from database.
 
     :param db: Bot's database handler (usually ``bot.db``)
-    :type db: :class:`~sopel.db.SopelDB`
     :param nick: IRC nickname
-    :type nick: :class:`~sopel.tools.Identifier`
     :return: the timezone associated with the ``nick``
 
     If a timezone cannot be found for ``nick``, or if it is invalid, ``None``
     will be returned.
+
+    .. versionadded:: 7.0
     """
     try:
         return validate_timezone(db.get_nick_value(nick, 'timezone'))
     except ValueError:
         return None
 
 
-def get_channel_timezone(db, channel):
+def get_channel_timezone(db: SopelDB, channel: str) -> Optional[str]:
     """Get a channel's timezone from database.
 
     :param db: Bot's database handler (usually ``bot.db``)
-    :type db: :class:`~sopel.db.SopelDB`
     :param channel: IRC channel name
-    :type channel: :class:`~sopel.tools.Identifier`
     :return: the timezone associated with the ``channel``
 
     If a timezone cannot be found for ``channel``, or if it is invalid,
     ``None`` will be returned.
+
+    .. versionadded:: 7.0
     """
     try:
         return validate_timezone(db.get_channel_value(channel, 'timezone'))
     except ValueError:
         return None
 
 
-def get_timezone(db=None, config=None, zone=None, nick=None, channel=None):
+def get_timezone(
+    db: Optional[SopelDB] = None,
+    config: Optional[Config] = None,
+    zone: Optional[str] = None,
+    nick: Optional[str] = None,
+    channel: Optional[str] = None,
+) -> Optional[str]:
     """Find, and return, the appropriate timezone.
 
     :param db: bot database object (optional)
-    :type db: :class:`~.db.SopelDB`
     :param config: bot config object (optional)
-    :type config: :class:`~.config.Config`
-    :param str zone: preferred timezone name (optional)
-    :param str nick: nick whose timezone to use, if set (optional)
-    :param str channel: channel whose timezone to use, if set (optional)
+    :param zone: preferred timezone name (optional)
+    :param nick: nick whose timezone to use, if set (optional)
+    :param channel: channel whose timezone to use, if set (optional)
 
     Timezone is pulled in the following priority:
 
     1. ``zone``, if it is valid
     2. The timezone for the channel or nick ``zone`` in ``db`` if one is set
        and valid.
     3. The timezone for the nick ``nick`` in ``db``, if one is set and valid.
@@ -127,132 +183,170 @@
 
     .. seealso::
 
        The :func:`validate_timezone` function handles the validation and
        formatting of the timezone.
 
     """
-    def _check(zone):
+    def _check(zone: Optional[str]) -> Optional[str]:
         try:
             return validate_timezone(zone)
         except ValueError:
             return None
 
-    tz = None
+    tz: Optional[str] = None
 
     if zone:
         tz = _check(zone)
-        if not tz:
-            tz = _check(
-                db.get_nick_or_channel_value(zone, 'timezone'))
-    if not tz and nick:
-        tz = _check(db.get_nick_value(nick, 'timezone'))
-    if not tz and channel:
-        tz = _check(db.get_channel_value(channel, 'timezone'))
-    if not tz and config and config.core.default_timezone:
+        # zone might be a nick or a channel
+        if not tz and db is not None:
+            tz = _check(db.get_nick_or_channel_value(zone, 'timezone'))
+
+    # get nick's timezone, and if none, get channel's timezone instead
+    if not tz and db is not None:
+        if nick:
+            tz = _check(db.get_nick_value(nick, 'timezone'))
+        if not tz and channel:
+            tz = _check(db.get_channel_value(channel, 'timezone'))
+
+    # if still not found, default to core configuration
+    if not tz and config is not None and config.core.default_timezone:
         tz = _check(config.core.default_timezone)
+
     return tz
 
 
-def format_time(db=None, config=None, zone=None, nick=None, channel=None,
-                time=None):
+def format_time(
+    db: Optional[SopelDB] = None,
+    config: Optional[Config] = None,
+    zone: Optional[str] = None,
+    nick: Optional[str] = None,
+    channel: Optional[str] = None,
+    time: Optional[datetime.datetime] = None,
+) -> str:
     """Return a formatted string of the given time in the given zone.
 
     :param db: bot database object (optional)
-    :type db: :class:`~.db.SopelDB`
     :param config: bot config object (optional)
-    :type config: :class:`~.config.Config`
-    :param str zone: name of timezone to use (optional)
-    :param str nick: nick whose time format to use, if set (optional)
-    :param str channel: channel whose time format to use, if set (optional)
+    :param zone: name of timezone to use for output (optional)
+    :param nick: nick whose time format to use, if set (optional)
+    :param channel: channel whose time format to use, if set (optional)
     :param time: the time value to format (optional)
-    :type time: :class:`~datetime.datetime`
 
-    ``time``, if given, should be a naive ``datetime.datetime`` object and will
-    be treated as being in the UTC timezone. If it is not given, the current
-    time will be used. If ``zone`` is given it must be present in the IANA Time
-    Zone Database; ``get_timezone`` can be helpful for this. If ``zone`` is not
-    given, UTC will be assumed.
+    ``time``, if given, should be a ``~datetime.datetime`` object, and will be
+    treated as being in the UTC timezone if it is :ref:`naïve
+    <datetime-naive-aware>`. If ``time`` is not given, the current time will
+    be used.
+
+    If ``zone`` is given it must be present in the IANA Time Zone Database;
+    ``get_timezone`` can be helpful for this. If ``zone`` is not given, UTC
+    will be assumed.
 
     The format for the string is chosen in the following order:
 
     1. The format for the nick ``nick`` in ``db``, if one is set and valid.
     2. The format for the channel ``channel`` in ``db``, if one is set and
        valid.
     3. The default format in ``config``, if one is set and valid.
     4. ISO-8601
 
     If ``db`` is not given or is not set up, steps 1 and 2 are skipped. If
     ``config`` is not given, step 3 will be skipped.
     """
-    tformat = None
+    target_tz: datetime.tzinfo = pytz.utc
+    tformat: Optional[str] = None
+
+    # get an aware datetime
+    if not time:
+        time = datetime.datetime.now(datetime.timezone.utc)
+    elif not time.tzinfo:
+        time = pytz.utc.localize(time)
+
+    # get target timezone
+    if zone:
+        target_tz = pytz.timezone(zone)
+
+    # get format for nick or channel
     if db:
         if nick:
             tformat = db.get_nick_value(nick, 'time_format')
         if not tformat and channel:
             tformat = db.get_channel_value(channel, 'time_format')
+
+    # get format from configuration
     if not tformat and config and config.core.default_time_format:
         tformat = config.core.default_time_format
+
+    # or default to hard-coded format
     if not tformat:
-        tformat = '%Y-%m-%d - %T%Z'
+        tformat = '%Y-%m-%d - %T %z'
 
-    if not time:
-        time = datetime.datetime.utcnow()
+    # format local time with format
+    return time.astimezone(target_tz).strftime(tformat)
 
-    if not zone:
-        return time.strftime(tformat)
-    else:
-        if not time.tzinfo:
-            utc = pytz.timezone('UTC')
-            time = utc.localize(time)
-        zone = pytz.timezone(zone)
-        return time.astimezone(zone).strftime(tformat)
 
-
-def seconds_to_split(seconds):
+def seconds_to_split(seconds: int) -> Duration:
     """Split an amount of ``seconds`` into years, months, days, etc.
 
-    :param int seconds: amount of time in seconds
-    :return: the time split into a tuple of years, months, days, hours,
+    :param seconds: amount of time in seconds
+    :return: the time split into a named tuple of years, months, days, hours,
              minutes, and seconds
-    :rtype: :class:`tuple`
 
     Examples::
 
         >>> seconds_to_split(7800)
-        (0, 0, 0, 2, 10, 0)
+        Duration(years=0, months=0, days=0, hours=2, minutes=10, seconds=0)
         >>> seconds_to_split(143659)
-        (0, 0, 1, 15, 54, 19)
+        Duration(years=0, months=0, days=1, hours=15, minutes=54, seconds=19)
+
+    .. versionadded:: 7.1
+
+    .. versionchanged:: 8.0
+
+        This function returns a :class:`Duration` named tuple.
 
     """
     years, seconds_left = divmod(int(seconds), YEARS)
     months, seconds_left = divmod(seconds_left, MONTHS)
     days, seconds_left = divmod(seconds_left, DAYS)
     hours, seconds_left = divmod(seconds_left, HOURS)
     minutes, seconds_left = divmod(seconds_left, MINUTES)
 
-    return years, months, days, hours, minutes, seconds_left
+    return Duration(years, months, days, hours, minutes, seconds_left)
 
 
-def get_time_unit(years=0, months=0, days=0, hours=0, minutes=0, seconds=0):
+def get_time_unit(
+    years: int = 0,
+    months: int = 0,
+    days: int = 0,
+    hours: int = 0,
+    minutes: int = 0,
+    seconds: int = 0,
+) -> tuple[
+    tuple[int, str],
+    tuple[int, str],
+    tuple[int, str],
+    tuple[int, str],
+    tuple[int, str],
+    tuple[int, str],
+]:
     """Map a time in (y, m, d, h, min, s) to its labels.
 
-    :param int years: number of years
-    :param int months: number of months
-    :param int days: number of days
-    :param int hours: number of hours
-    :param int minutes: number of minutes
-    :param int seconds: number of seconds
+    :param years: number of years
+    :param months: number of months
+    :param days: number of days
+    :param hours: number of hours
+    :param minutes: number of minutes
+    :param seconds: number of seconds
     :return: a tuple of 2-value tuples, each for a time amount and its label
-    :rtype: :class:`tuple`
 
-    This helper function get a time split in years, months, days, hours,
+    This helper function takes a time split into years, months, days, hours,
     minutes, and seconds to return a tuple with the correct label for each
-    unit. The label is pluralized and account for zéro, one, and more than one
-    value per unit::
+    unit. The label is pluralized according to whether the value is zero, one,
+    or more than one::
 
         >>> get_time_unit(days=1, hours=15, minutes=54, seconds=19)
         (
             (0, 'years'),
             (0, 'months'),
             (1, 'day'),
             (15, 'hours'),
@@ -261,14 +355,16 @@
         )
 
     This function can be used with :func:`seconds_to_split`::
 
         >>> get_time_unit(*seconds_to_split(143659))
         # ... same result as the example above
 
+    .. versionadded:: 7.1
+
     .. note::
 
         This function always returns a tuple with **all** time units, even when
         their amount is 0 (which is their default value).
 
     """
     years_text = "year{}".format("s" if years != 1 else "")
@@ -284,20 +380,22 @@
         (days, days_text),
         (hours, hours_text),
         (minutes, minutes_text),
         (seconds, seconds_text),
     )
 
 
-def seconds_to_human(secs, granularity=2):
+def seconds_to_human(
+    secs: Union[datetime.timedelta, float, int],
+    granularity: int = 2,
+) -> str:
     """Format :class:`~datetime.timedelta` as a human-readable relative time.
 
     :param secs: time difference to format
-    :type secs: :class:`~datetime.timedelta` or integer
-    :param int granularity: number of time units to return (default to 2)
+    :param granularity: number of time units to return (default to 2)
 
     Inspiration for function structure from:
     https://gist.github.com/Highstaker/280a09591df4a5fb1363b0bbaf858f0d
 
     Examples::
 
         >>> seconds_to_human(65707200)
@@ -320,14 +418,15 @@
         >>> seconds_to_human(3672)  # 2 by default
         '1 hour, 1 minute ago'
         >>> seconds_to_human(3672, granularity=3)
         '1 hour, 1 minute, 12 seconds ago'
         >>> seconds_to_human(3672, granularity=1)
         '1 hour ago'
 
+    .. versionadded:: 7.0
     """
     if isinstance(secs, datetime.timedelta):
         secs = secs.total_seconds()
 
     future = False
     if secs < 0:
         future = True
@@ -345,8 +444,9 @@
             if value
         ][:granularity])
 
     if future is False:
         result += " ago"
     else:
         result = "in " + result
+
     return result
```

### Comparing `sopel-7.1.9/sopel/tools/web.py` & `sopel-8.0.0/sopel/tools/web.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,31 @@
-# coding=utf-8
 """
 The ``tools.web`` package contains utility functions for interaction with web
 applications, APIs, or websites in your plugins.
 
 .. versionadded:: 7.0
-
-.. note::
-    Some parts of this module will remain accessible through ``sopel.web`` as
-    well until its final removal in Sopel 8. This is for backward
-    compatibility only; please update old code as soon as possible.
 """
 # Copyright © 2008, Sean B. Palmer, inamidst.com
 # Copyright © 2009, Michael Yanovich <yanovich.1@osu.edu>
 # Copyright © 2012, Dimitri Molenaars, Tyrope.nl.
 # Copyright © 2012-2013, Elad Alfassa, <elad@fedoraproject.org>
 # Copyright © 2019, dgw, technobabbl.es
 # Licensed under the Eiffel Forum License 2.
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import annotations
 
+import html
+from html.entities import name2codepoint
 import re
-import sys
 import urllib
+from urllib.parse import urlparse, urlunparse
 
 from sopel import __version__
+from sopel.lifecycle import deprecated
 
-if sys.version_info.major < 3:
-    from htmlentitydefs import name2codepoint
-    from urlparse import urlparse, urlunparse
-else:
-    from html.entities import name2codepoint
-    from urllib.parse import urlparse, urlunparse
-    unichr = chr
-    unicode = str
-
-try:
-    import html as HTMLLib
-except ImportError:
-    HTMLLib = None
 
 __all__ = [
     'USER_AGENT',
     'DEFAULT_HEADERS',
     'decode',
     'entity',
     'iri_to_uri',
@@ -94,92 +78,97 @@
 
        default_headers.update(custom_headers)
 
 """
 
 
 r_entity = re.compile(r'&([^;\s]+);')
-"""Regular expression to match HTML entities."""
+"""Regular expression to match HTML entities.
+
+.. deprecated:: 8.0
 
+    Will be removed in Sopel 9, along with :func:`entity`.
+"""
 
+
+@deprecated(
+    version='8.0',
+    removed_in='9.0',
+    reason="No longer needed now that Python 3.4+ has `html.unescape()`",
+)
 def entity(match):
     """Convert an entity reference to the appropriate character.
 
     :param str match: the entity name or code, as matched by
         :py:const:`r_entity`
     :return str: the Unicode character corresponding to the given ``match``
         string, or a fallback representation if the reference cannot be
         resolved to a character
+
+    .. deprecated:: 8.0
+
+        Will be removed in Sopel 9. Use :func:`decode` directly or migrate to
+        Python's standard-library equivalent, :func:`html.unescape`.
+
     """
     value = match.group(1).lower()
     if value.startswith('#x'):
-        return unichr(int(value[2:], 16))
+        return chr(int(value[2:], 16))
     elif value.startswith('#'):
-        return unichr(int(value[1:]))
+        return chr(int(value[1:]))
     elif value in name2codepoint:
-        return unichr(name2codepoint[value])
+        return chr(name2codepoint[value])
     return '[' + value + ']'
 
 
-def decode(html):
+def decode(text):
     """Decode HTML entities into Unicode text.
 
-    :param str html: the HTML page or snippet to process
-    :return str: ``html`` with all entity references replaced
-    """
-    if HTMLLib is not None:
-        # Python's stdlib has our back in 3.4+
-        # TODO: This should be the only implementation in Sopel 8
-        try:
-            return HTMLLib.unescape(html)
-        except AttributeError:
-            # Must be py3.3; fall through to our half-assed version.
-            pass
+    :param str text: the HTML page or snippet to process
+    :return str: ``text`` with all entity references replaced
 
-    # Not on py3.4+ yet? Then you get to deal with the jankiness.
-    return r_entity.sub(entity, html)
+    .. versionchanged:: 8.0
+
+        Renamed ``html`` parameter to ``text``. (Python gained a standard
+        library module named :mod:`html` in version 3.4.)
+
+    """
+    # TODO deprecated?
+    return html.unescape(text)
 
 
-# Identical to urllib2.quote
 def quote(string, safe='/'):
     """Safely encodes a string for use in a URL.
 
     :param str string: the string to encode
     :param str safe: a list of characters that should not be quoted; defaults
                      to ``'/'``
     :return str: the ``string`` with special characters URL-encoded
 
     .. note::
         This is a shim to make writing cross-compatible plugins for both
         Python 2 and Python 3 easier.
     """
-    if sys.version_info.major < 3:
-        if isinstance(string, unicode):
-            string = string.encode('utf8')
-        string = urllib.quote(string, safe.encode('utf8'))
-    else:
-        string = urllib.parse.quote(str(string), safe)
-    return string
+    # TODO deprecated?
+    return urllib.parse.quote(str(string), safe)
 
 
 # six-like shim for Unicode safety
 def unquote(string):
     """Decodes a URL-encoded string.
 
     :param str string: the string to decode
     :return str: the decoded ``string``
 
     .. note::
-        This is a shim to make writing cross-compatible plugins for both
-        Python 2 and Python 3 easier.
+
+        This is a convenient shortcut for ``urllib.parse.unquote``.
     """
-    if sys.version_info.major < 3:
-        return urllib.unquote(string.encode('utf-8')).decode('utf-8')
-    else:
-        return urllib.parse.unquote(string)
+    # TODO deprecated?
+    return urllib.parse.unquote(string)
 
 
 def quote_query(string):
     """Safely encodes a URL's query parameters.
 
     :param str string: a URL containing query parameters
     :return str: the input URL with query parameter values URL-encoded
@@ -189,53 +178,47 @@
     return string
 
 
 # Functions for international domain name magic
 
 def urlencode_non_ascii(b):
     """Safely encodes non-ASCII characters in a URL."""
-    regex = '[\x80-\xFF]'
-    if sys.version_info.major > 2:
-        regex = b'[\x80-\xFF]'
-    return re.sub(regex, lambda c: '%%%02x' % ord(c.group(0)), b)
+    return re.sub(b'[\x80-\xFF]', lambda c: b'%%%02x' % ord(c.group(0)), b)
 
 
 def iri_to_uri(iri):
     """Decodes an internationalized domain name (IDN)."""
     parts = urlparse(iri)
-    parts_seq = (part.encode('idna') if parti == 1 else urlencode_non_ascii(part.encode('utf-8')) for parti, part in enumerate(parts))
-    if sys.version_info.major > 2:
-        parts_seq = list(parts_seq)
-
+    parts_seq = list(
+        part.encode('idna')
+        if parti == 1 else urlencode_non_ascii(part.encode('utf-8'))
+        for parti, part in enumerate(parts)
+    )
     parsed = urlunparse(parts_seq)
-    if sys.version_info.major > 2:
-        return parsed.decode()
-    else:
-        return parsed
+    return parsed.decode()
 
 
-if sys.version_info.major < 3:
-    urlencode = urllib.urlencode
-else:
-    urlencode = urllib.parse.urlencode
+# direct shortcut kept for backward compatibility reasons
+# TODO consider removing this
+urlencode = urllib.parse.urlencode
 
 
 # Functions for URL detection
 
 def trim_url(url):
     """Removes extra punctuation from URLs found in text.
 
     :param str url: the raw URL match
     :return str: the cleaned URL
 
     This function removes trailing punctuation that looks like it was not
     intended to be part of the URL:
 
-        * trailing sentence- or clause-ending marks like ``.``, ``;``, etc.
-        * unmatched trailing brackets/braces like ``}``, ``)``, etc.
+    * trailing sentence- or clause-ending marks like ``.``, ``;``, etc.
+    * unmatched trailing brackets/braces like ``}``, ``)``, etc.
 
     It is intended for use with the output of :py:func:`~.search_urls`, which
     may include trailing punctuation when used on input from chat.
     """
     # clean trailing sentence- or clause-ending punctuation
     while url[-1] in '.,?!\'":;':
         url = url[:-1]
@@ -272,15 +255,15 @@
         re_url = r'((?<!%s)(?:%s)(?::\/\/\S+))' % (
             exclusion_char, schemes_patterns)
 
     r = re.compile(re_url, re.IGNORECASE | re.UNICODE)
 
     urls = re.findall(r, text)
     if clean:
-        urls = (trim_url(url) for url in urls)
+        urls = [trim_url(url) for url in urls]
 
     # yield unique URLs in their order of appearance
     seen = set()
     for url in urls:
         try:
             url = iri_to_uri(url)
         except Exception:  # TODO: Be specific
```

### Comparing `sopel-7.1.9/sopel/trigger.py` & `sopel-8.0.0/sopel/trigger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,63 @@
-# coding=utf-8
-"""Triggers are how Sopel tells callables about their runtime context."""
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""Triggers are how Sopel tells callables about their runtime context.
 
-import datetime
+A :class:`~.trigger.Trigger` is the main type of user input plugins will see.
+
+Sopel uses :class:`~.trigger.PreTrigger`\\s internally while processing
+incoming IRC messages. Plugin authors can reasonably expect that their code
+will never receive one. They are documented here for completeness, and for the
+aid of Sopel's core development.
+"""
+from __future__ import annotations
+
+from datetime import datetime, timezone
 import re
-import sys
+from typing import (
+    cast,
+    Match,
+    Optional,
+    Sequence,
+    TYPE_CHECKING,
+)
 
 from sopel import formatting, tools
 from sopel.tools import web
+from sopel.tools.identifiers import Identifier, IdentifierFactory
+
+if TYPE_CHECKING:
+    from sopel import config
 
 
 __all__ = [
     'PreTrigger',
     'Trigger',
 ]
 
-if sys.version_info.major >= 3:
-    unicode = str
-    basestring = str
+COMMANDS_WITH_CONTEXT = frozenset({
+    'INVITE',
+    'JOIN',
+    'KICK',
+    'MODE',
+    'NOTICE',
+    'PART',
+    'PRIVMSG',
+    'TOPIC',
+})
+"""Set of commands with a :attr:`trigger.sender<Trigger.sender>`.
+
+Most IRC messages a plugin will want to handle (channel messages and PMs) are
+associated with a context, exposed in the Trigger's ``sender`` property.
+However, not *all* commands can be directly associated to a channel or nick.
+
+For IRC message types other than those listed here, the ``trigger``\'s
+``sender`` property will be ``None``.
+"""
 
 
-class PreTrigger(object):
+class PreTrigger:
     """A parsed raw message from the server.
 
     :param str own_nick: the bot's own IRC nickname
     :param str line: the full line from the server
     :param tuple url_schemes: allowed schemes for URL detection
 
     At the :class:`PreTrigger` stage, the line has not been matched against any
@@ -38,14 +71,18 @@
 
     .. py:attribute:: args
 
         The IRC command's arguments.
 
         These are split on spaces, per the IRC protocol.
 
+    .. py:attribute:: ctcp
+
+        The CTCP command name, if present (``None`` otherwise)
+
     .. py:attribute:: event
 
         The IRC command name or numeric value.
 
         See :class:`sopel.tools.events` for a built-in mapping of names to
         numeric values.
 
@@ -65,14 +102,22 @@
 
         The nickname that sent this command.
 
     .. py:attribute:: sender
 
         Channel name or query where this message was received.
 
+        .. warning::
+
+            The ``sender`` Will be ``None`` for commands that have no implicit
+            channel or private-message context, for example AWAY or QUIT.
+
+            The :attr:`COMMANDS_WITH_CONTEXT` attribute lists IRC commands for
+            which ``sender`` can be relied upon.
+
     .. py:attribute:: tags
 
         Any IRCv3 message tags attached to the line, as a :class:`dict`.
 
     .. py:attribute:: text
 
         The last argument of the IRC command.
@@ -97,50 +142,69 @@
     .. py:attribute:: time
 
         The time when the message was received.
 
         If the IRC server sent a message tag indicating when *it* received the
         message, that is used instead of the time when Sopel received it.
 
+        .. versionchanged:: 8.0
+            Now a timezone-aware ``datetime`` object.
+
     .. py:attribute:: user
 
         The sender's local username.
 
     """
     component_regex = re.compile(r'([^!]*)!?([^@]*)@?(.*)')
-    intent_regex = re.compile('\x01(\\S+) ?(.*)\x01')
+    ctcp_regex = re.compile('\x01(\\S+) ?(.*)\x01')
 
-    def __init__(self, own_nick, line, url_schemes=None):
+    def __init__(
+        self,
+        own_nick: Identifier,
+        line: str,
+        url_schemes: Optional[Sequence] = None,
+        identifier_factory: IdentifierFactory = Identifier,
+        statusmsg_prefixes: tuple[str, ...] = tuple(),
+    ):
+        self.make_identifier: IdentifierFactory = identifier_factory
         line = line.strip('\r\n')
-        self.line = line
-        self.urls = tuple()
-        self.plain = ''
+        self.line: str = line
+        self.urls: tuple[str, ...] = tuple()
+        self.plain: str = ''
+        self.ctcp: Optional[str] = None
 
         # Break off IRCv3 message tags, if present
-        self.tags = {}
+        self.tags: dict[str, Optional[str]] = {}
         if line.startswith('@'):
             tagstring, line = line.split(' ', 1)
-            for tag in tagstring[1:].split(';'):
-                tag = tag.split('=', 1)
+            for raw_tag in tagstring[1:].split(';'):
+                tag = raw_tag.split('=', 1)
                 if len(tag) > 1:
                     self.tags[tag[0]] = tag[1]
                 else:
                     self.tags[tag[0]] = None
 
-        self.time = datetime.datetime.utcnow()
+        # Client time or server time
+        self.time = datetime.now(timezone.utc)
         if 'time' in self.tags:
+            # ensure "time" is a string (typecheck)
+            tag_time = self.tags['time'] or ''
             try:
-                self.time = datetime.datetime.strptime(self.tags['time'], '%Y-%m-%dT%H:%M:%S.%fZ')
+                self.time = datetime.strptime(
+                    tag_time,
+                    "%Y-%m-%dT%H:%M:%S.%fZ",
+                ).replace(tzinfo=timezone.utc)
             except ValueError:
                 pass  # Server isn't conforming to spec, ignore the server-time
 
         # Grabs hostmask from line.
         # Example: line = ':Sopel!foo@bar PRIVMSG #sopel :foobar!'
         #          print(hostmask)  # Sopel!foo@bar
         # All lines start with ":" except PING.
+        self.hostmask: Optional[str]
         if line.startswith(':'):
             self.hostmask, line = line[1:].split(' ', 1)
         else:
             self.hostmask = None
 
         # Parses the line into a list of arguments.
         # Some events like MODE don't have a secondary string argument, i.e. no ' :' inside the line.
@@ -153,41 +217,51 @@
         #             print(args)    # ['irc.libera.chat', 'MODE', 'Sopel', '+i']
         if ' :' in line:
             argstr, self.text = line.split(' :', 1)
             self.args = argstr.split(' ')
             self.args.append(self.text)
         else:
             self.args = line.split(' ')
-            self.text = self.args[-1]
+            # see `text` attr documentation above, and #2360
+            self.text = self.args[-1] if len(self.args) > 1 else ''
 
         self.event = self.args[0]
         self.args = self.args[1:]
-        components = PreTrigger.component_regex.match(self.hostmask or '').groups()
-        self.nick, self.user, self.host = components
-        self.nick = tools.Identifier(self.nick)
-
-        # If we have arguments, the first one is the sender
-        # Unless it's a QUIT event
-        if self.args and self.event != 'QUIT':
-            target = tools.Identifier(self.args[0])
-        else:
-            target = None
 
-        # Unless we're messaging the bot directly, in which case that second
-        # arg will be our bot's name.
-        if target and target.lower() == own_nick.lower():
-            target = self.nick
+        # The regex will always match any string, even an empty one
+        components_match = cast(
+            Match, PreTrigger.component_regex.match(self.hostmask or ''))
+        nick, self.user, self.host = components_match.groups()
+        self.nick: Identifier = self.make_identifier(nick)
+
+        # If we have arguments, the first one is *usually* the sender,
+        # most numerics and certain general events (e.g. QUIT) excepted
+        target: Optional[Identifier] = None
+        status_prefix: Optional[str] = None
+
+        if self.args and self.event in COMMANDS_WITH_CONTEXT:
+            raw_target = self.args[0]
+            if statusmsg_prefixes and raw_target[0] in statusmsg_prefixes:
+                status_prefix, raw_target = raw_target[0], raw_target[1:]
+            target = self.make_identifier(raw_target)
+
+            # Unless we're messaging the bot directly, in which case that
+            # second arg will be our bot's name.
+            if target.lower() == own_nick.lower():
+                target = self.nick
+
         self.sender = target
+        self.status_prefix = status_prefix
 
-        # Parse CTCP into a form consistent with IRCv3 intents
+        # Parse CTCP
         if self.event == 'PRIVMSG' or self.event == 'NOTICE':
-            intent_match = PreTrigger.intent_regex.match(self.args[-1])
-            if intent_match:
-                intent, message = intent_match.groups()
-                self.tags['intent'] = intent
+            ctcp_match = PreTrigger.ctcp_regex.match(self.args[-1])
+            if ctcp_match is not None:
+                ctcp, message = ctcp_match.groups()
+                self.ctcp = ctcp
                 self.args[-1] = message or ''
 
             # Search URLs after CTCP parsing
             self.urls = tuple(
                 web.search_urls(self.args[-1], schemes=url_schemes))
 
         # Populate account from extended-join messages
@@ -196,15 +270,15 @@
             self.tags['account'] = self.args[1]
 
         # get plain text message
         if self.args:
             self.plain = formatting.plain(self.args[-1])
 
 
-class Trigger(unicode):
+class Trigger(str):
     """A line from the server, which has matched a callable's rules.
 
     :param config: Sopel's current configuration settings object
     :type config: :class:`~sopel.config.Config`
     :param message: the message that matched the callable
     :type message: :class:`PreTrigger`
     :param match: what *in* the message matched
@@ -218,32 +292,70 @@
 
     The ``match`` is based on the matching regular expression rule; Sopel's
     command decorators auto-generate rules containing specific numbered groups
     that are documented separately. (See :attr:`group` below.)
 
     Note that CTCP messages (``PRIVMSG``\\es and ``NOTICE``\\es which start
     and end with ``'\\x01'``) will have the ``'\\x01'`` bytes stripped, and
-    the command (e.g. ``ACTION``) placed mapped to the ``'intent'`` key in
-    :attr:`Trigger.tags`.
+    :attr:`trigger.ctcp <ctcp>` will contain the command (e.g. ``ACTION``).
+
+    .. note::
+
+        CTCP used to be stored as the ``intent`` tag. Since message intents
+        never made it past the IRCv3 draft stage, Sopel dropped support for
+        them in Sopel 8.
+
     """
     sender = property(lambda self: self._pretrigger.sender)
     """Where the message arrived from.
 
-    :type: :class:`~.tools.Identifier`
+    :type: :class:`~sopel.tools.identifiers.Identifier`
 
     This will be a channel name for "regular" (channel) messages, or the nick
     that sent a private message.
 
     You can check if the trigger comes from a channel or a nick with its
-    :meth:`~sopel.tools.Identifier.is_nick` method::
+    :meth:`~sopel.tools.identifiers.Identifier.is_nick` method::
 
         if trigger.sender.is_nick():
             # message sent from a private message
         else:
             # message sent from a channel
+
+    .. important::
+
+        If the message was sent to a `specific status prefix`__, the ``sender``
+        does not include the status prefix. Be sure to use the
+        :attr:`status_prefix` when replying.
+
+        Note that the ``bot`` argument passed to plugin callables is a
+        :class:`~sopel.bot.SopelWrapper` that handles this for the default
+        ``destination`` of the methods it overrides (most importantly,
+        :meth:`~sopel.bot.SopelWrapper.say` &
+        :meth:`~sopel.bot.SopelWrapper.reply`).
+
+    .. warning::
+
+        The ``sender`` Will be ``None`` for commands that have no implicit
+        channel or private-message context, for example AWAY or QUIT.
+
+        The :attr:`COMMANDS_WITH_CONTEXT` attribute lists IRC commands for
+        which ``sender`` can be relied upon.
+
+    .. __: https://modern.ircdocs.horse/#statusmsg-parameter
+    """
+    status_prefix = property(lambda self: self._pretrigger.status_prefix)
+    """The prefix used for the :attr:`sender` for status-specific messages.
+
+    :type: Optional[str]
+
+    This will be ``None`` by default. If a message is sent to a channel, it may
+    have a status prefix for status-specific messages. In that case, the prefix
+    is removed from the channel's identifier (see :attr:`sender`) and saved to
+    this attribute.
     """
     time = property(lambda self: self._pretrigger.time)
     """When the message was received.
 
     :type: naïve :class:`~datetime.datetime` object (no timezone)
 
     If the IRC server supports ``server-time``, :attr:`time` will give that
@@ -274,15 +386,15 @@
     """Local username of the person who sent the message.
 
     :type: str
     """
     nick = property(lambda self: self._pretrigger.nick)
     """The nickname who sent the message.
 
-    :type: :class:`~.tools.Identifier`
+    :type: :class:`~sopel.tools.identifiers.Identifier`
     """
     host = property(lambda self: self._pretrigger.host)
     """The hostname of the person who sent the message.
 
     :type: str
     """
     event = property(lambda self: self._pretrigger.event)
@@ -290,29 +402,30 @@
 
     :type: str
 
     Most plugin :func:`callables <callable>` primarily need to deal with
     ``PRIVMSG``. Other event types like ``NOTICE``, ``NICK``, ``TOPIC``,
     ``KICK``, etc. must be requested using :func:`.plugin.event`.
     """
-    ctcp = property(lambda self: self.tags.get('intent', None))
+    ctcp = property(lambda self: self._pretrigger.ctcp)
     """The CTCP command (if any).
 
     :type: str
 
     Common CTCP commands are ``ACTION``, ``VERSION``, and ``TIME``. Other
     commands include ``USERINFO``, ``PING``, and various ``DCC`` operations.
 
     .. versionadded:: 7.1
 
     .. important::
 
         Use this attribute instead of the ``intent`` tag in :attr:`tags`.
-        Message intents never made it past the IRCv3 draft stage, and Sopel will
-        drop support for them in a future release.
+        Message intents never made it past the IRCv3 draft stage, and Sopel
+        dropped support for them in Sopel 8.
+
     """
     match = property(lambda self: self._match)
     """The :ref:`Match object <match-objects>` for the triggering line.
 
     :type: :ref:`Match object <match-objects>`
     """
     group = property(lambda self: self._match.group)
@@ -407,32 +520,44 @@
 
     Note: This is only available if the ``account-tag`` capability or *both*
     the ``account-notify`` and ``extended-join`` capabilities are available on
     the connected IRC network. If this is not the case, or if the user sending
     the message isn't logged in to services, this property will be ``None``.
     """
 
-    def __new__(cls, config, message, match, account=None):
-        self = unicode.__new__(cls, message.args[-1] if message.args else '')
+    def __new__(
+        cls,
+        settings: config.Config,
+        message: PreTrigger,
+        match: Match,
+        account: Optional[str] = None,
+    ) -> 'Trigger':
+        return str.__new__(cls, message.args[-1] if message.args else '')
+
+    def __init__(
+        self,
+        settings: config.Config,
+        message: PreTrigger,
+        match: Match,
+        account: Optional[str] = None,
+    ) -> None:
         self._account = account
         self._pretrigger = message
         self._match = match
         self._is_privmsg = message.sender and message.sender.is_nick()
 
         def match_host_or_nick(pattern):
             pattern = tools.get_hostmask_regex(pattern)
             return bool(
                 pattern.match(self.nick) or
                 pattern.match('@'.join((self.nick, self.host)))
             )
 
-        if config.core.owner_account:
-            self._owner = config.core.owner_account == self.account
+        if settings.core.owner_account:
+            self._owner = settings.core.owner_account == self.account
         else:
-            self._owner = match_host_or_nick(config.core.owner)
+            self._owner = match_host_or_nick(settings.core.owner)
         self._admin = (
             self._owner or
-            self.account in config.core.admin_accounts or
-            any(match_host_or_nick(item) for item in config.core.admins)
+            self.account in settings.core.admin_accounts or
+            any(match_host_or_nick(item) for item in settings.core.admins)
         )
-
-        return self
```

### Comparing `sopel-7.1.9/sopel.egg-info/PKG-INFO` & `sopel-8.0.0/sopel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: sopel
-Version: 7.1.9
+Version: 8.0.0
 Summary: Simple and extensible IRC bot
-Home-page: https://sopel.chat/
-Author: dgw
-Author-email: dgw@technobabbl.es
-License: Eiffel Forum License, version 2
-Platform: Linux x86
-Platform: x86-64
+Author: dgw, Florian Strzelecki, Sean B. Palmer, Else Powell, Elad Alfassa, Dimitri Molenaars, Michael Yanovich
+Maintainer: dgw, Florian Strzelecki
+License: EFL-2.0
+Project-URL: Homepage, https://sopel.chat/
+Project-URL: Release notes, https://sopel.chat/changelog/
+Project-URL: Documentation, https://sopel.chat/docs/
+Project-URL: Bug Tracker, https://github.com/sopel-irc/sopel/issues
+Project-URL: Donate on Open Collective, https://opencollective.com/sopel
+Project-URL: Donate on GitHub, https://github.com/sponsors/sopel-irc
+Project-URL: Source, https://github.com/sopel-irc/sopel
+Project-URL: Coverage, https://coveralls.io/github/sopel-irc/sopel
+Platform: Linux x86, x86-64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,<4,>=2.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: COPYING
 
 =======
  Sopel
 =======
 
-|version| |build| |issues| |alerts| |coverage-status| |license|
+|version| |build| |issues| |coverage-status| |license|
 
 Introduction
 ------------
 
 Sopel is a simple, lightweight, open source, easy-to-use IRC Utility bot,
 written in Python. It's designed to be easy to use, run and extend.
 
@@ -53,25 +55,18 @@
 Failing both of those options, you can grab the latest tarball `from GitHub
 <https://github.com/sopel-irc/sopel/releases/latest>`_  and follow the steps
 for installing from the latest source below.
 
 Latest source
 =============
 First, either clone the repository with ``git clone
-git://github.com/sopel-irc/sopel.git`` or download a tarball `from GitHub
-<https://github.com/sopel-irc/sopel/releases/latest>`_.
+https://github.com/sopel-irc/sopel.git`` or download a `source archive from
+GitHub <https://github.com/sopel-irc/sopel/archive/refs/heads/master.zip>`_.
 
-Note: Sopel requires Python 2.7.x or Python 3.3+ to run. On Python 2.7,
-Sopel requires ``backports.ssl_match_hostname`` to be installed. Use
-``pip install backports.ssl_match_hostname`` or
-``yum install python-backports.ssl_match_hostname`` to install it, or download
-and install it manually `from PyPI <https://pypi.org/project/backports.ssl_match_hostname>`_.
-
-Important: Sopel 8.0 will drop support for many old Python versions,
-including Python 2.7!
+Note: Sopel requires Python 3.8+ to run.
 
 In the source directory (whether cloned or from the tarball) run ``pip install
 -e .``. You can then run ``sopel`` to configure and start the bot.
 
 Database support
 ----------------
 Sopel leverages SQLAlchemy to support the following database types: SQLite,
@@ -125,19 +120,15 @@
 `Netlify <https://www.netlify.com/>`_, but we are considering building a few
 new features that would require more than static hosting. All project-related
 `expenses <https://opencollective.com/sopel/expenses>`_ are tracked on our
 Open Collective profile, for transparency.
 
 .. |version| image:: https://img.shields.io/pypi/v/sopel.svg
    :target: https://pypi.python.org/pypi/sopel
-.. |build| image:: https://travis-ci.org/sopel-irc/sopel.svg?branch=master
-   :target: https://travis-ci.org/sopel-irc/sopel
+.. |build| image:: https://github.com/sopel-irc/sopel/actions/workflows/ci.yml/badge.svg?branch=master&event=push
+   :target: https://github.com/sopel-irc/sopel/actions/workflows/ci.yml?query=branch%3Amaster+event%3Apush
 .. |issues| image:: https://img.shields.io/github/issues/sopel-irc/sopel.svg
    :target: https://github.com/sopel-irc/sopel/issues
-.. |alerts| image:: https://img.shields.io/lgtm/alerts/g/sopel-irc/sopel.svg
-   :target: https://lgtm.com/projects/g/sopel-irc/sopel/alerts/
 .. |coverage-status| image:: https://coveralls.io/repos/github/sopel-irc/sopel/badge.svg?branch=master
    :target: https://coveralls.io/github/sopel-irc/sopel?branch=master
 .. |license| image:: https://img.shields.io/pypi/l/sopel.svg
    :target: https://github.com/sopel-irc/sopel/blob/master/COPYING
-
-
```

