# Comparing `tmp/bttc-0.0.80.tar.gz` & `tmp/bttc-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.80.tar", last modified: Sat May 25 14:30:25 2024, max compression
+gzip compressed data, was "bttc-0.0.81.tar", last modified: Sun Jun  2 07:21:54 2024, max compression
```

## Comparing `bttc-0.0.80.tar` & `bttc-0.0.81.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.463412 bttc-0.0.80/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.80/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2751 2024-05-25 14:30:25.463412 bttc-0.0.80/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2023 2024-05-25 14:30:11.000000 bttc-0.0.80/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-05-25 14:29:31.000000 bttc-0.0.80/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    10830 2024-05-19 04:05:38.000000 bttc-0.0.80/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.80/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-05-20 14:07:40.000000 bttc-0.0.80/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.80/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.80/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    40032 2024-05-25 14:27:31.000000 bttc-0.0.80/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.451412 bttc-0.0.80/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9163 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7155 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.80/bttc/utils/device_factory.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/utils/dialer_simulator.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.80/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.80/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.80/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    17165 2024-05-19 04:05:38.000000 bttc-0.0.80/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2751 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-25 14:30:25.463412 bttc-0.0.80/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.80/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.536377 bttc-0.0.81/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.81/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2751 2024-06-02 07:21:54.536377 bttc-0.0.81/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2023 2024-05-28 02:15:37.000000 bttc-0.0.81/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.528377 bttc-0.0.81/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-06-02 07:21:44.000000 bttc-0.0.81/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    10830 2024-05-19 04:05:38.000000 bttc-0.0.81/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.81/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    14748 2024-06-02 07:18:44.000000 bttc-0.0.81/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.532377 bttc-0.0.81/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.81/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.81/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-11 11:42:51.000000 bttc-0.0.81/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    41973 2024-06-02 07:18:44.000000 bttc-0.0.81/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.532377 bttc-0.0.81/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.532377 bttc-0.0.81/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.528377 bttc-0.0.81/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.532377 bttc-0.0.81/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.532377 bttc-0.0.81/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9163 2024-05-11 11:42:51.000000 bttc-0.0.81/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7155 2024-05-11 11:42:51.000000 bttc-0.0.81/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.536377 bttc-0.0.81/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.81/bttc/utils/device_factory.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-11 11:42:51.000000 bttc-0.0.81/bttc/utils/dialer_simulator.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.536377 bttc-0.0.81/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.81/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-11 11:42:51.000000 bttc-0.0.81/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.536377 bttc-0.0.81/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.81/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.536377 bttc-0.0.81/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.81/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    17165 2024-05-19 04:05:38.000000 bttc-0.0.81/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.81/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.81/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-06-02 07:21:54.532377 bttc-0.0.81/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2751 2024-06-02 07:21:54.000000 bttc-0.0.81/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-06-02 07:21:54.000000 bttc-0.0.81/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-06-02 07:21:54.000000 bttc-0.0.81/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-06-02 07:21:54.000000 bttc-0.0.81/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-06-02 07:21:54.000000 bttc-0.0.81/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-06-02 07:21:54.536377 bttc-0.0.81/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.81/setup.py
```

### Comparing `bttc-0.0.80/LICENSE` & `bttc-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/PKG-INFO` & `bttc-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.80
+Version: 0.0.81
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.80/README.md` & `bttc-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/__init__.py` & `bttc-0.0.81/bttc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.80'
+__version__ = '0.0.81'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.80/bttc/apk_utils.py` & `bttc-0.0.81/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/ble_data.py` & `bttc-0.0.81/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/ble_utils.py` & `bttc-0.0.81/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/bt_data.py` & `bttc-0.0.81/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/bt_utils.py` & `bttc-0.0.81/bttc/bt_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility to support common BT operations/methods."""
 import datetime
-import deprecation
 from functools import partial
 import logging
 import time
 
 from mobly.controllers import android_device
-from mobly.controllers.android_device_lib import adb
+import bttc
 from bttc import bt_data
 from bttc import common_data
 from bttc import constants
 from bttc import core
 from bttc.utils import device_factory
 from bttc.utils import log_parser
 
-import shlex
 import re
-from typing import Any, Callable, Sequence, TypeAlias, Union
+from typing import Any, Sequence, TypeAlias, Union
 
 
 BINDING_KEYWORD = 'bt'
 AUTO_LOAD = True
 ANDROID_DEVICE: TypeAlias = android_device.AndroidDevice
 BT_BONDED_STATE: TypeAlias = constants.BluetoothBondedState
 BT_PAIRED_DEVICE: TypeAlias = bt_data.PairedDeviceInfo
@@ -66,15 +64,15 @@
     self._bind(get_device_mac_by_name)
     self._bind(get_connected_ble_devices)
     self._bind(get_current_le_audio_active_group_id)
     self._bind(is_le_audio_device_connected)
     self._bind(is_bluetooth_enabled, 'is_enabled')
     self._bind(list_paired_devices)
     self._bind(unbond_device)
-    self.shell = safe_adb_shell(ad)
+    self.shell = bttc.safe_adb_shell(ad)
     self.enable = partial(toggle_bluetooth, ad=ad, enabled=True)
     self.disable = partial(toggle_bluetooth, ad=ad, enabled=False)
 
   @property
   def enabled(self):
     return self.is_enabled()
 
@@ -393,78 +391,29 @@
         map(lambda paired_info: paired_info['Name'], paired_devices))
 
   return [
       bt_data.PairedDeviceInfo.from_dict(pair_info_dict)
       for pair_info_dict in paired_devices]
 
 
-@deprecation.deprecated(
-    deprecated_in='0.0.75.x',
-    removed_in='0.0.77.x',
-    details=(
-        'This function is soon to be expired. '
-        'Please use `bttc.safe_adb_shell` instead'))
-def safe_adb_shell(
-    device: android_device.AndroidDevice,
-    use_shlex_split: bool = True,
-    timeout: float | None = None) -> Callable[[str], tuple[str, str, int]]:
-  """Gets safe adb shell executor.
-
-  Below is demo of this function:
-  ```python
-  >>> from bttc import bt_utils
-  >>> from mobly.controllers import android_device
-  >>> phone = android_device.create([{'serial': '07311JECB08252'}])[0]
-  >>> safe_adb = bt_utils.safe_adb_shell(phone)
-  >>> stdout, stderr, rt = safe_adb('getprop ro.build.version.sdk')
-  >>> stdout  # My phone is of SDK 30.
-  '30\n'
-  ```
-
-  Args:
-    device: Adb like device.
-    use_shlex_split: Leverage shlex.split iff True.
-    timeout: float, the number of seconds to wait before timing out. If not
-      specified, no timeout takes effect.
-
-  Returns:
-    Safe callable adb object.
-  """
-
-  def _adb_wrapper(command: str) -> tuple[str, str, int]:
-    try:
-      command = shlex.split(command) if use_shlex_split else command
-      command_output = device.adb.shell(command, timeout=timeout).decode()
-      return (command_output, '', 0)
-    except adb.AdbError as err:
-      return (err.stdout.decode(encoding='utf-8', errors='strict'),
-              err.stderr.decode(encoding='utf-8',
-                                errors='strict'), err.ret_code)
-    except adb.AdbTimeoutError as err:
-      device.log.warning('Timeout in executing command: %s', command)
-      return ('', str(err), -1)
-
-  return _adb_wrapper
-
-
 def toggle_bluetooth(
     ad: android_device.AndroidDevice, enabled: bool = True) -> None:
   """Enables or disables Bluetooth on an Android device.
 
   Args:
     ad: The Android device object.
     enabled: True to enable Bluetooth, False to disable it.
 
   RuntimeError: If Bluetooth could not be toggled successfully. The error
       message includes the attempted state ('enabled' or 'disabled'),
       return code, and command output for troubleshooting.
   """
   status = 'enable' if enabled else 'disable'
   cmd = f'svc bluetooth {status}'
-  stdout, _, ret_code = safe_adb_shell(ad)(cmd)
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(cmd)
   stdout = stdout.strip()
   # Expect 'disable: Success' or 'enable: Success'
   if ret_code == 0 and any([
       'Success' in stdout,
       stdout in {
           'Enabling Bluetooth',  # BDS's output
           '',  # SDK version < 33 (b/297539822#comment4)
```

### Comparing `bttc-0.0.80/bttc/cli/__init__.py` & `bttc-0.0.81/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/cli/constants.py` & `bttc-0.0.81/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/cli/main.py` & `bttc-0.0.81/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/common_data.py` & `bttc-0.0.81/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/constants.py` & `bttc-0.0.81/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/core.py` & `bttc-0.0.81/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/errors.py` & `bttc-0.0.81/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/general_data.py` & `bttc-0.0.81/bttc/general_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/general_utils.py` & `bttc-0.0.81/bttc/general_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import dataclasses
 import datetime
 from functools import cache
 import logging
 import os
 import re
 import sys
+from typing import Protocol
 from subprocess import Popen, PIPE
 import time
 
 import bttc
-from bttc import bt_utils
 from bttc import constants
 from bttc import core
 from bttc import errors
 from bttc import general_data
 from bttc.cli.constants import warning
 from bttc.profiles.hfp import hfp_data
 from bttc.utils import device_factory
@@ -55,15 +55,15 @@
 
 _ActivityRecord = general_data.ActivityRecord
 
 # Default timeout for adb shell command.
 _ADB_SHELL_TIMEOUT_SEC = constants.ADB_SHELL_TIMEOUT_SEC
 
 # Logcat message timestamp format
-_DATETIME_FMT = constants.LOGCAT_DATETIME_FMT
+_LOGCAT_DATETIME_FMT = constants.LOGCAT_DATETIME_FMT
 
 # Pattern to match message of logcat service.
 _LOGCAT_MSG_PATTERN = constants.LOGTCAT_MSG_PATTERN
 
 # Command to retrieve SDK information.
 _CMD_GET_SDK_VERSION = "getprop ro.build.version.sdk"
 
@@ -170,15 +170,15 @@
         'device_config get_sync_disabled_for_tests').decode().strip()
     self._sync_disabled_for_tests = shell_output
     return self._sync_disabled_for_tests
 
   @sync_disabled_for_tests.setter
   def sync_disabled_for_tests(self, value: str):
     value = value.strip()
-    stdout, _, ret_code = bt_utils.safe_adb_shell(self._ad)(
+    stdout, _, ret_code = bttc.safe_adb_shell(self._ad)(
         f"device_config set_sync_disabled_for_tests {value}")
 
     if ret_code != 0:
       self._ad.log.error(
           'Failed to set "sync_disabled_for_tests" with value="%s"', value)
       raise adb.Error(f'Stdout: {stdout} (rt={ret_code})')
 
@@ -345,76 +345,102 @@
       """Iterates the settings of current namespace."""
       return Settings.Namespace.SettingIter(
           self._ad.adb.shell(f"settings list {self._namespace}")
               .decode()
               .split("\n"))
 
 
-class LogcatSearchStrategy:
-  """Logcat searching strategy."""
+class LogcatSearchStrategy(Protocol):
+  """Logcat searching strategy.
 
