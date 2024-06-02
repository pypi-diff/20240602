# Comparing `tmp/qulab-2.1.0.tar.gz` & `tmp/qulab-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.1.0.tar", last modified: Fri May 31 15:59:31 2024, max compression
+gzip compressed data, was "qulab-2.1.1.tar", last modified: Sun Jun  2 15:41:24 2024, max compression
```

## Comparing `qulab-2.1.0.tar` & `qulab-2.1.1.tar`

### file list

```diff
@@ -1,109 +1,111 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.375771 qulab-2.1.0/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-31 15:58:55.000000 qulab-2.1.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-31 15:58:55.000000 qulab-2.1.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-31 15:59:31.375535 qulab-2.1.0/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.375213 qulab-2.1.0/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-31 15:58:55.000000 qulab-2.1.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-31 15:58:55.000000 qulab-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.363888 qulab-2.1.0/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.365343 qulab-2.1.0/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.367032 qulab-2.1.0/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    25698 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    29740 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.368025 qulab-2.1.0/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.368271 qulab-2.1.0/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.369595 qulab-2.1.0/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.370132 qulab-2.1.0/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.370637 qulab-2.1.0/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.370903 qulab-2.1.0/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.371918 qulab-2.1.0/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.373676 qulab-2.1.0/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.374693 qulab-2.1.0/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-31 15:59:31.375807 qulab-2.1.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-31 15:58:55.000000 qulab-2.1.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.374831 qulab-2.1.0/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-31 15:58:55.000000 qulab-2.1.0/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.375038 qulab-2.1.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-31 15:58:55.000000 qulab-2.1.0/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.272846 qulab-2.1.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-06-02 15:40:50.000000 qulab-2.1.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-06-02 15:40:50.000000 qulab-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-06-02 15:41:24.272630 qulab-2.1.1/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.272313 qulab-2.1.1/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-06-02 15:41:24.000000 qulab-2.1.1/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2311 2024-06-02 15:41:24.000000 qulab-2.1.1/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-06-02 15:41:24.000000 qulab-2.1.1/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-06-02 15:41:24.000000 qulab-2.1.1/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-06-02 15:41:24.000000 qulab-2.1.1/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-06-02 15:41:24.000000 qulab-2.1.1/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-06-02 15:40:50.000000 qulab-2.1.1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-06-02 15:40:50.000000 qulab-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.262101 qulab-2.1.1/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.263487 qulab-2.1.1/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.265063 qulab-2.1.1/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      117 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11579 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/query.py
+-rw-r--r--   0 runner     (501) staff       (20)    15087 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/record.py
+-rw-r--r--   0 runner     (501) staff       (20)     8563 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    29143 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2768 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/space.py
+-rw-r--r--   0 runner     (501) staff       (20)     3613 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.265872 qulab-2.1.1/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.266137 qulab-2.1.1/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.267132 qulab-2.1.1/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.267584 qulab-2.1.1/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.268215 qulab-2.1.1/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.268483 qulab-2.1.1/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.269565 qulab-2.1.1/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.271130 qulab-2.1.1/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.271932 qulab-2.1.1/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-06-02 15:40:50.000000 qulab-2.1.1/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-06-02 15:41:24.272882 qulab-2.1.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-06-02 15:40:50.000000 qulab-2.1.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.272040 qulab-2.1.1/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-06-02 15:40:50.000000 qulab-2.1.1/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-06-02 15:41:24.272143 qulab-2.1.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-06-02 15:40:50.000000 qulab-2.1.1/tests/test_scan.py
```

### Comparing `qulab-2.1.0/LICENSE` & `qulab-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/PKG-INFO` & `qulab-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.1.0
+Version: 2.1.1
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.1.0/QuLab.egg-info/PKG-INFO` & `qulab-2.1.1/QuLab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.1.0
+Version: 2.1.1
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.1.0/QuLab.egg-info/SOURCES.txt` & `qulab-2.1.1/QuLab.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 qulab/monitor/qt_compat.py
 qulab/monitor/toolbar.py
 qulab/scan/__init__.py
 qulab/scan/curd.py
 qulab/scan/expression.py
 qulab/scan/models.py
 qulab/scan/optimize.py
-qulab/scan/query_record.py
+qulab/scan/query.py
+qulab/scan/record.py
 qulab/scan/recorder.py
 qulab/scan/scan.py
 qulab/scan/server.py
+qulab/scan/space.py
 qulab/scan/utils.py
 qulab/storage/__init__.py
 qulab/storage/__main__.py
 qulab/storage/base_dataset.py
 qulab/storage/chunk.py
 qulab/storage/dataset.py
 qulab/storage/file.py