-  def __init__(self, interested_ts: str, log_pattern: str):
+  Attributes:
+    log_pattern: Log pattern to search in logcat messages.
+    start_device_time: Begin time to start searching.
+    stop: True means the searching is completed.
+  """
+
+  def __init__(self, begin_device_time: str, log_pattern: str):
     try:
-      self._start_time_conv = datetime.datetime.strptime(
-          interested_ts, _DATETIME_FMT)
+      self._start_device_time = datetime.datetime.strptime(
+          begin_device_time, _LOGCAT_DATETIME_FMT)
     except ValueError as ex:
-      logging.error('Invalid time format = "%s"!', interested_ts)
+      logging.error('Invalid device time as "%s"!', begin_device_time)
       raise ex
 
     self._log_pattern = log_pattern
     self._stop = False
-    self._regex_logcat_time = re.compile(
-      r'(?P<datetime>[\d]{2}-[\d]{2} [\d]{2}:[\d]{2}:[\d]{2}.[\d]{3})')
+
+  @property
+  def log_pattern(self) -> str:
+    """Log pattern to search in logcat messages."""
+    return self._log_pattern
+
+  @property
+  def start_device_time(self) -> datetime.datetime:
+    """The device time to start searching."""
+    return self._start_device_time
 
   @property
   def stop(self) -> bool:
+    """True means the searching is done."""
     return self._stop
 
   def search(self, line: str) -> str:
+    """Matches the input line to checks if it is wanted."""
     ...
 
 
 class LogcatSearchToEnd(LogcatSearchStrategy):
+  """Searches logcat message with given pattern until the last line."""
 
   def search(self, line: str) -> str:
-    match = self._regex_logcat_time.match(line)
+    matcher = _LOGCAT_MSG_PATTERN.match(line)
     post_start_time = False
-    if match:
-      if (datetime.datetime.strptime(
-          match.group('datetime'), _DATETIME_FMT) >= self._start_time_conv):
+    if matcher:
+      log_device_time = datetime.datetime.strptime(
+          matcher.group('datetime'), _LOGCAT_DATETIME_FMT)
+      if not post_start_time and log_device_time >= self.start_device_time:
         post_start_time = True
 
       if (
           post_start_time and
-          re.search(self._log_pattern, line) is not None):
+          re.search(self.log_pattern, line) is not None):
         return line
 
-      return ''
+    return ''
 
 
 class LogcatSearchAfter(LogcatSearchStrategy):
-  def __init__(self, interested_ts: str):
-    super().__init__(interested_ts, '')
+  """Searches logcat message after given device time."""
+
+  def __init__(self, begin_device_time: str):
+    super().__init__(
+        begin_device_time=begin_device_time,
+        log_pattern='')
 
   def search(self, line: str) -> str:
-    match = self._regex_logcat_time.match(line)
-    if match:
-      if (datetime.datetime.strptime(
-          match.group('datetime'), _DATETIME_FMT) >= self._start_time_conv):
+    matcher = _LOGCAT_MSG_PATTERN.match(line)
+    if matcher:
+      log_device_time = datetime.datetime.strptime(
+          matcher.group('datetime'), _LOGCAT_DATETIME_FMT)
+      if log_device_time >= self.start_device_time:
         return line
+
     return ''
 
 
 class LogcatSearchUntil(LogcatSearchStrategy):
 
   def search(self, line: str) -> str:
-    match = self._regex_logcat_time.match(line)
-    if match:
-      if (datetime.datetime.strptime(
-          match.group('datetime'), _DATETIME_FMT) > self._start_time_conv):
+    matcher = _LOGCAT_MSG_PATTERN.match(line)
+    if matcher:
+      log_device_time = datetime.datetime.strptime(
+          matcher.group('datetime'), _LOGCAT_DATETIME_FMT)
+
+      if log_device_time > self.start_device_time:
         self._stop = True
         return ''
 
       if re.search(self._log_pattern, line):
         return line
 
     return ''
@@ -448,19 +474,20 @@
     self._bind(get_all_volume)
     self._bind(get_volume)
     self._bind(is_apk_installed)
     self._bind(logcat_filter)
     self.props = Props(self._ad)
     self._bind(push_file)
     self._bind(push_non_persistent_property)
+    self._bind(search_logcat_after)
     self._bind(settings_get)
     self._bind(settings_put)
     self._bind(set_volume)
     self.settings = Settings(self._ad)
-    self.shell = bt_utils.safe_adb_shell(ad)
+    self.shell = bttc.safe_adb_shell(ad)
     self._bind(take_screenshot)
 
   @property
   def airplane_mode(self) -> bool:
     """Gets the current airplane mode status of the device.
 
     Returns:
@@ -773,15 +800,15 @@
 
   Returns:
     The corresponding setting value.
 
   Raises:
     adb.Error: Fail to get setting from given namespace.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(
       f"device_config get {namespace} {setting}"
   )
   if ret_code != 0:
     raise adb.Error(
         f"Failed to retrieve setting={setting} (rt={ret_code}): "
         f'{stdout or "?"}')
 
@@ -797,15 +824,15 @@
 
   Returns:
     All settings of given namespace.
 
   Raises:
     adb.Error: Fail to list settings of given device_config namespace.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(
       f"device_config list {namespace}")
   if ret_code != 0:
     raise adb.Error(
         'Failed to retrieve settings of device_config '
         f'namespace={namespace} (rt={ret_code}): {stdout or "?"}'
     )
 
@@ -820,15 +847,15 @@
 
   Returns:
     List of device_config namespace.
 
   Raises:
     adb.Error: Fail to list device_config namespaces.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(
       'device_config list_namespaces')
   if ret_code != 0:
     raise adb.Error(
         f'Failed to retrieve namespaces of device_config (rt={ret_code}): '
         f'{stdout or "?"}'
     )
 
@@ -844,15 +871,15 @@
     ad: Adb like device.
     namespace: Namespace to process.
     setting: The setting name.
 
   Raises:
     adb.Error: Fail to put device_config setting.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(
       f"device_config put {namespace} {setting} {value}")
   if ret_code != 0:
     raise adb.Error(
         f'Failed to put "{setting}={value}" in namespace={namespace}'
         f'(rt={ret_code}): {stdout or "?"}'
     )
 