```

### Comparing `qulab-2.1.0/README.md` & `qulab-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/pyproject.toml` & `qulab-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/config.py` & `qulab-2.1.1/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/dataset.py` & `qulab-2.1.1/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/event_queue.py` & `qulab-2.1.1/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/mainwindow.py` & `qulab-2.1.1/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/monitor.py` & `qulab-2.1.1/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/ploter.py` & `qulab-2.1.1/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/qt_compat.py` & `qulab-2.1.1/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/monitor/toolbar.py` & `qulab-2.1.1/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/scan/curd.py` & `qulab-2.1.1/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/scan/expression.py` & `qulab-2.1.1/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/scan/models.py` & `qulab-2.1.1/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/scan/optimize.py` & `qulab-2.1.1/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/scan/query_record.py` & `qulab-2.1.1/qulab/scan/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 import dill
 import ipywidgets as widgets
 import zmq
 from IPython.display import display
 
 from qulab.sys.rpc.zmq_socket import ZMQContextManager
 
-from .recorder import Record
+from .record import Record
+from .scan import default_server
 
 
-def get_record(id, database='tcp://127.0.0.1:6789'):
+def get_record(id, database=default_server) -> Record:
     if isinstance(database, str) and database.startswith('tcp://'):
         with ZMQContextManager(zmq.DEALER, connect=database) as socket:
             socket.send_pyobj({
                 'method': 'record_description',
                 'record_id': id
             })
             d = dill.loads(socket.recv_pyobj())
-            return Record(id, database, d)
+            d.id = id
+            d.database = database
+            d._file = None
+            return d
     else:
         from .models import Record as RecordInDB
         from .models import create_engine, sessionmaker
 
         db_file = Path(database) / 'data.db'
         engine = create_engine(f'sqlite:///{db_file}')
         Session = sessionmaker(bind=engine)
@@ -288,15 +292,15 @@
 
 def _on_tags_submit(tags, ui_widgets):
     __query_state.page = 1
     _update_state(*_get_query_params(__query_state, ui_widgets))
     _update_view(ui_widgets)
 
 