@@ -1034,15 +1061,15 @@
 
   if not ui_xml_content:
     ad.log.warning('Failed to retrieve UI xml from uiautomator!')
     ad.log.info('Trying `uiautomator dump`...')
     ad.adb.shell(
         f'test -f {internal_dump_xml_path} && rm {internal_dump_xml_path}'
         " || echo 'no need to clean exist dumped xml file'")
-    shell_obj = bt_utils.safe_adb_shell(ad)
+    shell_obj = bttc.safe_adb_shell(ad)
 
     last_rt = 0
     last_message = None
     for retry_num in range(5):
       shell_obj('uiautomator dump')
       stdout, stderr, rt = shell_obj(f'test -f {internal_dump_xml_path}')
       if rt != 0:
@@ -1085,15 +1112,15 @@
 
   Args:
     ad: Device to retrieve volume setting.
 
   Returns:
     The settings of all audio volume types with key as name; value as settings.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)('dumpsys audio')
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)('dumpsys audio')
 
   if ret_code != 0:
     raise adb.Error(
         f'Failed to get volume with stdout: {stdout} (rt={ret_code})')
 
   return log_parser.parse_audio_dump_for_volume_info(stdout)
 
@@ -1185,27 +1212,27 @@
   >>> device_time = dut.gm.device_time
   >>> # Conduct pairing with headset from DUT
   >>> dut.gm.logcat_filter(device_time, 'BOND_BONDING => BOND_BONDED')
   '...'
   ```
 
   Args:
-    start_time: start time in string format of `_DATETIME_FMT`.
+    start_time: start time in string format of `_LOGCAT_DATETIME_FMT`.
     text_filter: only return logcat lines that include this string or regex.
 
   Returns:
     A logcat output.
 
   Raises:
     ValueError Exception if start_time is invalid format.
   """
   searching_uitl_now = False
   if not start_time:
     searching_uitl_now = True
-    start_time = datetime.datetime.now().strftime(_DATETIME_FMT)
+    start_time = datetime.datetime.now().strftime(_LOGCAT_DATETIME_FMT)
 
   logcat_response = ''
   search_strategy = (
       LogcatSearchUntil(start_time, text_filter) if searching_uitl_now
       else LogcatSearchToEnd(start_time, text_filter))
 
   with open(ad.adb_logcat_file_path, 'r', errors='replace') as logcat_file:
@@ -1289,14 +1316,47 @@
     ad.adb.shell("'chmod 644 /data/local.prop'", shell=True)
   except adb.AdbError as ex:
     ad.log.error(
         f'Failed to push persistent property="{property_name}": {ex}')
     raise ex
 
 
+def search_logcat_after(
+    ad: typing_utils.AdbDevice,
+    start_device_time: str,
+    search_pattern: str,
+) -> list[str]:
+  """Search the logcat message with given pattern and after given device time.
+
+  Args:
+    ad: Adb like object.
+    start_device_time: A string representing the device time (logcat timestamp
+      format) from which to start searching.
+    search_pattern: A regular expression or plain text string used to filter
+      logcat messages. Matching messages will be included in the results. If
+      empty string is given, all messages will be collected.
+
+  Returns:
+    List of collected logcat message.
+  """
+  search_strategy: LogcatSearchStrategy = (
+      LogcatSearchToEnd(start_device_time, search_pattern) if search_pattern
+      else LogcatSearchAfter(start_device_time))
+  collected_messages = []
+  with open(ad.adb_logcat_file_path, "r", errors="replace") as logcat_fo:
+    for line in logcat_fo:
+      if search_strategy.search(line):
+        collected_messages.append(line.rstrip())
+
+      if search_strategy.stop:
+        break
+
+  return collected_messages
+
+
 def settings_get(
     ad: typing_utils.AdbDevice, namespace: str, setting: str) -> str:
   """Gets setting from a given namespace in device's settings.
 
   Args:
     ad: Adb like device.
     namespace: Namespace to query for.
@@ -1304,15 +1364,15 @@
 
   Returns:
     The corresponding setting value.
 
   Raises:
     adb.Error: Fail to get setting from given namespace.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(
       f"settings get {namespace} {setting}"
   )
   if ret_code != 0:
     raise adb.Error(
         f"Failed to retrieve setting={setting} (rt={ret_code}): "
         f'{stdout or "?"}')
 
@@ -1328,15 +1388,15 @@
     ad: Adb like device.
     namespace: Namespace to process.
     setting: The setting name.
 
   Raises:
     adb.Error: Fail to put device_config setting.
   """
-  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+  stdout, _, ret_code = bttc.safe_adb_shell(ad)(
       f"settings put {namespace} {setting} {value}")
   if ret_code != 0:
     raise adb.Error(
         f'Failed to put "{setting}={value}" in namespace={namespace}'
         f'(rt={ret_code}): {stdout or "?"}'
     )
```