-def lookup(app=None, limit=10, database='tcp://127.0.0.1:6789'):
+def lookup(app=None, limit=10, database=default_server):
     after = widgets.DatePicker()
     before = widgets.DatePicker()
     app_prefix = widgets.Label('App:')
     app_name = widgets.Dropdown(
         options=[
             '*',
         ],
```

### Comparing `qulab-2.1.0/qulab/scan/scan.py` & `qulab-2.1.1/qulab/scan/scan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 import asyncio
 import copy
-import datetime
 import inspect
 import itertools
 import os
 import re
 import sys
 import uuid
-import warnings
 from concurrent.futures import ProcessPoolExecutor
 from graphlib import TopologicalSorter
 from pathlib import Path
-from types import MethodType
-from typing import Any, Awaitable, Callable, Iterable, Type
+from typing import Any, Awaitable, Callable, Iterable
 
 import dill
 import numpy as np
-import skopt
 import zmq
-from skopt.space import Categorical, Integer, Real
-from tqdm.notebook import tqdm
 
 from ..sys.rpc.zmq_socket import ZMQContextManager
 from .expression import Env, Expression, Symbol
 from .optimize import NgOptimizer
-from .recorder import Record, default_record_port
-from .utils import async_zip, call_function
+from .record import Record
+from .recorder import default_record_port
+from .space import Optimizer, OptimizeSpace, Space
+from .utils import async_zip, call_function, dump_globals
+
+try:
+    from tqdm.notebook import tqdm
+except:
+
+    class tqdm():
+
+        def update(self, n):
+            pass
+
+        def close(self):
+            pass
+
+        def reset(self):
+            pass
+
 
 __process_uuid = uuid.uuid1()
 __task_counter = itertools.count()
 
+if os.getenv('QULAB_SERVER'):
+    default_server = os.getenv('QULAB_SERVER')
+else:
+    default_server = f'tcp://127.0.0.1:{default_record_port}'
+
 
 def task_uuid():
     return uuid.uuid3(__process_uuid, str(next(__task_counter)))
 
 
 def _get_depends(func: Callable):
     try:
@@ -51,87 +68,14 @@
         elif param.kind == param.VAR_KEYWORD:
             pass
         elif param.kind == param.VAR_POSITIONAL:
             raise ValueError('not support VAR_POSITIONAL')
     return args
 
 
-class OptimizeSpace():
-
-    def __init__(self, optimizer: 'Optimizer', space):
-        self.optimizer = optimizer
-        self.space = space
-        self.name = None
-
-    def __len__(self):
-        return self.optimizer.maxiter
-
-
-class Optimizer():
-
-    def __init__(self,
-                 scanner: 'Scan',
-                 name: str,
-                 level: int,
-                 method: str | Type = skopt.Optimizer,
-                 maxiter: int = 1000,
-                 minimize: bool = True,
-                 **kwds):
-        self.scanner = scanner
-        self.method = method
-        self.maxiter = maxiter
-        self.dimensions = {}
-        self.name = name
-        self.level = level
-        self.kwds = kwds
-        self.minimize = minimize
-
-    def create(self):
-        return self.method(list(self.dimensions.values()), **self.kwds)
-
-    def Categorical(self,
-                    categories,
-                    prior=None,
-                    transform=None,
-                    name=None) -> OptimizeSpace:
-        return OptimizeSpace(self,
-                             Categorical(categories, prior, transform, name))
-
-    def Integer(self,
-                low,
-                high,
-                prior="uniform",
-                base=10,
-                transform=None,
-                name=None,
-                dtype=np.int64) -> OptimizeSpace:
-        return OptimizeSpace(
-            self, Integer(low, high, prior, base, transform, name, dtype))
-
-    def Real(self,
-             low,
-             high,
-             prior="uniform",
-             base=10,
-             transform=None,
-             name=None,
-             dtype=float) -> OptimizeSpace:
-        return OptimizeSpace(
-            self, Real(low, high, prior, base, transform, name, dtype))
-
-    def __getstate__(self) -> dict:
-        state = self.__dict__.copy()
-        del state['scanner']
-        return state
-
-    def __setstate__(self, state: dict) -> None:
-        self.__dict__.update(state)
-        self.scanner = None
-
-
 class Promise():
     __slots__ = ['task', 'key', 'attr']
 
     def __init__(self, task, key=None, attr=None):
         self.task = task
         self.key = key
         self.attr = attr
@@ -176,15 +120,15 @@
                     pass
         return super().__new__(cls)
 
     def __init__(self,
                  app: str = 'task',
                  tags: tuple[str] = (),
                  database: str | Path
-                 | None = f'tcp://127.0.0.1:{default_record_port}',
+                 | None = default_server,
                  dump_globals: bool = False,
                  max_workers: int = 4,
                  max_promise: int = 100,
                  mixin=None):
         self.id = task_uuid()
         self.record = None
         self.namespace = {}
@@ -197,14 +141,16 @@
             'getters': {},
             'setters': {},
             'optimizers': {},
             'namespace': {} if dump_globals else None,
             'actions': {},
             'dependents': {},
             'order': {},
+            'axis': {},
+            'independent_variables': set(),
             'filters': {},
             'total': {},
             'database': database,
             'hiden': ['self', r'^__.*', r'.*__$'],
             'entry': {
                 'env': {},
                 'shell': '',
@@ -361,26 +307,42 @@
             func: A callable object or an instance of Expression.
             level: The level of the scan to add the filter. -1 means any level.
         """
         if level not in self.description['filters']:
             self.description['filters'][level] = []
         self.description['filters'][level].append(func)
 
-    def set(self, name: str, value, setter: Callable | None = None):
+    def set(self,
+            name: str,
+            value,
+            depends: Iterable[str] | None = None,
+            setter: Callable | None = None):
         try:
             dill.dumps(value)
         except:
             raise ValueError('value is not serializable.')
         if isinstance(value, Expression):
             self.add_depends(name, value.symbols())
             self.description['functions'][name] = value
         elif callable(value):
-            self.add_depends(name, _get_depends(value))
-            self.description['functions'][name] = value
+            if depends:
+                self.add_depends(name, depends)
+                s = ','.join(depends)
+                self.description['functions'][f'_tmp_{name}'] = value
+                self.description['functions'][name] = eval(
+                    f"lambda self, {s}: self.description['functions']['_tmp_{name}']({s})"
+                )
+            else:
+                self.add_depends(name, _get_depends(value))
+                self.description['functions'][name] = value
         else:
+            try:
+                value = Space.fromarray(value)
+            except:
+                pass
             self.description['consts'][name] = value
         if setter:
             self.description['setters'][name] = setter
 
     def search(self,
                name: str,
                range: Iterable | Expression | Callable | OptimizeSpace,
@@ -392,14 +354,18 @@
             range.name = name
             range.optimizer.dimensions[name] = range.space
             self._add_loop_var(name, range.optimizer.level, range)
             self.add_depends(range.optimizer.name, [name])
         else:
             if level is None:
                 raise ValueError('level must be provided.')
+            try:
+                range = Space.fromarray(range)
+            except:
+                pass
             self._add_loop_var(name, level, range)
             if isinstance(range, Expression) or callable(range):
                 self.add_depends(name, range.symbols())
         if setter:
             self.description['setters'][name] = setter
 
     def trace(self,
@@ -477,15 +443,22 @@
 
     async def _run(self):
         send_msg = asyncio.create_task(self._send_msg())
         update_progress_task = asyncio.create_task(self._update_progress())
 
         self._variables = {'self': self}
 
-        await update_variables(self._variables, self.description['consts'],
+        consts = {}
+        for k, v in self.description['consts'].items():
+            if isinstance(v, Space):
+                consts[k] = v.toarray()
+            else:
+                consts[k] = v
+
+        await update_variables(self._variables, consts,
                                self.description['setters'])
         for level, total in self.description['total'].items():
             if total == np.inf:
                 total = None
             self._bar[level] = tqdm(total=total)
 
         updates = await call_many_functions(
@@ -636,59 +609,14 @@
             return awaitable
 
     async def _await(self, awaitable: Awaitable):
         async with self._sem:
             return await awaitable
 
 
-class Unpicklable:
-
-    def __init__(self, obj):
-        self.type = str(type(obj))
-        self.id = id(obj)
-
-    def __repr__(self):
-        return f'<Unpicklable: {self.type} at 0x{id(self):x}>'
-
-
-class TooLarge:
-
-    def __init__(self, obj):
-        self.type = str(type(obj))
-        self.id = id(obj)
-
-    def __repr__(self):
-        return f'<TooLarge: {self.type} at 0x{id(self):x}>'
-
-
-def dump_globals(ns=None, *, size_limit=10 * 1024 * 1024, warn=False):
-    import __main__
-
-    if ns is None:
-        ns = __main__.__dict__
-
-    namespace = {}
-
-    for name, value in ns.items():
-        try:
-            buf = dill.dumps(value)
-        except:
-            namespace[name] = Unpicklable(value)
-            if warn:
-                warnings.warn(f'Unpicklable: {name} {type(value)}')
-        if len(buf) > size_limit:
-            namespace[name] = TooLarge(value)
-            if warn:
-                warnings.warn(f'TooLarge: {name} {type(value)}')
-        else:
-            namespace[name] = buf
-
-    return namespace
-
-
 def assymbly(description):
     import __main__
     from IPython import get_ipython
 
     if isinstance(description['namespace'], dict):
         description['namespace'] = dump_globals()
 
@@ -806,14 +734,46 @@
         keys = set(levels[level])
         description['order'][level] = []
         for ready in order:
             ready = list(keys & set(ready))
             if ready:
                 description['order'][level].append(ready)
                 keys -= set(ready)
+
+    axis = {}
+    independent_variables = set()
+
+    for name in description['consts']:
+        axis[name] = ()
+    for level, range_list in description['loops'].items():
+        for name, iterable in range_list:
+            if isinstance(iterable, OptimizeSpace):
+                axis[name] = tuple(range(level + 1))
+                continue
+            elif isinstance(iterable, (np.ndarray, list, tuple, range, Space)):
+                independent_variables.add(name)
+            axis[name] = (level, )
+
+    for level, group in description['order'].items():
+        for names in group:
+            for name in names:
+                if name not in description['dependents']:
+                    if name not in axis:
+                        axis[name] = (level, )
+                else:
+                    d = set()
+                    for n in description['dependents'][name]:
+                        d.update(axis[n])
+                    if name not in axis:
+                        axis[name] = tuple(sorted(d))
+                    else:
+                        axis[name] = tuple(sorted(set(axis[name]) | d))
+    description['axis'] = axis
+    description['independent_variables'] = independent_variables
+
     return description
 
 
 async def update_variables(variables: dict[str, Any], updates: dict[str, Any],
                            setters: dict[str, Callable]):
     coros = []
     for name, value in updates.items():
@@ -841,14 +801,16 @@
 
     for name, iter in iters:
         if isinstance(iter, OptimizeSpace):
             if iter.optimizer.name not in opts:
                 opts[iter.optimizer.name] = iter.optimizer.create()
         elif isinstance(iter, Expression):
             iters_d[name] = iter.eval(env)
+        elif isinstance(iter, Space):
+            iters_d[name] = iter.toarray()
         elif callable(iter):
             iters_d[name] = await call_function(iter, variables)
         else:
             iters_d[name] = iter
 
     maxiter = 0xffffffff
     for name, opt in opts.items():
```

### Comparing `qulab-2.1.0/qulab/scan/server.py` & `qulab-2.1.1/qulab/scan/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import asyncio
 import pickle
-import sys
-import time
-import uuid
-from pathlib import Path
-from .scan import Scan
+
 import click
 import dill
-import numpy as np
 import zmq
 from loguru import logger
 
 from qulab.sys.rpc.zmq_socket import ZMQContextManager
 
+from .scan import Scan
+
 pool = {}
 
+
 class Request():
     __slots__ = ['sock', 'identity', 'msg', 'method']
 
     def __init__(self, sock, identity, msg):
         self.sock = sock
         self.identity = identity
         self.msg = pickle.loads(msg)
```

### Comparing `qulab-2.1.0/qulab/scan/utils.py` & `qulab-2.1.1/qulab/scan/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,63 @@
 import ast
 import asyncio
 import inspect
+import warnings
 from typing import Any, Callable
 
+import dill
+
 from .expression import Env, Expression
 
 
+class Unpicklable:
+
+    def __init__(self, obj):
+        self.type = str(type(obj))
+        self.id = id(obj)
+
+    def __repr__(self):
+        return f'<Unpicklable: {self.type} at 0x{id(self):x}>'
+
+
+class TooLarge:
+
+    def __init__(self, obj):
+        self.type = str(type(obj))
+        self.id = id(obj)
+
+    def __repr__(self):
+        return f'<TooLarge: {self.type} at 0x{id(self):x}>'
+
+
+def dump_globals(ns=None, *, size_limit=10 * 1024 * 1024, warn=False):
+    import __main__
+
+    if ns is None:
+        ns = __main__.__dict__
+
+    namespace = {}
+
+    for name, value in ns.items():
+        try:
+            buf = dill.dumps(value)
+        except:
+            namespace[name] = Unpicklable(value)
+            if warn:
+                warnings.warn(f'Unpicklable: {name} {type(value)}')
+        if len(buf) > size_limit:
+            namespace[name] = TooLarge(value)
+            if warn:
+                warnings.warn(f'TooLarge: {name} {type(value)}')
+        else:
+            namespace[name] = buf
+
+    return namespace
+
+
 def is_valid_identifier(s: str) -> bool:
     """
     Check if a string is a valid identifier.
     """
     try:
         ast.parse(f"f({s}=0)")
         return True
```

### Comparing `qulab-2.1.0/qulab/storage/__main__.py` & `qulab-2.1.1/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/backend/redis.py` & `qulab-2.1.1/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/base_dataset.py` & `qulab-2.1.1/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/chunk.py` & `qulab-2.1.1/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/dataset.py` & `qulab-2.1.1/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/file.py` & `qulab-2.1.1/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/__init__.py` & `qulab-2.1.1/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/config.py` & `qulab-2.1.1/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/file.py` & `qulab-2.1.1/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/ipy.py` & `qulab-2.1.1/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/models.py` & `qulab-2.1.1/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/record.py` & `qulab-2.1.1/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/report.py` & `qulab-2.1.1/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/models/tag.py` & `qulab-2.1.1/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/storage/storage.py` & `qulab-2.1.1/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/chat.py` & `qulab-2.1.1/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/device/basedevice.py` & `qulab-2.1.1/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/device/loader.py` & `qulab-2.1.1/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/device/utils.py` & `qulab-2.1.1/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.1.1/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/ipy_events.py` & `qulab-2.1.1/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/bencoder.py` & `qulab-2.1.1/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/cli.py` & `qulab-2.1.1/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/dhcp.py` & `qulab-2.1.1/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/dhcpd.py` & `qulab-2.1.1/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/kad.py` & `qulab-2.1.1/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/kcp.py` & `qulab-2.1.1/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/net/nginx.py` & `qulab-2.1.1/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/progress.py` & `qulab-2.1.1/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/exceptions.py` & `qulab-2.1.1/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/msgpack.py` & `qulab-2.1.1/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/msgpack.pyi` & `qulab-2.1.1/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/rpc.py` & `qulab-2.1.1/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/serialize.py` & `qulab-2.1.1/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/server.py` & `qulab-2.1.1/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/socket.py` & `qulab-2.1.1/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/utils.py` & `qulab-2.1.1/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/sys/rpc/zmq_socket.py` & `qulab-2.1.1/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/__init__.py` & `qulab-2.1.1/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/__main__.py` & `qulab-2.1.1/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/_autoplot.py` & `qulab-2.1.1/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/plot_layout.py` & `qulab-2.1.1/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/plot_seq.py` & `qulab-2.1.1/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/qdat.py` & `qulab-2.1.1/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/qulab/visualization/widgets.py` & `qulab-2.1.1/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.1.0/setup.py` & `qulab-2.1.1/setup.py`

 * *Files identical despite different names*