### Comparing `bttc-0.0.80/bttc/mc_data.py` & `bttc-0.0.81/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/mc_utils.py` & `bttc-0.0.81/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.81/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.81/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.81/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.81/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.81/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.81/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.81/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/avrcp/errors.py` & `bttc-0.0.81/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/__init__.py` & `bttc-0.0.81/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/constants.py` & `bttc-0.0.81/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/errors.py` & `bttc-0.0.81/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.81/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.81/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.81/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.81/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/strategy.py` & `bttc-0.0.81/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/ad_checker.py` & `bttc-0.0.81/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/device_factory.py` & `bttc-0.0.81/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/dialer_simulator.py` & `bttc-0.0.81/bttc/utils/dialer_simulator.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/iperf/__init__.py` & `bttc-0.0.81/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/iperf/errors.py` & `bttc-0.0.81/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/key_events_handler.py` & `bttc-0.0.81/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/log_parser.py` & `bttc-0.0.81/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/logcat.py` & `bttc-0.0.81/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.81/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.81/bttc/utils/media_player/yt_player_agent.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/retry.py` & `bttc-0.0.81/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/typing_utils.py` & `bttc-0.0.81/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.81/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/ui_pages/errors.py` & `bttc-0.0.81/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.81/bttc/utils/ui_pages/ui_core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.81/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils/ui_pages/utils.py` & `bttc-0.0.81/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/utils_loader.py` & `bttc-0.0.81/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc/wifi_utils.py` & `bttc-0.0.81/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/bttc.egg-info/PKG-INFO` & `bttc-0.0.81/bttc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.80
+Version: 0.0.81
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.80/bttc.egg-info/SOURCES.txt` & `bttc-0.0.81/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.80/setup.py` & `bttc-0.0.81/setup.py`

 * *Files identical despite different names*

