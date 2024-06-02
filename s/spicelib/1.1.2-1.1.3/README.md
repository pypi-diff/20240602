# Comparing `tmp/spicelib-1.1.2.tar.gz` & `tmp/spicelib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicelib-1.1.2.tar", last modified: Sun May  5 18:29:47 2024, max compression
+gzip compressed data, was "spicelib-1.1.3.tar", last modified: Sun Jun  2 10:43:53 2024, max compression
```

## Comparing `spicelib-1.1.2.tar` & `spicelib-1.1.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.109243 spicelib-1.1.2/
--rw-rw-rw-   0        0        0    35823 2023-09-01 13:27:07.000000 spicelib-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      132 2024-03-10 15:30:59.000000 spicelib-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    67542 2024-05-05 18:29:47.108236 spicelib-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    25431 2024-05-05 15:59:33.000000 spicelib-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.839020 spicelib-1.1.2/examples/
--rw-rw-rw-   0        0        0      798 2023-09-01 13:57:48.000000 spicelib-1.1.2/examples/ltsteps_example.py
--rw-rw-rw-   0        0        0     1142 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/ngspice_batch.py
--rw-rw-rw-   0        0        0     1708 2024-02-23 21:06:01.000000 spicelib-1.1.2/examples/qspice_example.py
--rw-rw-rw-   0        0        0     3151 2023-09-18 15:59:31.000000 spicelib-1.1.2/examples/raw_plotting.py
--rw-rw-rw-   0        0        0      486 2024-02-25 16:29:46.000000 spicelib-1.1.2/examples/raw_read_example.py
--rw-rw-rw-   0        0        0     4276 2024-02-25 14:48:43.000000 spicelib-1.1.2/examples/raw_write_example.py
--rw-rw-rw-   0        0        0     2241 2024-05-05 15:55:48.000000 spicelib-1.1.2/examples/run_fast_worst_case.py
--rw-rw-rw-   0        0        0     2673 2024-03-16 10:43:35.000000 spicelib-1.1.2/examples/run_montecarlo.py
--rw-rw-rw-   0        0        0     1910 2024-02-02 12:19:23.000000 spicelib-1.1.2/examples/run_sensitivity.py
--rw-rw-rw-   0        0        0     2812 2024-04-21 13:17:00.000000 spicelib-1.1.2/examples/run_worst_case.py
--rw-rw-rw-   0        0        0     2464 2024-03-16 10:41:24.000000 spicelib-1.1.2/examples/sim_client_example.py
--rw-rw-rw-   0        0        0     1479 2024-03-16 10:24:39.000000 spicelib-1.1.2/examples/sim_runner_asc_example.py
--rw-rw-rw-   0        0        0     2867 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sim_runner_callback_example.py
--rw-rw-rw-   0        0        0     2732 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/sim_runner_callback_process_example.py
--rw-rw-rw-   0        0        0     1705 2024-03-16 10:24:39.000000 spicelib-1.1.2/examples/sim_runner_example.py
--rw-rw-rw-   0        0        0     2010 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/sim_server_example.py
--rw-rw-rw-   0        0        0     1253 2024-02-23 21:30:13.000000 spicelib-1.1.2/examples/sim_stepper_example.py
--rw-rw-rw-   0        0        0      379 2023-09-08 09:39:40.000000 spicelib-1.1.2/examples/spice_editor_example.py
--rw-rw-rw-   0        0        0     1280 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sub_circuit_asc_edits.py
--rw-rw-rw-   0        0        0     1302 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sub_circuit_edits.py
--rw-rw-rw-   0        0        0     1184 2024-04-21 13:16:18.000000 spicelib-1.1.2/examples/sub_circuit_qsch_edits.py
--rw-rw-rw-   0        0        0     1714 2024-05-05 15:55:48.000000 spicelib-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 18:29:47.109243 spicelib-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.840025 spicelib-1.1.2/spicelib/
--rw-rw-rw-   0        0        0     1741 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.886121 spicelib-1.1.2/spicelib/client_server/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/client_server/__init__.py
--rw-rw-rw-   0        0        0    10097 2024-02-15 17:23:09.000000 spicelib-1.1.2/spicelib/client_server/sim_client.py
--rw-rw-rw-   0        0        0     8378 2024-02-16 14:22:36.000000 spicelib-1.1.2/spicelib/client_server/sim_server.py
--rw-rw-rw-   0        0        0     6097 2024-02-15 19:28:40.000000 spicelib-1.1.2/spicelib/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.900761 spicelib-1.1.2/spicelib/editor/
--rw-rw-rw-   0        0        0      123 2023-10-15 17:22:56.000000 spicelib-1.1.2/spicelib/editor/__init__.py
--rw-rw-rw-   0        0        0    24463 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/asc_editor.py
--rw-rw-rw-   0        0        0    13608 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/asy_reader.py
--rw-rw-rw-   0        0        0    19855 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/base_editor.py
--rw-rw-rw-   0        0        0    13410 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/base_schematic.py
--rw-rw-rw-   0        0        0     4065 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/ltspice_utils.py
--rw-rw-rw-   0        0        0    36418 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/qsch_editor.py
--rw-rw-rw-   0        0        0    47162 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/editor/spice_editor.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.922097 spicelib-1.1.2/spicelib/log/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/log/__init__.py
--rw-rw-rw-   0        0        0    20952 2024-03-02 20:08:05.000000 spicelib-1.1.2/spicelib/log/logfile_data.py
--rw-rw-rw-   0        0        0    25636 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/log/ltsteps.py
--rw-rw-rw-   0        0        0     8183 2024-03-02 20:02:43.000000 spicelib-1.1.2/spicelib/log/qspice_log_reader.py
--rw-rw-rw-   0        0        0     6664 2023-09-01 14:14:09.000000 spicelib-1.1.2/spicelib/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.944039 spicelib-1.1.2/spicelib/raw/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/raw/__init__.py
--rw-rw-rw-   0        0        0    14833 2023-10-16 19:39:04.000000 spicelib-1.1.2/spicelib/raw/raw_classes.py
--rw-rw-rw-   0        0        0     6197 2023-09-01 23:08:42.000000 spicelib-1.1.2/spicelib/raw/raw_convert.py
--rw-rw-rw-   0        0        0    42506 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/raw/raw_read.py
--rw-rw-rw-   0        0        0    17368 2023-09-01 14:14:09.000000 spicelib-1.1.2/spicelib/raw/raw_write.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:46.986493 spicelib-1.1.2/spicelib/scripts/
--rw-rw-rw-   0        0        0     9237 2024-04-21 13:16:18.000000 spicelib-1.1.2/spicelib/scripts/asc_to_qsch.py
--rw-rw-rw-   0        0        0     5654 2024-03-09 13:11:41.000000 spicelib-1.1.2/spicelib/scripts/asc_to_qsch_data.xml
--rw-rw-rw-   0        0        0    12544 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/scripts/histogram.py
--rw-rw-rw-   0        0        0     7464 2024-03-16 10:24:39.000000 spicelib-1.1.2/spicelib/scripts/ltsteps.py
--rw-rw-rw-   0        0        0     4479 2023-09-01 22:58:58.000000 spicelib-1.1.2/spicelib/scripts/rawplot.py
--rw-rw-rw-   0        0        0     3505 2024-04-28 17:15:15.000000 spicelib-1.1.2/spicelib/scripts/readme_update.py
--rw-rw-rw-   0        0        0     4295 2024-02-15 10:43:01.000000 spicelib-1.1.2/spicelib/scripts/run_server.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.003037 spicelib-1.1.2/spicelib/sim/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/sim/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-09-08 09:39:40.000000 spicelib-1.1.2/spicelib/sim/process_callback.py
--rw-rw-rw-   0        0        0     8337 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/sim/run_task.py
--rw-rw-rw-   0        0        0    28817 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/sim/sim_runner.py
--rw-rw-rw-   0        0        0    10216 2023-10-19 12:50:05.000000 spicelib-1.1.2/spicelib/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     5757 2023-11-03 11:50:22.000000 spicelib-1.1.2/spicelib/sim/simulator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.042833 spicelib-1.1.2/spicelib/sim/tookit/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.2/spicelib/sim/tookit/__init__.py
--rw-rw-rw-   0        0        0     4800 2023-10-19 16:51:29.000000 spicelib-1.1.2/spicelib/sim/tookit/failure_modes.py
--rw-rw-rw-   0        0        0    14582 2024-02-15 19:51:50.000000 spicelib-1.1.2/spicelib/sim/tookit/fast_worst_case.py
--rw-rw-rw-   0        0        0    12645 2024-03-09 16:55:25.000000 spicelib-1.1.2/spicelib/sim/tookit/montecarlo.py
--rw-rw-rw-   0        0        0    10260 2024-02-15 19:49:53.000000 spicelib-1.1.2/spicelib/sim/tookit/quick_sensitivity_analysis.py
--rw-rw-rw-   0        0        0     9616 2024-02-15 09:14:53.000000 spicelib-1.1.2/spicelib/sim/tookit/sim_analysis.py
--rw-rw-rw-   0        0        0    13777 2024-02-15 19:48:44.000000 spicelib-1.1.2/spicelib/sim/tookit/tolerance_deviations.py
--rw-rw-rw-   0        0        0    13523 2024-02-15 19:49:32.000000 spicelib-1.1.2/spicelib/sim/tookit/worst_case.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.063164 spicelib-1.1.2/spicelib/simulators/
--rw-rw-rw-   0        0        0        0 2023-09-08 09:39:40.000000 spicelib-1.1.2/spicelib/simulators/__init__.py
--rw-rw-rw-   0        0        0    10327 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/simulators/ltspice_simulator.py
--rw-rw-rw-   0        0        0     5355 2023-10-08 21:40:06.000000 spicelib-1.1.2/spicelib/simulators/ngspice_simulator.py
--rw-rw-rw-   0        0        0     6026 2023-11-03 11:49:49.000000 spicelib-1.1.2/spicelib/simulators/qspice_simulator.py
--rw-rw-rw-   0        0        0     8073 2023-10-08 21:40:06.000000 spicelib-1.1.2/spicelib/simulators/xyce_simulator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.068472 spicelib-1.1.2/spicelib/utils/
--rw-rw-rw-   0        0        0     3811 2024-02-10 22:37:40.000000 spicelib-1.1.2/spicelib/utils/detect_encoding.py
--rw-rw-rw-   0        0        0     3105 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/utils/file_search.py
--rw-rw-rw-   0        0        0     8213 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/utils/sweep_iterators.py
--rw-rw-rw-   0        0        0     2471 2024-05-05 15:55:48.000000 spicelib-1.1.2/spicelib/utils/windows_short_names.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.107236 spicelib-1.1.2/spicelib.egg-info/
--rw-rw-rw-   0        0        0    67542 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2804 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      330 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       53 2024-05-05 18:29:46.000000 spicelib-1.1.2/spicelib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 18:29:47.105230 spicelib-1.1.2/unittests/
--rw-rw-rw-   0        0        0     4093 2023-09-01 21:04:13.000000 spicelib-1.1.2/unittests/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0     4856 2024-02-11 08:24:38.000000 spicelib-1.1.2/unittests/test_asc_editor.py
--rw-rw-rw-   0        0        0     6573 2024-04-21 13:16:18.000000 spicelib-1.1.2/unittests/test_qsch_editor.py
--rw-rw-rw-   0        0        0    20957 2024-03-16 10:24:39.000000 spicelib-1.1.2/unittests/test_qspice_rawread.py
--rw-rw-rw-   0        0        0     4865 2023-10-19 13:29:57.000000 spicelib-1.1.2/unittests/test_spice_editor.py
--rw-rw-rw-   0        0        0    22930 2024-03-16 10:24:39.000000 spicelib-1.1.2/unittests/test_spicelib.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.514292 spicelib-1.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 13:27:07.000000 spicelib-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      132 2024-03-10 15:30:59.000000 spicelib-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    68077 2024-06-02 10:43:53.513285 spicelib-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    25966 2024-06-01 17:29:12.000000 spicelib-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.175117 spicelib-1.1.3/examples/
+-rw-rw-rw-   0        0        0      798 2023-09-01 13:57:48.000000 spicelib-1.1.3/examples/ltsteps_example.py
+-rw-rw-rw-   0        0        0     1142 2023-09-08 09:39:40.000000 spicelib-1.1.3/examples/ngspice_batch.py
+-rw-rw-rw-   0        0        0     1708 2024-02-23 21:06:01.000000 spicelib-1.1.3/examples/qspice_example.py
+-rw-rw-rw-   0        0        0     3151 2023-09-18 15:59:31.000000 spicelib-1.1.3/examples/raw_plotting.py
+-rw-rw-rw-   0        0        0      486 2024-02-25 16:29:46.000000 spicelib-1.1.3/examples/raw_read_example.py
+-rw-rw-rw-   0        0        0     4276 2024-02-25 14:48:43.000000 spicelib-1.1.3/examples/raw_write_example.py
+-rw-rw-rw-   0        0        0     2241 2024-05-19 20:40:39.000000 spicelib-1.1.3/examples/run_fast_worst_case.py
+-rw-rw-rw-   0        0        0     2673 2024-03-16 10:43:35.000000 spicelib-1.1.3/examples/run_montecarlo.py
+-rw-rw-rw-   0        0        0     1910 2024-02-02 12:19:23.000000 spicelib-1.1.3/examples/run_sensitivity.py
+-rw-rw-rw-   0        0        0     2812 2024-05-19 20:40:39.000000 spicelib-1.1.3/examples/run_worst_case.py
+-rw-rw-rw-   0        0        0     2464 2024-03-16 10:41:24.000000 spicelib-1.1.3/examples/sim_client_example.py
+-rw-rw-rw-   0        0        0     1479 2024-03-16 10:24:39.000000 spicelib-1.1.3/examples/sim_runner_asc_example.py
+-rw-rw-rw-   0        0        0     2867 2024-05-19 20:40:39.000000 spicelib-1.1.3/examples/sim_runner_callback_example.py
+-rw-rw-rw-   0        0        0     2732 2023-09-08 09:39:40.000000 spicelib-1.1.3/examples/sim_runner_callback_process_example.py
+-rw-rw-rw-   0        0        0     1705 2024-03-16 10:24:39.000000 spicelib-1.1.3/examples/sim_runner_example.py
+-rw-rw-rw-   0        0        0     2010 2023-09-08 09:39:40.000000 spicelib-1.1.3/examples/sim_server_example.py
+-rw-rw-rw-   0        0        0     1253 2024-02-23 21:30:13.000000 spicelib-1.1.3/examples/sim_stepper_example.py
+-rw-rw-rw-   0        0        0      379 2023-09-08 09:39:40.000000 spicelib-1.1.3/examples/spice_editor_example.py
+-rw-rw-rw-   0        0        0     1280 2024-05-19 20:39:54.000000 spicelib-1.1.3/examples/sub_circuit_asc_edits.py
+-rw-rw-rw-   0        0        0     1302 2024-05-19 20:39:54.000000 spicelib-1.1.3/examples/sub_circuit_edits.py
+-rw-rw-rw-   0        0        0     1184 2024-05-19 20:39:54.000000 spicelib-1.1.3/examples/sub_circuit_qsch_edits.py
+-rw-rw-rw-   0        0        0     1714 2024-05-19 20:54:16.000000 spicelib-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:43:53.515289 spicelib-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.184684 spicelib-1.1.3/spicelib/
+-rw-rw-rw-   0        0        0     1741 2024-03-16 10:24:39.000000 spicelib-1.1.3/spicelib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.230754 spicelib-1.1.3/spicelib/client_server/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.3/spicelib/client_server/__init__.py
+-rw-rw-rw-   0        0        0    10097 2024-02-15 17:23:09.000000 spicelib-1.1.3/spicelib/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     8378 2024-02-16 14:22:36.000000 spicelib-1.1.3/spicelib/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     6097 2024-02-15 19:28:40.000000 spicelib-1.1.3/spicelib/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.264501 spicelib-1.1.3/spicelib/editor/
+-rw-rw-rw-   0        0        0      123 2023-10-15 17:22:56.000000 spicelib-1.1.3/spicelib/editor/__init__.py
+-rw-rw-rw-   0        0        0    34355 2024-06-02 10:34:26.000000 spicelib-1.1.3/spicelib/editor/asc_editor.py
+-rw-rw-rw-   0        0        0    13426 2024-06-02 10:38:57.000000 spicelib-1.1.3/spicelib/editor/asy_reader.py
+-rw-rw-rw-   0        0        0    22873 2024-06-02 10:34:26.000000 spicelib-1.1.3/spicelib/editor/base_editor.py
+-rw-rw-rw-   0        0        0    15989 2024-06-01 17:22:52.000000 spicelib-1.1.3/spicelib/editor/base_schematic.py
+-rw-rw-rw-   0        0        0     4298 2024-06-01 17:22:52.000000 spicelib-1.1.3/spicelib/editor/ltspice_utils.py
+-rw-rw-rw-   0        0        0    48241 2024-06-02 10:34:26.000000 spicelib-1.1.3/spicelib/editor/qsch_editor.py
+-rw-rw-rw-   0        0        0    49437 2024-06-01 17:22:52.000000 spicelib-1.1.3/spicelib/editor/spice_editor.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.290750 spicelib-1.1.3/spicelib/log/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.3/spicelib/log/__init__.py
+-rw-rw-rw-   0        0        0    20952 2024-05-09 16:26:17.000000 spicelib-1.1.3/spicelib/log/logfile_data.py
+-rw-rw-rw-   0        0        0    25636 2024-03-16 10:24:39.000000 spicelib-1.1.3/spicelib/log/ltsteps.py
+-rw-rw-rw-   0        0        0     8183 2024-03-02 20:02:43.000000 spicelib-1.1.3/spicelib/log/qspice_log_reader.py
+-rw-rw-rw-   0        0        0     6664 2023-09-01 14:14:09.000000 spicelib-1.1.3/spicelib/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.317221 spicelib-1.1.3/spicelib/raw/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.3/spicelib/raw/__init__.py
+-rw-rw-rw-   0        0        0    14833 2023-10-16 19:39:04.000000 spicelib-1.1.3/spicelib/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     6197 2023-09-01 23:08:42.000000 spicelib-1.1.3/spicelib/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    42506 2024-02-10 22:37:40.000000 spicelib-1.1.3/spicelib/raw/raw_read.py
+-rw-rw-rw-   0        0        0    17368 2023-09-01 14:14:09.000000 spicelib-1.1.3/spicelib/raw/raw_write.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.361518 spicelib-1.1.3/spicelib/scripts/
+-rw-rw-rw-   0        0        0     9413 2024-06-01 17:22:52.000000 spicelib-1.1.3/spicelib/scripts/asc_to_qsch.py
+-rw-rw-rw-   0        0        0     5654 2024-03-09 13:11:41.000000 spicelib-1.1.3/spicelib/scripts/asc_to_qsch_data.xml
+-rw-rw-rw-   0        0        0    12544 2024-03-16 10:24:39.000000 spicelib-1.1.3/spicelib/scripts/histogram.py
+-rw-rw-rw-   0        0        0     7464 2024-03-16 10:24:39.000000 spicelib-1.1.3/spicelib/scripts/ltsteps.py
+-rw-rw-rw-   0        0        0     4479 2023-09-01 22:58:58.000000 spicelib-1.1.3/spicelib/scripts/rawplot.py
+-rw-rw-rw-   0        0        0     3505 2024-05-19 20:46:13.000000 spicelib-1.1.3/spicelib/scripts/readme_update.py
+-rw-rw-rw-   0        0        0     4295 2024-02-15 10:43:01.000000 spicelib-1.1.3/spicelib/scripts/run_server.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.390111 spicelib-1.1.3/spicelib/sim/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.3/spicelib/sim/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-09-08 09:39:40.000000 spicelib-1.1.3/spicelib/sim/process_callback.py
+-rw-rw-rw-   0        0        0     8337 2024-02-10 22:37:40.000000 spicelib-1.1.3/spicelib/sim/run_task.py
+-rw-rw-rw-   0        0        0    28817 2024-05-19 20:45:52.000000 spicelib-1.1.3/spicelib/sim/sim_runner.py
+-rw-rw-rw-   0        0        0    10216 2023-10-19 12:50:05.000000 spicelib-1.1.3/spicelib/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     5757 2023-11-03 11:50:22.000000 spicelib-1.1.3/spicelib/sim/simulator.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.428894 spicelib-1.1.3/spicelib/sim/tookit/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.3/spicelib/sim/tookit/__init__.py
+-rw-rw-rw-   0        0        0     4800 2023-10-19 16:51:29.000000 spicelib-1.1.3/spicelib/sim/tookit/failure_modes.py
+-rw-rw-rw-   0        0        0    14582 2024-02-15 19:51:50.000000 spicelib-1.1.3/spicelib/sim/tookit/fast_worst_case.py
+-rw-rw-rw-   0        0        0    12645 2024-03-09 16:55:25.000000 spicelib-1.1.3/spicelib/sim/tookit/montecarlo.py
+-rw-rw-rw-   0        0        0    10260 2024-02-15 19:49:53.000000 spicelib-1.1.3/spicelib/sim/tookit/quick_sensitivity_analysis.py
+-rw-rw-rw-   0        0        0     9616 2024-02-15 09:14:53.000000 spicelib-1.1.3/spicelib/sim/tookit/sim_analysis.py
+-rw-rw-rw-   0        0        0    13777 2024-02-15 19:48:44.000000 spicelib-1.1.3/spicelib/sim/tookit/tolerance_deviations.py
+-rw-rw-rw-   0        0        0    13523 2024-02-15 19:49:32.000000 spicelib-1.1.3/spicelib/sim/tookit/worst_case.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.452810 spicelib-1.1.3/spicelib/simulators/
+-rw-rw-rw-   0        0        0        0 2023-09-08 09:39:40.000000 spicelib-1.1.3/spicelib/simulators/__init__.py
+-rw-rw-rw-   0        0        0    10327 2024-02-10 22:37:40.000000 spicelib-1.1.3/spicelib/simulators/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     5355 2023-10-08 21:40:06.000000 spicelib-1.1.3/spicelib/simulators/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     6026 2023-11-03 11:49:49.000000 spicelib-1.1.3/spicelib/simulators/qspice_simulator.py
+-rw-rw-rw-   0        0        0     8073 2023-10-08 21:40:06.000000 spicelib-1.1.3/spicelib/simulators/xyce_simulator.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.477685 spicelib-1.1.3/spicelib/utils/
+-rw-rw-rw-   0        0        0     3811 2024-02-10 22:37:40.000000 spicelib-1.1.3/spicelib/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0     3105 2024-05-19 20:45:52.000000 spicelib-1.1.3/spicelib/utils/file_search.py
+-rw-rw-rw-   0        0        0     8213 2024-05-19 20:46:05.000000 spicelib-1.1.3/spicelib/utils/sweep_iterators.py
+-rw-rw-rw-   0        0        0     2471 2024-05-19 20:46:05.000000 spicelib-1.1.3/spicelib/utils/windows_short_names.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.512285 spicelib-1.1.3/spicelib.egg-info/
+-rw-rw-rw-   0        0        0    68077 2024-06-02 10:43:53.000000 spicelib-1.1.3/spicelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2024-06-02 10:43:53.000000 spicelib-1.1.3/spicelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:43:53.000000 spicelib-1.1.3/spicelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      330 2024-06-02 10:43:53.000000 spicelib-1.1.3/spicelib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2024-06-02 10:43:53.000000 spicelib-1.1.3/spicelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-06-02 10:43:53.000000 spicelib-1.1.3/spicelib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 10:43:53.511288 spicelib-1.1.3/unittests/
+-rw-rw-rw-   0        0        0     4093 2023-09-01 21:04:13.000000 spicelib-1.1.3/unittests/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0     5478 2024-06-01 17:22:52.000000 spicelib-1.1.3/unittests/test_asc_editor.py
+-rw-rw-rw-   0        0        0     7769 2024-06-01 17:22:52.000000 spicelib-1.1.3/unittests/test_qsch_editor.py
+-rw-rw-rw-   0        0        0    20957 2024-03-16 10:24:39.000000 spicelib-1.1.3/unittests/test_qspice_rawread.py
+-rw-rw-rw-   0        0        0     5483 2024-06-01 17:22:52.000000 spicelib-1.1.3/unittests/test_spice_editor.py
+-rw-rw-rw-   0        0        0    22930 2024-03-16 10:24:39.000000 spicelib-1.1.3/unittests/test_spicelib.py
```

### Comparing `spicelib-1.1.2/LICENSE` & `spicelib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/PKG-INFO` & `spicelib-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicelib
-Version: 1.1.2
+Version: 1.1.3
 Summary: A set of tools to Automate Spice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1185,14 +1185,24 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+
+* Version 1.1.3
+  * Implementing a set_component_parameters() and get_component_parameters() method on the Editor classes. 
+    This method allows to set and get the parameters of a component.
+  * Bug Fixes:
+    * AscEditor was hanging in comments. Issue #43
+    * Supporting other text orientations on the AscEditor. Issue #44
+    * Allow other encodings in AscEditor. Issues #45 and #48
+  * Supporting lines, rectangles, circles and arcs in AscEditor.
+  * Improving the regex for the component values in the SpiceEditor. 
 * Version 1.1.2
   * Fixes on the readme_update.py script. Was not supporting spaces after the []
   * Solving issue PyLTspice Issue #138. Hierarchical edits to ASC files are now supported.
 * Version 1.1.1
   * Supporting hierarchical edits on both QSpice and LTspice schematics
   * Skipping the need of the rich library on examples
   * Giving feedback on the search for symbols on the ASC to QSCH conversion
```

### Comparing `spicelib-1.1.2/README.md` & `spicelib-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -487,14 +487,24 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+
+* Version 1.1.3
+  * Implementing a set_component_parameters() and get_component_parameters() method on the Editor classes. 
+    This method allows to set and get the parameters of a component.
+  * Bug Fixes:
+    * AscEditor was hanging in comments. Issue #43
+    * Supporting other text orientations on the AscEditor. Issue #44
+    * Allow other encodings in AscEditor. Issues #45 and #48
+  * Supporting lines, rectangles, circles and arcs in AscEditor.
+  * Improving the regex for the component values in the SpiceEditor. 
 * Version 1.1.2
   * Fixes on the readme_update.py script. Was not supporting spaces after the []
   * Solving issue PyLTspice Issue #138. Hierarchical edits to ASC files are now supported.
 * Version 1.1.1
   * Supporting hierarchical edits on both QSpice and LTspice schematics
   * Skipping the need of the rich library on examples
   * Giving feedback on the search for symbols on the ASC to QSCH conversion
```

### Comparing `spicelib-1.1.2/examples/ltsteps_example.py` & `spicelib-1.1.3/examples/ltsteps_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/ngspice_batch.py` & `spicelib-1.1.3/examples/ngspice_batch.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/qspice_example.py` & `spicelib-1.1.3/examples/qspice_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/raw_plotting.py` & `spicelib-1.1.3/examples/raw_plotting.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/raw_write_example.py` & `spicelib-1.1.3/examples/raw_write_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/run_fast_worst_case.py` & `spicelib-1.1.3/examples/run_fast_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/run_montecarlo.py` & `spicelib-1.1.3/examples/run_montecarlo.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/run_sensitivity.py` & `spicelib-1.1.3/examples/run_sensitivity.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/run_worst_case.py` & `spicelib-1.1.3/examples/run_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_client_example.py` & `spicelib-1.1.3/examples/sim_client_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_runner_asc_example.py` & `spicelib-1.1.3/examples/sim_runner_asc_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_runner_callback_example.py` & `spicelib-1.1.3/examples/sim_runner_callback_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_runner_callback_process_example.py` & `spicelib-1.1.3/examples/sim_runner_callback_process_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_runner_example.py` & `spicelib-1.1.3/examples/sim_runner_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_server_example.py` & `spicelib-1.1.3/examples/sim_server_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sim_stepper_example.py` & `spicelib-1.1.3/examples/sim_stepper_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sub_circuit_asc_edits.py` & `spicelib-1.1.3/examples/sub_circuit_asc_edits.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sub_circuit_edits.py` & `spicelib-1.1.3/examples/sub_circuit_edits.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/examples/sub_circuit_qsch_edits.py` & `spicelib-1.1.3/examples/sub_circuit_qsch_edits.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/pyproject.toml` & `spicelib-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "spicelib"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate Spice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `spicelib-1.1.2/spicelib/__init__.py` & `spicelib-1.1.3/spicelib/__init__.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/client_server/sim_client.py` & `spicelib-1.1.3/spicelib/client_server/sim_client.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/client_server/sim_server.py` & `spicelib-1.1.3/spicelib/client_server/sim_server.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/client_server/srv_sim_runner.py` & `spicelib-1.1.3/spicelib/client_server/srv_sim_runner.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/editor/asc_editor.py` & `spicelib-1.1.3/spicelib/editor/asc_editor.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,54 +14,70 @@
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import os.path
 from pathlib import Path
-from typing import Union, Optional
+from typing import Union, Optional, Tuple
+from ..utils.detect_encoding import detect_encoding, EncodingDetectError
 import re
 import logging
 
 from .ltspice_utils import TEXT_REGEX, TEXT_REGEX_X, TEXT_REGEX_Y, TEXT_REGEX_ALIGN, TEXT_REGEX_SIZE, TEXT_REGEX_TYPE, \
     TEXT_REGEX_TEXT, END_LINE_TERM, ASC_ROTATION_DICT, ASC_INV_ROTATION_DICT, asc_text_align_set, asc_text_align_get
 from .spice_editor import SpiceEditor, SpiceCircuit
 from ..utils.file_search import search_file_in_containers
 from .base_editor import format_eng, ComponentNotFoundError, ParameterNotFoundError, PARAM_REGEX, \
     UNIQUE_SIMULATION_DOT_INSTRUCTIONS
-from .base_schematic import (BaseSchematic, Point, Line, Text, SchematicComponent, ERotation, TextTypeEnum, Port)
+from .base_schematic import (BaseSchematic, Point, Line, Shape, Text, SchematicComponent, ERotation, TextTypeEnum, Port)
 from .asy_reader import AsyReader
 
+from ..log.logfile_data import try_convert_value
+
 _logger = logging.getLogger("spicelib.AscEditor")
 
 
+LTSPICE_PARAMETERS = ("Value", "Value2", "SpiceModel", "SpiceLine", "SpiceLine2")
+LTSPICE_PARAMETERS_REDUCED = ("SpiceLine", "SpiceLine2")
+LTSPICE_ATTRIBUTES = ("InstName", "Def_Sub")
+
+
 class AscEditor(BaseSchematic):
     """Class made to update directly the LTspice ASC files"""
     lib_paths = []  # This is a class variable, so it can be shared between all instances.
     symbol_cache = {}  # This is a class variable, so it can be shared between all instances.
 
-    def __init__(self, asc_file: str):
+    def __init__(self, asc_file: Union[str, Path], encoding='autodetect'):
         super().__init__()
         self.version = 4
         self.sheet = "1 0 0"  # Three values are present on the SHEET clause
         self.asc_file_path = Path(asc_file)
         if not self.asc_file_path.exists():
             raise FileNotFoundError(f"File {asc_file} not found")
+        # determine encoding
+        if encoding == 'autodetect':
+            try:
+                self.encoding = detect_encoding(self.asc_file_path, r'^VERSION ', re_flags=re.IGNORECASE)  # Normally the file will start with 'VERSION '
+            except EncodingDetectError as err:
+                raise err
+        else:
+            self.encoding = encoding        
         # read the file into memory
         self.reset_netlist()
 
     @property
     def circuit_file(self) -> Path:
         return self.asc_file_path
 
     def save_netlist(self, run_netlist_file: Union[str, Path]) -> None:
         if isinstance(run_netlist_file, str):
             run_netlist_file = Path(run_netlist_file)
         run_netlist_file = run_netlist_file.with_suffix(".asc")
-        with open(run_netlist_file, 'w') as asc:
+        with open(run_netlist_file, 'w', encoding=self.encoding) as asc:
             _logger.info(f"Writing ASC file {run_netlist_file}")
 
             asc.write(f"Version {self.version}" + END_LINE_TERM)
             asc.write(f"SHEET {self.sheet}" + END_LINE_TERM)
             for wire in self.wires:
                 asc.write(f"WIRE {wire.V1.X} {wire.V1.Y} {wire.V2.X} {wire.V2.Y}" + END_LINE_TERM)
             for flag in self.labels:
@@ -95,18 +111,25 @@
                 alignment = asc_text_align_get(directive)
                 size = directive.size
                 if directive.type == TextTypeEnum.DIRECTIVE:
                     directive_type = '!'
                 else:
                     directive_type = ';'  # Otherwise assume it is a comment
                 asc.write(f"TEXT {posX} {posY} {alignment} {size} {directive_type}{directive.text}" + END_LINE_TERM)
+            for line in self.lines:
+                line_style = f' {line.style.pattern}' if line.style.pattern != "" else ""
+                asc.write(f"LINE Normal {line.V1.X} {line.V1.Y} {line.V2.X} {line.V2.Y}{line_style}" + END_LINE_TERM)
+            for shape in self.shapes:
+                line_style = f' {shape.line_style.pattern}' if shape.line_style.pattern != "" else ""
+                points = " ".join([f"{point.X} {point.Y}" for point in shape.points])
+                asc.write(f"{shape.name} Normal {points}{line_style}" + END_LINE_TERM)
 
     def reset_netlist(self, create_blank: bool = False) -> None:
         super().reset_netlist()
-        with open(self.asc_file_path, 'r') as asc_file:
+        with open(self.asc_file_path, 'r', encoding=self.encoding) as asc_file:
             _logger.info(f"Parsing ASC file {self.asc_file_path}")
             component = None
             for line in asc_file:
                 if line.startswith("SYMBOL"):
                     tag, symbol, posX, posY, rotation = line.split()
                     if component is not None:
                         assert component.reference is not None, "Component InstName was not given"
@@ -172,17 +195,48 @@
                     assert version in ["4"], f"Unsupported version : {version}"
                     self.version = version
                 elif line.startswith("SHEET "):
                     self.sheet = line[len("SHEET "):].strip()
                 elif line.startswith("IOPIN "):
                     tag, posX, posY, direction = line.split()
                     text = self.labels[-1]  # Assuming it is the last FLAG parsed
-                    assert text.coord.X == int(posX) and text.coord.Y == int(posY), "Syntax Error, getting a IOPIN withou an associated label"
+                    assert text.coord.X == int(posX) and text.coord.Y == int(posY), "Syntax Error, getting a IOPIN without an associated label"
                     port = Port(text, direction)
                     self.ports.append(port)
+                elif line.startswith("LINE") or line.startswith("RECTANGLE") or line.startswith("CIRCLE"):
+                    # format: LINE|RECTANGLE|CIRCLE Normal, x1, y1, x2, y2, [line_style]
+                    # Maybe support something else than 'Normal', but LTSpice does not seem to do so.
+                    line_elements = line.split()
+                    assert len(line_elements) in (6, 7), "Syntax Error, line badly badly formatted"
+                    x1 = int(line_elements[2])
+                    y1 = int(line_elements[3])
+                    x2 = int(line_elements[4])
+                    y2 = int(line_elements[5])
+                    if line.startswith("LINE"):
+                        line = Line(Point(x1, y1), Point(x2, y2))
+                        if len(line_elements) == 7:
+                            line.style.pattern = line_elements[6]
+                        self.lines.append(line)
+                    if line_elements[0] in ("RECTANGLE", "CIRCLE"):
+                        shape = Shape(line_elements[0], [Point(x1, y1), Point(x2, y2)])
+                        if len(line_elements) == 7:
+                            shape.line_style.pattern = line_elements[6]
+                        self.shapes.append(shape)
+
+                elif line.startswith("ARC"):
+                    # I don't support editing yet, so why make it complicated
+                    # format: ARC Normal, x1, y1, x2, y2, x3, y3, x4, y4 [line_style]
+                    # Maybe support something else than 'Normal', but LTSpice does not seem to do so.
+                    line_elements = line.split()
+                    assert len(line_elements) in (10, 11), "Syntax Error, line badly formatted"
+                    points = [Point(int(line_elements[i]), int(line_elements[i + 1])) for i in range(2, 9, 2)]
+                    arc = Shape("ARC", points)
+                    if len(line_elements) == 11:
+                        arc.line_style.pattern = line_elements[10]
+                    self.shapes.append(arc)
                 else:
                     raise NotImplementedError("Primitive not supported for ASC file\n" 
                                               f'"{line}"')
             if component is not None:
                 assert component.reference is not None, "Component InstName was not given"
                 self.components[component.reference] = component
 
@@ -210,14 +264,17 @@
                                                      *self.lib_paths)
             if asc_path is None:
                 raise FileNotFoundError(f"File {asc_filename} not found")
             answer = AscEditor(asc_path)
         elif symbol.symbol_type == "CELL":
             model = symbol.get_model()
             lib = symbol.get_library()
+            if lib is None:
+                # TODO: the library is often specified later on, so this may need to move.
+                return None
             lib_path = self._lib_file_find(lib)
             if lib_path is None:
                 raise FileNotFoundError(f"File {lib} not found")
             answer = SpiceEditor.find_subckt_in_lib(lib_path, model)
         else:
             raise ValueError(f"Symbol type {symbol.symbol_type} not supported")
         return answer
@@ -230,15 +287,15 @@
     def get_component_info(self, reference) -> dict:
         """Returns the reference information as a dictionary"""
         component = self.get_component(reference)
         info = {name: value for name, value in component.attributes.items() if not name.startswith("WINDOW ")}
         info["InstName"] = reference  # For legacy purposes
         return info
 
-    def get_component_position(self, reference: str) -> (Point, ERotation):
+    def get_component_position(self, reference: str) -> Tuple[Point, ERotation]:
         component = self.get_component(reference)
         return component.position, component.rotation
 
     def set_component_position(self, reference: str, position: Point, rotation: ERotation) -> None:
         component = self.get_component(reference)
         component.position = position
         component.rotation = rotation
@@ -250,32 +307,32 @@
             if command_upped_directive.startswith(command_upped):
                 match = search_expression.search(directive.text)
                 if match:
                     return match, directive
         return None, None
 
     def get_parameter(self, param: str) -> str:
-        param_regex = re.compile(PARAM_REGEX % param, re.IGNORECASE)
+        param_regex = re.compile(PARAM_REGEX(param), re.IGNORECASE)
         match, directive = self._get_directive(".PARAM", param_regex)
         if match:
             return match.group('value')
         else:
             raise ParameterNotFoundError(f"Parameter {param} not found in ASC file")
 
     def set_parameter(self, param: str, value: Union[str, int, float]) -> None:
-        param_regex = re.compile(PARAM_REGEX % param, re.IGNORECASE)
+        param_regex = re.compile(PARAM_REGEX(param), re.IGNORECASE)
         match, directive = self._get_directive(".PARAM", param_regex)
         if match:
             _logger.debug(f"Parameter {param} found in ASC file, updating it")
             if isinstance(value, (int, float)):
                 value_str = format_eng(value)
             else:
                 value_str = value
-            start, stop = match.span('replace')
-            directive.text = f"{directive.text[:start]}{param}={value_str}{directive.text[stop:]}"
+            start, stop = match.span('value')
+            directive.text = f"{directive.text[:start]}{value_str}{directive.text[stop:]}"
             _logger.info(f"Parameter {param} updated to {value_str}")
         else:
             # Was not found so we need to add it,
             _logger.debug(f"Parameter {param} not found in ASC file, adding it")
             x, y = self._get_text_space()
             coord = Point(x, y)
             text = f".param {param}={value}"
@@ -316,18 +373,138 @@
         component = self.get_component(element)
         component.symbol = model
         _logger.info(f"Component {element} updated to {model}")
         self.set_updated(element)
 
     def get_component_value(self, element: str) -> str:
         component = self.get_component(element)
-        if "Value" not in component.attributes:
+        values = [component.attributes[param_name] for param_name in ["Value", "Value2"]
+                  if param_name in component.attributes]
+        if len(values) == 0:
             _logger.error(f"Component {element} does not have a Value attribute")
             raise ComponentNotFoundError(f"Component {element} does not have a Value attribute")
-        return component.attributes["Value"]
+        return ' '.join(values)
+
+    def get_component_parameters(self, element: str, as_dicts: bool = False) -> dict:
+        """
+        Returns the parameters of a component that are related with Spice operation.
+        That is: Value, Value2, SpiceModel, SpiceLine, SpiceLine2, plus all contents of SpiceLine, SpiceLine2
+
+        :param element: Reference of the circuit element to get the parameters.
+        :type element: str
+        :param as_dicts: will report the contents of SpiceLine and SpiceLine2 inside a SpiceLine/SpiceLine2 instead of separately.
+        :type as_dicts: bool
+
+        :return: parameters of the circuit element in dictionary format.
+        :rtype: dict
+
+        :raises: ComponentNotFoundError - In case the component is not found
+
+                 NotImplementedError - for not supported operations
+        """
+        component = self.get_component(element)
+        parameters = {}
+        search_regex = re.compile(PARAM_REGEX(r'\w+'), re.IGNORECASE)
+        for key, value in component.attributes.items():
+            if key in LTSPICE_PARAMETERS:
+                parameters[key] = value
+                if key in LTSPICE_PARAMETERS_REDUCED:
+                    # if we have a structured attribute, return the full dict of it
+                    # this is compatible with set_component_parameters
+                    sub_parameters = {}                    
+                    matches = search_regex.findall(value)
+                    if matches:
+                        # This might contain one or more parameters
+                        for param_name, param_value in matches:
+                            sub_parameters[param_name] = try_convert_value(param_value)
+                        if as_dicts:
+                            parameters[key] = sub_parameters
+                        else:
+                            parameters.update(sub_parameters)
+
+        return parameters
+
+    def set_component_parameters(self, element: str, **kwargs) -> None:
+        """
+        Sets the parameters of a component that are related with Spice operation.
+        That is: Value, Value2, SpiceModel, SpiceLine, SpiceLine2, or any parameters are or could be in SpiceLine, SpiceLine2.
+        Unknown parameters will be added to SpiceLine.
+        Setting None removes the parameter if possible.
+
+        Usage 1: ::
+
+         editor.set_component_parameters(R1, value=330, temp=25)
+
+        Usage 2: ::
+
+         value_settings = {'value': 330, 'temp': 25}
+         editor.set_component_parameters(R1, **value_settings)
+
+        :param element: Reference of the circuit element.
+        :type element: str
+
+        :key <param_name>:
+            The key is the parameter name and the value is the value to be set. Values can either be
+            strings; integers or floats. When None is given, the parameter will be removed, if possible.
+
+        :return: Nothing
+        :raises: ComponentNotFoundError - In case one of the component is not found.
+        """
+        component = self.get_component(element)
+        for key, value in kwargs.items():
+            # format the value
+            if value is None:
+                value_str = None
+            elif isinstance(value, str):
+                value_str = value.strip()
+            else:
+                value_str = format_eng(value)               
+            params = self.get_component_parameters(element, as_dicts=True)
+            if key in params:
+                # I only have the LTSPICE_PARAMETERS as keys here, so when I match, i can overwrite
+                # I do not support delete here, as some of the keys are mandatory
+                component.attributes[key] = value_str
+                _logger.info(f"Component {element} updated with parameter {key}:{value}")
+            else:
+                foundme = False
+                # not found: look in the second level dicts
+                for param_key in LTSPICE_PARAMETERS_REDUCED:
+                    if param_key in params:
+                        if key in params[param_key]:
+                            # found in the dict
+                            # update the dict
+                            if value_str is None:
+                                # remove if empty
+                                params[param_key].pop(key)
+                            else:
+                                params[param_key][key] = value_str
+                            # and make the line out of the dict
+                            component.attributes[param_key] = ' '.join([f'{p_key}={p_value}' for p_key, p_value in params[param_key].items()])
+                            _logger.info(f"Component {element} updated with parameter {key}:{value_str}")
+                            foundme = True
+                if not foundme:
+                    if value_str is not None:
+                        # don't add if there's nothing to add
+                        if key in LTSPICE_PARAMETERS:
+                            # known parameter, set the value
+                            component.attributes[key] = value_str
+                            _logger.info(f"Component {element} updated with parameter {key}:{value_str}")
+                        else:
+                            # nothing found, and not a known parameter, put it in SpiceLine
+                            param_key = LTSPICE_PARAMETERS_REDUCED[0]
+                            if param_key in params:
+                                # if SpiceLine exists: add to the dict
+                                params[param_key][key] = value_str
+                                # and make the line out of the dict
+                                component.attributes[param_key] = ' '.join([f'{p_key}={p_value}' for p_key, p_value in params[param_key].items()])
+                            else:
+                                # if SpiceLine does not exist: create the line
+                                component.attributes[param_key] = f'{key}={value_str}'
+                            _logger.info(f"Component {element} updated with parameter {key}:{value_str}")
+        self.set_updated(element)
 
     def get_components(self, prefixes='*') -> list:
         if prefixes == '*':
             return list(self.components.keys())
         return [k for k in self.components.keys() if k[0] in prefixes]
 
     def remove_component(self, designator: str):
@@ -377,32 +554,32 @@
         file_found = search_file_in_containers(filename, *self.lib_paths)  # The library paths
         if file_found is None:
             file_found = search_file_in_containers(filename,
                                                    os.path.split(self.asc_file_path)[0],
                                                    os.path.curdir,  # The current script directory,
                                                    os.path.split(self.asc_file_path)[0],
                                                    # The directory where the script is located
-                                                   os.path.expanduser(r"~\AppData\Local\LTspice\lib\sub"),
-                                                   os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sub"),
-                                                   os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"),
+                                                   os.path.expanduser("~/AppData/Local/LTspice/lib/sub"),
+                                                   os.path.expanduser("~/Documents/LtspiceXVII/lib/sub"),
+                                                   os.path.expanduser("~/AppData/Local/Programs/ADI/LTspice/lib.zip"),
                                                    )
         return file_found
 
     def _asy_file_find(self, filename) -> Optional[str]:
         if filename in self.symbol_cache:
             return self.symbol_cache[filename]
         _logger.info(f"Searching for symbol {filename}...")
         file_found = search_file_in_containers(filename, *self.lib_paths)
         if file_found is None:
             file_found = search_file_in_containers(filename,
                                                    os.path.curdir,  # The current script directory
                                                    os.path.split(self.asc_file_path)[0],
                                                    # The directory where the script is located
-                                                   os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
-                                                   os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sym"),
+                                                   os.path.expanduser("~/AppData/Local/LTspice/lib/sym"),
+                                                   os.path.expanduser("~/Documents/LtspiceXVII/lib/sym"),
                                                    )
         if file_found is not None:
             self.symbol_cache[filename] = file_found
         return file_found
 
     def add_instruction(self, instruction: str) -> None:
         # docstring inherited from BaseEditor
@@ -411,14 +588,15 @@
 
         if set_command in UNIQUE_SIMULATION_DOT_INSTRUCTIONS:
             # Before adding new instruction, if it is a unique instruction, we just replace it
             i = 0
             while i < len(self.directives):
                 directive = self.directives[i]
                 if directive.type == TextTypeEnum.COMMENT:
+                    i += 1
                     continue  # this is a comment
                 directive_command = directive.text.split()[0].upper()
                 if directive_command in UNIQUE_SIMULATION_DOT_INSTRUCTIONS:
                     directive.text = instruction
                     self.updated = True
                     return  # Job done, can exit this method
                 i += 1
```

### Comparing `spicelib-1.1.2/spicelib/editor/asy_reader.py` & `spicelib-1.1.3/spicelib/editor/asy_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 #  ██╔════╝██╔══██╗██║██╔════╝██╔════╝██║     ██║██╔══██╗
 #  ███████╗██████╔╝██║██║     █████╗  ██║     ██║██████╔╝
 #  ╚════██║██╔═══╝ ██║██║     ██╔══╝  ██║     ██║██╔══██╗
 #  ███████║██║     ██║╚██████╗███████╗███████╗██║██████╔╝
 #  ╚══════╝╚═╝     ╚═╝ ╚═════╝╚══════╝╚══════╝╚═╝╚═════╝
 #
 # Name:        asy_reader.py
-# Purpose:     Class to parse and then translate LTspice symbol files
+# Purpose:     Class to parse and then translate LTSpice symbol files
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 import logging
 from collections import OrderedDict
 from pathlib import Path
 from typing import Union
 
-from .base_schematic import Point, Text, TextTypeEnum, Line, Circle, Rectangle, Arc, HorAlign, ERotation, VerAlign
+from .base_schematic import Point, Text, TextTypeEnum, Line, Shape, HorAlign, ERotation, VerAlign
 from .ltspice_utils import asc_text_align_set
 
 from .qsch_editor import QschTag
 
 _logger = logging.getLogger("spicelib.AsyReader")
 SCALE_X = 6.25
 SCALE_Y = - 6.25
@@ -37,17 +37,15 @@
 
     def __init__(self, asy_file: Union[Path, str]):
         super().__init__()
         self.version = 4
         self.symbol_type = None
         self.pins = []
         self.lines = []
-        self.arcs = []
-        self.circles = []
-        self.rectangles = []
+        self.shapes = []
         self.attributes = OrderedDict()
         self._asy_file_path = Path(asy_file)
         self.windows = []
         pin = None
         if not self._asy_file_path.exists():
             raise FileNotFoundError(f"File {asy_file} not found")
         with open(self._asy_file_path, 'r') as asc_file:
@@ -70,29 +68,30 @@
                         continue
                     text = text.strip()  # Gets rid of the \n terminator
                     self.attributes[ref] = text
                 elif line.startswith("LINE"):
                     tag, weight, x1, y1, x2, y2 = line.split()
                     v1 = Point(int(x1), int(y1))
                     v2 = Point(int(x2), int(y2))
-                    segment = Line(v1, v2, style=f"{{weight:{weight}}}")
+                    segment = Line(v1, v2)
+                    segment.style.weight = f"{weight}"
                     self.lines.append(segment)
                 elif line.startswith("CIRCLE"):
                     tag, weight, x1, y1, x2, y2 = line.split()
-                    # In LTspice the circle is set using the top left and bottom right points of the rectangle that
+                    # In LTSpice the circle is set using the top left and bottom right points of the rectangle that
                     # encloses the circle
                     x1 = int(x1)
                     x2 = int(x2)
                     y1 = int(y1)
                     y2 = int(y2)
                     # distance = (x2-x1)  # Always assuming a circle
                     # circle = Arc(Point((x1+x2)/2, (y1+y2)/2), radius=distance/2, start_angle=0, stop_angle=360,
                     #              style=f"{{style:1, weight:{weight}}}")
-                    circle = Circle(Point(x1, y1), Point(x2, y2))
-                    self.circles.append(circle)
+                    circle = Shape("CIRCLE", [Point(x1, y1), Point(x2, y2)])
+                    self.shapes.append(circle)
                 elif line.startswith("Version"):
                     tag, version = line.split()
                     assert version in ["4"], f"Unsupported version : {version}"
                     self.version = version
                 elif line.startswith("SymbolType "):
                     self.symbol_type = line[len("SymbolType "):].strip()
                 elif line.startswith("PINATTR"):
@@ -128,41 +127,41 @@
                             elif justification == "RIGHT":
                                 text_alignment = HorAlign.RIGHT
                             # else: justification == "LEFT" (default)
 
                     pin = Text(coord, "", type=TextTypeEnum.PIN, size=int(offset),
                                textAlignment=text_alignment, verticalAlignment=vertical_alignment, angle=angle)
                 elif line.startswith("ARC"):
-                    tag, weight, x1, y1, x2, y2, x3, y3, x4, y4  = line.split()
+                    tag, weight, x1, y1, x2, y2, x3, y3, x4, y4 = line.split()
                     x1 = int(x1)
                     x2 = int(x2)
                     x3 = int(x3)
                     x4 = int(x4)
                     y1 = int(y1)
                     y2 = int(y2)
                     y3 = int(y3)
                     y4 = int(y4)
 
                     center = Point((x1+x2)//2, (y1+y2)//2)
-                    radius = abs(x2-x1)/2  # Using only the X axis. Assuming a circle not an elipse
+                    radius = abs(x2-x1)/2  # Using only the X axis. Assuming a circle not an ellipse
                     start = Point((x3-center.X)/radius, (y3-center.Y)/radius)
                     stop = Point((x4-center.X)/radius, (y4-center.Y)/radius)
-                    arc = Arc(center, radius=radius, start=start, stop=stop)
-                    self.arcs.append(arc)
+                    arc = Shape("ARC", [center, start, stop])
+                    self.shapes.append(arc)
                 elif line.startswith("RECTANGLE"):
                     tag, weight, x1, y1, x2, y2 = line.split()
                     x1 = int(x1)
                     x2 = int(x2)
                     y1 = int(y1)
                     y2 = int(y2)
-                    rect = Rectangle(Point(x1, y1), Point(x2, y2))
-                    self.rectangles.append(rect)
+                    rect = Shape("RECTANGLE", [Point(x1, y1), Point(x2, y2)])
+                    self.shapes.append(rect)
                 else:
                     print("Primitive not supported for ASC file\n"
-                                              f'"{line}"')
+                          f'"{line}"')
             if pin is not None:
                 self.pins.append(pin)
 
     def to_qsch(self, *args):
         """Create a QschTag representing a component symbol."""
         spice_prefix = self.attributes['Prefix']
         symbol = QschTag("symbol", spice_prefix[0])
@@ -174,50 +173,45 @@
             y1 = int(line.V1.Y * SCALE_Y)
             x2 = int(line.V2.X * SCALE_X)
             y2 = int(line.V2.Y * SCALE_Y)
             segment, _ = QschTag.parse(
                 f"«line ({x1},{y1}) ({x2},{y2}) 0 0 0x1000000 -1 -1»")
             symbol.items.append(segment)
 
-        for circle in self.circles:
-            # x1 = int((arc.center.X - arc.radius) * SCALE_X)
-            # y1 = int((arc.center.Y - arc.radius) * SCALE_Y)
-            # x2 = int((arc.center.X + arc.radius) * SCALE_X)
-            # y2 = int((arc.center.Y + arc.radius) * SCALE_Y)
-            x1 = int(circle.V1.X * SCALE_X)
-            y1 = int(circle.V1.Y * SCALE_Y)
-            x2 = int(circle.V2.X * SCALE_X)
-            y2 = int(circle.V2.Y * SCALE_Y)
-            elipse_tag, _ = QschTag.parse(
-                f"«ellipse ({x1},{y1}) ({x2},{y2}) 0 0 0 0x1000000 0x1000000 -1 -1»"
-            )
-            symbol.items.append(elipse_tag)
-
-        for rectangle in self.rectangles:
-            x1 = int(rectangle.V1.X * SCALE_X)
-            y1 = int(rectangle.V1.Y * SCALE_Y)
-            x2 = int(rectangle.V2.X * SCALE_X)
-            y2 = int(rectangle.V2.Y * SCALE_Y)
-            rectangle_tag, _ = QschTag.parse(
-                f"«rect ({x1},{y1}) ({x2},{y2}) 0 0 0 0x4000000 0x1000000 -1 0 -1»"
-            )
-            symbol.items.append(rectangle_tag)
-
-        for arc in self.arcs:
-            cx = int(arc.center.X * SCALE_X)
-            cy = int(arc.center.Y * SCALE_Y)
-            x1 = int((arc.center.X + arc.start.X * arc.radius) * SCALE_X)
-            y1 = int((arc.center.Y + arc.start.Y * arc.radius) * SCALE_Y)
-            x2 = int((arc.center.X + arc.stop.X * arc.radius) * SCALE_X)
-            y2 = int((arc.center.Y + arc.stop.Y * arc.radius) * SCALE_Y)
-
-            elipse_tag, _ = QschTag.parse(
-                f"«arc3p ({x1},{y1}) ({x2},{y2}) ({cx},{cy}) 0 0 0xff0000 -1 -1»"
-            )
-            symbol.items.append(elipse_tag)
+        for shape in self.shapes:
+            if shape.name == "RECTANGLE":
+                x1 = int(shape.points[0].X * SCALE_X)
+                y1 = int(shape.points[0].Y * SCALE_Y)
+                x2 = int(shape.points[1].X * SCALE_X)
+                y2 = int(shape.points[1].Y * SCALE_Y)
+                shape_tag, _ = QschTag.parse(
+                    f"«rect ({x1},{y1}) ({x2},{y2}) 0 0 0 0x4000000 0x1000000 -1 0 -1»"
+                )
+            elif shape.name == "ARC":
+                x1 = int(shape.points[0].X * SCALE_X)
+                y1 = int(shape.points[0].Y * SCALE_Y)
+                x2 = int(shape.points[1].X * SCALE_X)
+                y2 = int(shape.points[1].Y * SCALE_Y)
+                x3 = int(shape.points[2].X * SCALE_X)
+                y3 = int(shape.points[2].Y * SCALE_Y)
+                shape_tag, _ = QschTag.parse(
+                    f"«arc3p ({x1},{y1}) ({x2},{y2}) ({x3},{y3}) 0 0 0xff0000 -1 -1»"
+                )
+            elif shape.name == "CIRCLE" or shape.name == "ellipse":
+                x1 = int(shape.points[0].X * SCALE_X)
+                y1 = int(shape.points[0].Y * SCALE_Y)
+                x2 = int(shape.points[1].X * SCALE_X)
+                y2 = int(shape.points[1].Y * SCALE_Y)
+                shape_tag, _ = QschTag.parse(
+                    f"«ellipse ({x1},{y1}) ({x2},{y2}) 0 0 0 0x1000000 0x1000000 -1 -1»"
+                )
+            else:
+                raise ValueError(f"Shape {shape.name} not supported")
+            symbol.items.append(shape_tag)
+
         for i, attr in enumerate(self.windows):
             coord = attr.coord
             x = coord.X * SCALE_X
             y = coord.Y * SCALE_Y
             text, _ = QschTag.parse(f'«text ({x :.0f},{y :.0f})'
                                     f' 1 7 0 0x1000000 -1 -1 "{args[i]}"»')
             symbol.items.append(text)
@@ -240,17 +234,16 @@
         return self.symbol_type == 'BLOCK' or self.attributes.get('Prefix') == 'X'
 
     def get_library(self) -> str:
         """Returns the library name of the model. If not found, returns None."""
         # Searching in this exact order
         for attr in ('ModelFile', 'SpiceModel', 'SpiceLine', 'SpiceLine2', 'Def_Sub', 'Value', 'Value2'):
             if attr in self.attributes and (self.attributes[attr].endswith('.lib') or
-                        self.attributes[attr].endswith('.sub') or
-                        self.attributes[attr].endswith('.cir')
-            ):
+                                            self.attributes[attr].endswith('.sub') or
+                                            self.attributes[attr].endswith('.cir')):
                 return self.attributes[attr]
         return self.attributes.get('SpiceModel')
 
     def get_model(self) -> str:
         """Returns the model name of the component. If not found, returns None."""
         # Searching in this exact order
         for attr in ('Value', 'SpiceModel', 'Value2', 'ModelFile', 'SpiceLine', 'SpiceLine2', 'Def_Sub', ):
@@ -271,9 +264,9 @@
                 ans = float(value)
             except ValueError:
                 ans = value.strip()  # Removes the leading trailing spaces
         return ans
 
     def get_schematic_file(self):
         assert self._asy_file_path.suffix == '.asy', "File is not an asy file"
-        assert self.symbol_type == 'BLOCK', "File is not a subcircuit"
+        assert self.symbol_type == 'BLOCK', "File is not a sub-circuit"
         return self._asy_file_path.with_suffix('.asc')
```

### Comparing `spicelib-1.1.2/spicelib/editor/base_editor.py` & `spicelib-1.1.3/spicelib/editor/base_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,27 +62,32 @@
     '.SAVEBIAS',
     '.STEP',
     '.SUBCKT',
     '.TEXT',
     '.WAVE',  # Write Selected Nodes to a .Wav File
 
 )
-PARAM_REGEX = r"(?<= )(?P<replace>%s(\s*=\s*)(?P<value>[\w\*\/\.\+\-\/\*\{\}\(\)\t ]*))(?<!\s)($|\s+)(?!\s*=)"
+
+
+def PARAM_REGEX(pname):
+    return r"(?P<name>" + pname + r")\s*[= ]\s*(?P<value>[\w\*\/\.\+\-\/\*\{\}\(\)%]*)"
 
 
 def format_eng(value) -> str:
     """
     Helper function for formatting value with the SI qualifiers.  That is, it will use
 
         * p for pico (10E-12)
         * n for nano (10E-9)
         * u for micro (10E-6)
         * m for mili (10E-3)
         * k for kilo (10E+3)
         * Meg for Mega (10E+6)
+        * g for giga (10E+9)
+        * t for tera (10E+12)
 
 
     :param value: float value to format
     :type value: float
     :return: String with the formatted value
     :rtype: str
     """
@@ -93,31 +98,37 @@
         suffix = "fpnum"[e]
     elif e == 0:
         return "{:g}".format(value)
     elif e == 1:
         suffix = "k"
     elif e == 2:
         suffix = 'Meg'
+    elif e == 3:
+        suffix = 'g'
+    elif e == 4:
+        suffix = 't'
     else:
         return '{:E}'.format(value)
     return '{:g}{:}'.format(value * 1000 ** -e, suffix)
 
 
 def scan_eng(value: str) -> float:
     """
     Converts a string to a float, considering SI multipliers
 
         * f for femto (10E-15)
         * p for pico (10E-12)
         * n for nano (10E-9)
         * u or µ for micro (10E-6)
         * m for mili (10E-3)
-        * k or K for kilo (10E+3)
-        * Meg for Mega (10E+6)
-
+        * k for kilo (10E+3)
+        * meg for Mega (10E+6)
+        * g for giga (10E+9)
+        * t for tera (10E+12)
+        
     The extra unit qualifiers such as V for volts or F for Farads are ignored.
 
 
     :param value: string to be converted to float
     :type value: str
     :return:
     :rtype: float
@@ -129,27 +140,30 @@
     while x > 0:
         if value[x - 1] in "0123456789":
             break
         x -= 1
     suffix = value[x:]  # this is the non-numeric part at the end
     f = float(value[:x])  # this is the numeric part. Can raise ValueError.
     if suffix:
-        if suffix[0] in "fpnuµmkK":
+        suffix = suffix.lower()
+        # By industry convention, SPICE is not case sensitive
+        if suffix.startswith("meg"):
+            return f * 1E+6
+        elif suffix[0] in "fpnuµmkgt":
             return f * {
                 'f': 1.0e-15,
                 'p': 1.0e-12,
                 'n': 1.0e-09,
                 'u': 1.0e-06,
                 'µ': 1.0e-06,
                 'm': 1.0e-03,
                 'k': 1.0e+03,
-                'K': 1.0e+03,  # LTSpice uses the capital K for Kilo
+                'g': 1.0e+09,
+                't': 1.0e+12,
             }[suffix[0]]
-        elif suffix.upper().startswith("MEG"):
-            return f * 1E+6
     return f
 
 
 class ComponentNotFoundError(Exception):
     """Component Not Found Error"""
 
 
@@ -216,15 +230,17 @@
 
     @abstractmethod
     def get_subcircuit(self, reference: str) -> 'BaseEditor':
         """Returns a hierarchical subdesign"""
         ...
 
     def get_component_attribute(self, reference: str, attribute: str) -> str:
-        """Returns the value of the attribute of the component.
+        """Returns the value of the attribute of the component. Attributes are the values that are not related with
+        SPICE parameters. For example, component manufacturer, footprint, schematic appearance, etc.
+        User can define whatever attributes they want. The only restriction is that the attribute name must be a string.
         :param reference: Reference of the component
         :type reference: str
         :param attribute: Name of the attribute to be retrieved
         :type attribute: str
         :return: Value of the attribute being sought
         :rtype: str
         :raises: ComponentNotFoundError - In case the component is not found
@@ -310,25 +326,25 @@
         """
         for param in kwargs:
             self.set_parameter(param, kwargs[param])
 
     @abstractmethod
     def set_component_value(self, device: str, value: Union[str, int, float]) -> None:
         """Changes the value of a component, such as a Resistor, Capacitor or Inductor. For components inside
-        subcircuits, use the subcirciut designator prefix with ':' as separator (Example X1:R1)
+        sub-circuits, use the sub-circuit designator prefix with ':' as separator (Example X1:R1)
         Usage: ::
 
             editor.set_component_value('R1', '3.3k')
             editor.set_component_value('X1:C1', '10u')
 
         :param device: Reference of the circuit element to be updated.
         :type device: str
         :param value:
-            value to be be set on the given circuit element. Float and integer values will automatically
-            formatted as per the engineering notations 'k' for kilo, 'm', for mili and so on.
+            value to be set on the given circuit element. Float and integer values will automatically
+            formated as per the engineering notations 'k' for kilo, 'm', for mili and so on.
         :type value: str, int or float
         :raises:
             ComponentNotFoundError - In case the component is not found
 
             ValueError - In case the value doesn't correspond to the expected format
 
             NotImplementedError - In case the circuit element is defined in a format which is not supported by this
@@ -359,14 +375,56 @@
             NotImplementedError - In case the circuit element is defined in a format which is not supported by this version.
 
             If this is the case, use GitHub to start a ticket.  https://github.com/nunobrum/spicelib
         """
         ...
 
     @abstractmethod
+    def set_component_parameters(self, element: str, **kwargs) -> None:
+        """
+        Adds one or more parameters to the component on the netlist. The argument is in the form of a key-value pair
+        where each parameter is the key and the value is value to be set in the netlist.
+
+        Usage 1: ::
+
+         editor.set_component_parameters(R1, value=330, temp=25)
+
+        Usage 2: ::
+
+         value_settings = {'value': 330, 'temp': 25}
+         editor.set_component_parameters(R1, **value_settings)
+
+        :param element: Reference of the circuit element.
+        :type element: str
+
+        :key <param_name>:
+            The key is the parameter name and the value is the value to be set. Values can either be
+            strings; integers or floats. When None is given, the parameter will be removed, if possible.
+
+        :return: Nothing
+        :raises: ComponentNotFoundError - In case one of the component is not found.
+        """
+        ...
+
+    def set_component_attribute(self, reference: str, attribute: str, value: str) -> None:
+        """Sets the value of the attribute of the component. Attributes are the values that are not related with
+        SPICE parameters. For example, component manufacturer, footprint, schematic appearance, etc.
+        User can define whatever attributes they want. The only restriction is that the attribute name must be a string.
+        :param reference: Reference of the component
+        :type reference: str
+        :param attribute: Name of the attribute to be set
+        :type attribute: str
+        :param value: Value of the attribute to be set
+        :type value: str
+        :return: Nothing
+        :raises: ComponentNotFoundError - In case the component is not found
+        """
+        self.get_component(reference).attributes[attribute] = value
+
+    @abstractmethod
     def get_component_value(self, element: str) -> str:
         """
         Returns the value of a component retrieved from the netlist.
 
         :param element: Reference of the circuit element to get the value.
         :type element: str
 
@@ -375,14 +433,31 @@
 
         :raises: ComponentNotFoundError - In case the component is not found
 
                  NotImplementedError - for not supported operations
         """
         ...
 
+    @abstractmethod
+    def get_component_parameters(self, element: str) -> dict:
+        """
+        Returns the parameters of a component retrieved from the netlist.
+
+        :param element: Reference of the circuit element to get the parameters.
+        :type element: str
+
+        :return: parameters of the circuit element in dictionary format.
+        :rtype: dict
+
+        :raises: ComponentNotFoundError - In case the component is not found
+
+                 NotImplementedError - for not supported operations
+        """
+        ...
+
     def get_component_floatvalue(self, element: str) -> float:
         """
         Returns the value of a component retrieved from the netlist.
 
         :param element: Reference of the circuit element to get the value in float format.
         :type element: str
 
@@ -514,15 +589,15 @@
         instructions to be removed. The search pattern will be applied to each line of the netlist and if the pattern
         matches, the line will be removed.
 
         Example: The code below will remove all AC analysis instructions from the netlist.
 
         .. code-block:: python
 
-            editor.remove_Xinstruction("\.AC.*")
+            editor.remove_Xinstruction("\\.AC.*")
 
         :param search_pattern: The list of instructions to remove. Each instruction is of the type 'str'
         :type search_pattern: str
         :returns: Nothing
         """
         ...
```

### Comparing `spicelib-1.1.2/spicelib/editor/base_schematic.py` & `spicelib-1.1.3/spicelib/editor/base_schematic.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 
 import dataclasses
 import enum
-from typing import List, Callable, Union
+from typing import List, Callable, Union, Tuple
 from collections import OrderedDict
 import logging
 from .base_editor import BaseEditor, Component, ComponentNotFoundError, SUBCKT_DIVIDER
 
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2021, Fribourg Switzerland"
 
@@ -130,28 +130,38 @@
     COMMENT = enum.auto()
     DIRECTIVE = enum.auto()
     LABEL = enum.auto()
     ATTRIBUTE = enum.auto()
     PIN = enum.auto()  # pin label
 
 
-@dataclasses.dataclass
+class LineStyle:
+    def __init__(self, width: str = "", color: str = "", pattern: str = ""):
+        self.width: str = width
+        self.color: str = color
+        self.pattern: str = pattern
+
+
 class Point:
     """X, Y coordinates"""
-    X: float
-    Y: float
+    def __init__(self, X: float, Y: float):
+        self.X = X
+        self.Y = Y
 
 
-@dataclasses.dataclass
 class Line:
     """X1, Y1, X2, Y2 coordinates"""
-    V1: Point
-    V2: Point
-    style: str = ""
-    net: str = ""
+    def __init__(self, v1: Point, v2: Point, style: LineStyle = None, net: str = ""):
+        self.V1 = v1
+        self.V2 = v2
+        if style is None:
+            self.style = LineStyle()
+        else:
+            self.style = style
+        self.net = net
 
     def touches(self, point: Point) -> bool:
         """Returns True if the line passes through the given point"""
         if self.V1.X == self.V2.X:
             if self.V1.X == point.X:
                 if min(self.V1.Y, self.V2.Y) <= point.Y <= max(self.V1.Y, self.V2.Y):
                     return True
@@ -183,42 +193,64 @@
             return True
         # We also have to check if the given line touches any of the vertices of this line
         if line.touches(self.V1) or line.touches(self.V2):
             return True
         return False
 
 
-Rectangle = Line  # Rectangles have the same properties as Line: Defined as the line that crosses two opposing vertices
-Circle = Line  # Circles are defined by the rectangle that touches 4 points of a circle.
-
+class Shape:
+    """Polygon object. The shape is defined by a list of points. It can define a closed or open shape.
+    The closed shape is defined by the first and last points being the same. In this case, it can have a fill.
+    It is used to define polygons, arcs, circles or more complex shapes like the ones found in QSPICE"""
+    def __init__(self, name: str, points: List[Point], line_style: LineStyle = None, fill: str = ""):
+        self.name = name
+        self.points = points
+        if line_style is None:
+            self.line_style = LineStyle()
+        else:
+            self.line_style = line_style
+        self.fill = fill
 
-@dataclasses.dataclass
-class Arc:
-    """Opting for a non-native representation of the arc as LTspice and Qspice have different
-    ways of storing Arc information. Start and Stop points are calculated as a fraction of the radius
-    for X and Y. This avoids having to deal with the calculation of sines and cosines and their inverse
-    into radians."""
-    center: Point
-    radius: float
-    start: Point
-    stop: Point
-    style: str = ""
-    # The Arcs are decorative, they don't have associated nets
+# Rectangle = Shape
+# Rectangle is a special case of a Shape. Rectangle is defined by two points that define the diagonal
+# of the rectangle.
+
+# Circle = Shape  # Circle is a special case of a Shape. Circle is defined by the rectangle that encloses it.
+
+# Arc = Shape
+# Arc is a special case of a Shape. Since different tools have different ways of defining arcs, we will use
+# # the Shape class to define them. We will only store the list of points that are provided by the tool.
+
+#  TODO: The following code is commented out because it is not used in the current implementation. It is kept here for
+# when we decode how ARCs are stored and we could use it to update them.
+# @dataclasses.dataclass
+# class Arc:
+#     """Opting for a non-native representation of the arc as LTspice and Qspice have different
+#     ways of storing Arc information. Start and Stop points are calculated as a fraction of the radius
+#     for X and Y. This avoids having to deal with the calculation of sines and cosines and their inverse
+#     into radians."""
+#     center: Point
+#     radius: float
+#     start: Point = Point(0, 0)
+#     stop: Point = Point(0, 0)
+#     style: LineStyle = LineStyle()
+#     # The Arcs are decorative, they don't have associated nets
 
 
 @dataclasses.dataclass
 class Text:
     """Text object"""
     coord: Point
     text: str
     size: int = 1
     type: TextTypeEnum = TextTypeEnum.NULL
     textAlignment: HorAlign = HorAlign.LEFT
     verticalAlignment: VerAlign = VerAlign.CENTER
     angle: ERotation = ERotation.R0
+    visible: bool = True
 
 
 @dataclasses.dataclass
 class Port:
     text: Text
     direction: str
 
@@ -241,34 +273,40 @@
 
     def __init__(self):
         self.components: OrderedDict[str, SchematicComponent] = OrderedDict()
         self.wires: List[Line] = []
         self.labels: List[Text] = []
         self.directives: List[Text] = []
         self.ports: List[Port] = []
+        self.lines: List[Line] = []
+        self.shapes: List[Shape] = []
         self.updated = False  # indicates if an edit was done and the file has to be written back to disk
 
     def reset_netlist(self, create_blank: bool = False) -> None:
         """Resets the netlist to the original state"""
         self.components.clear()
         self.wires.clear()
         self.labels.clear()
         self.directives.clear()
+        self.lines.clear()
+        self.shapes.clear()
         self.updated = False
 
     def copy_from(self, editor: 'BaseSchematic') -> None:
         """Clones the contents of the given editor"""
         from copy import deepcopy
         self.components = deepcopy(editor.components)
         self.wires = deepcopy(editor.wires)
         self.labels = deepcopy(editor.labels)
         self.directives = deepcopy(editor.directives)
+        self.lines = deepcopy(editor.lines)
+        self.shapes = deepcopy(editor.shapes)
         self.updated = True
 
-    def _get_parent(self, reference) -> ("BaseSchematic", str):
+    def _get_parent(self, reference) -> Tuple["BaseSchematic", str]:
         if SUBCKT_DIVIDER in reference:
             sub_ref, sub_comp = reference.split(SUBCKT_DIVIDER, 1)
 
             subckt = self.get_component(sub_ref)
             subcircuit = subckt.attributes['_SUBCKT']
             return subcircuit, sub_comp
         else:
@@ -292,15 +330,15 @@
             return sub_circuit.get_component(ref)
         else:
             if ref not in sub_circuit.components:
                 _logger.error(f"Component {reference} not found")
                 raise ComponentNotFoundError(f"Component {reference} not found in Schematic file")
             return sub_circuit.components[ref]
 
-    def get_component_position(self, reference: str) -> (Point, ERotation):
+    def get_component_position(self, reference: str) -> Tuple[Point, ERotation]:
         """Returns the position and rotation of the component"""
         comp = self.get_component(reference)
         return comp.position, comp.rotation
 
     def set_component_position(self, reference: str, position: Point, rotation: ERotation) -> None:
         """Sets the position and rotation of the component.
 
@@ -341,8 +379,20 @@
             wire.V2.Y = round_fun(wire.V2.Y * scale_y + offset_y)
         for label in self.labels:
             label.coord.X = round_fun(label.coord.X * scale_x + offset_x)
             label.coord.Y = round_fun(label.coord.Y * scale_y + offset_y)
         for directive in self.directives:
             directive.coord.X = round_fun(directive.coord.X * scale_x + offset_x)
             directive.coord.Y = round_fun(directive.coord.Y * scale_y + offset_y)
+        for port in self.ports:
+            port.text.coord.X = round_fun(port.text.coord.X * scale_x + offset_x)
+            port.text.coord.Y = round_fun(port.text.coord.Y * scale_y + offset_y)
+        for line in self.lines:
+            line.V1.X = round_fun(line.V1.X * scale_x + offset_x)
+            line.V1.Y = round_fun(line.V1.Y * scale_y + offset_y)
+            line.V2.X = round_fun(line.V2.X * scale_x + offset_x)
+            line.V2.Y = round_fun(line.V2.Y * scale_y + offset_y)
+        for shape in self.shapes:
+            for point in shape.points:
+                point.X = round_fun(point.X * scale_x + offset_x)
+                point.Y = round_fun(point.Y * scale_y + offset_y)
         self.updated = True
```

### Comparing `spicelib-1.1.2/spicelib/editor/ltspice_utils.py` & `spicelib-1.1.3/spicelib/editor/ltspice_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,20 +19,23 @@
 # -------------------------------------------------------------------------------
 
 import re
 
 from .base_schematic import ERotation, Text, HorAlign, VerAlign
 
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
-__copyright__ = "Copyright 2021, Fribourg Switzerland"
+__copyright__ = "Copyright 2024, Fribourg Switzerland"
 
 
 # Regular expressions
-TEXT_REGEX = re.compile(r"TEXT (-?\d+)\s+(-?\d+)\s+(Left|Right|Top|Bottom)\s(\d+)\s*(?P<type>[!;])(?P<text>.*)",
-                        re.IGNORECASE)
+TEXT_REGEX = re.compile(
+    r"TEXT (-?\d+)\s+(-?\d+)\s+V?(Left|Right|Top|Bottom|Center|Invisible)\s(\d+)\s*(?P<type>[!;])(?P<text>.*)",
+    re.IGNORECASE
+)
+
 TEXT_REGEX_X = 1
 TEXT_REGEX_Y = 2
 TEXT_REGEX_ALIGN = 3
 TEXT_REGEX_SIZE = 4
 TEXT_REGEX_TYPE = 5
 TEXT_REGEX_TEXT = 6
 END_LINE_TERM = "\n"
@@ -59,49 +62,56 @@
     'SpiceLine2': 40,
 }
 LT_ATTRIBUTE_NUMBERS_INV = {val: key for key, val in LT_ATTRIBUTE_NUMBERS.items()}
 WEIGHT_CONVERSION_TABLE = ('Thin', 'Normal', 'Thick')
 
 
 def asc_text_align_set(text: Text, alignment: str):
-    if alignment == 'Left':
+    """Sets the alignment of the text in the ASC format"""
+    # Default
+    text.textAlignment = HorAlign.CENTER
+    text.verticalAlignment = VerAlign.CENTER
+    if alignment == 'Left' or alignment == 'VLeft':
         text.textAlignment = HorAlign.LEFT
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'Center':
-        text.textAlignment = HorAlign.CENTER
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'Right':
+    elif alignment == 'Center' or alignment == 'VCenter':
+        pass
+    elif alignment == 'Right' or alignment == 'VRight':
         text.textAlignment = HorAlign.RIGHT
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'VTop':
-        text.textAlignment = HorAlign.CENTER
+    elif alignment == 'Top' or alignment == 'VTop':
         text.verticalAlignment = VerAlign.TOP
-    elif alignment == 'VCenter':
-        text.textAlignment = HorAlign.CENTER
-        text.verticalAlignment = VerAlign.CENTER
-    elif alignment == 'VBottom':
-        text.textAlignment = HorAlign.LEFT
+    elif alignment == 'Bottom' or alignment == 'VBottom':
         text.verticalAlignment = VerAlign.BOTTOM
+    elif alignment == 'Invisible' or alignment == 'VInvisible':
+        text.visible = False
     else:
-        # Default
-        text.textAlignment = HorAlign.LEFT
-        text.verticalAlignment = VerAlign.CENTER
+        raise ValueError(f"Invalid alignment {alignment}")
+
+    if alignment.startswith('V'):
+        text.angle = ERotation.R90
+    else:
+        text.angle = ERotation.R0
     return text
 
 
 def asc_text_align_get(text: Text) -> str:
-    if text.verticalAlignment == VerAlign.CENTER:
-        if text.textAlignment == HorAlign.RIGHT:
-            return 'Right'
-        elif text.textAlignment == HorAlign.CENTER:
-            return 'Center'
-        else:
-            return 'Left'
+    """Returns the alignment of the text in the ASC format"""
+    if not text.visible:
+        ans = 'Invisible'
     else:
-        if text.verticalAlignment == VerAlign.TOP:
-            return 'VTop'
-        elif text.verticalAlignment == VerAlign.CENTER:
-            return 'VCenter'
-        elif text.verticalAlignment == VerAlign.BOTTOM:
-            return 'VBottom'
+        if text.verticalAlignment == VerAlign.CENTER:
+            if text.textAlignment == HorAlign.RIGHT:
+                ans = 'Right'
+            elif text.textAlignment == HorAlign.CENTER:
+                ans = 'Center'
+            else:
+                ans = 'Left'
         else:
-            return 'Left'
+            if text.verticalAlignment == VerAlign.TOP:
+                ans = 'Top'
+            elif text.verticalAlignment == VerAlign.BOTTOM:
+                ans = 'Bottom'
+            else:            
+                ans = 'Left'
+
+    if text.angle == ERotation.R90:
+        ans = 'V' + ans
+    return ans
```

### Comparing `spicelib-1.1.2/spicelib/editor/qsch_editor.py` & `spicelib-1.1.3/spicelib/editor/qsch_editor.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import math
 import os
 import sys
 from collections import OrderedDict
 from pathlib import Path
-from typing import Union, List, Optional, IO, TextIO
+from typing import Union, List, Optional, TextIO, Tuple
 import re
 import logging
 from .base_editor import (
     format_eng, ComponentNotFoundError, ParameterNotFoundError,
     PARAM_REGEX, UNIQUE_SIMULATION_DOT_INSTRUCTIONS
 )
-from .base_schematic import BaseSchematic, SchematicComponent, Point, ERotation, Line, Text, TextTypeEnum
+from .base_schematic import (BaseSchematic, SchematicComponent, Point, ERotation, Line, Text, TextTypeEnum,
+                             LineStyle, Shape)
 from ..utils.file_search import find_file_in_directory
 
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2021, Fribourg Switzerland"
 
-__all__ = ('QschEditor', )
+__all__ = ('QschEditor', 'QschTag', 'QschReadingError')
 
 _logger = logging.getLogger("qspice.QschEditor")
 
 QSCH_HEADER = (255, 216, 255, 219)
 
 
 # «component (-1200,-100) 0 0
@@ -83,14 +84,88 @@
 QSCH_TEXT_ROTATION = 3  # 13="0 Degrees" 45="90 Degrees" 77="180 Degrees" 109="270 Degrees" r= 13+32*alpha/90
 QSCH_TEXT_COMMENT = 4  # 0="Normal Text" 1="Comment"
 QSCH_TEXT_COLOR = 5  # 0xdbbggrr  d=1 "Default" rr=Red gg=Green bb=Blue in hex format
 QSCH_TEXT_STR_ATTR = 8
 
 QSCH_TEXT_INSTR_QUALIFIER = "ï»¿"
 
+# «line (2000,1300) (3150,-100) 1 1 0xff0000 -1 -1»
+QSCH_LINE_POS1 = 1
+QSCH_LINE_POS2 = 2
+QSCH_LINE_WIDTH = 3  # 0=Default 1=Thinnest ... 7=Thickest
+QSCH_LINE_TYPE = 4  # 0=Normal 1=Dashed 2=Dotted 3=DashDot 4=DashDotDot
+QSCH_LINE_COLOR = 5
+QSCH_LINE_UNKNOWN1 = 6
+QSCH_LINE_UNKNOWN2 = 7
+
+# «rect (1850,1550) (3650,-400) 0 0 0 0x8000 0x1000000 -1 0 -1»
+QSCH_RECT_POS1 = 1
+QSCH_RECT_POS2 = 2
+QSCH_RECT_UNKNOWN0 = 3
+QSCH_RECT_LINE_WIDTH = 4
+QSCH_RECT_LINE_TYPE = 5  # 0=Normal 1=Dashed 2=Dotted 3=DashDot 4=DashDotDot
+QSCH_RECT_LINE_COLOR = 6
+QSCH_RECT_FILL_COLOR = 7
+QSCH_RECT_UNKNOWN1 = 8
+QSCH_RECT_UNKNOWN2 = 9
+QSCH_RECT_UNKNOWN3 = 10
+
+#  «ellipse (2100,1150) (2650,150) 0 0 2 0xff0000 0x1000000 -1 -1»
+QSCH_ELLIPSE_POS1 = 1
+QSCH_ELLIPSE_POS2 = 2
+QSCH_ELLIPSE_UNKNOWN0 = 3
+QSCH_ELLIPSE_WIDTH = 4
+QSCH_ELLIPSE_LINE_TYPE = 5  # 0=Normal 1=Dashed 2=Dotted 3=DashDot 4=DashDotDot
+QSCH_ELLIPSE_LINE_COLOR = 6
+QSCH_ELLIPSE_FILL_COLOR = 7
+QSCH_ELLIPSE_UNKNOWN1 = 8
+QSCH_ELLIPSE_UNKNOWN2 = 9
+
+# «arc3p (2700,300) (2250,1200) (2500,800) 0 2 0xff0000 -1 -1»
+QSCH_ARC3P_POS1 = 1
+QSCH_ARC3P_POS2 = 2
+QSCH_ARC3P_POS3 = 3
+QSCH_ARC3P_UNKNOWN0 = 4
+QSCH_ARC3P_WIDTH = 5
+QSCH_ARC3P_LINE_COLOR = 6
+QSCH_ARC3P_UNKNOWN1 = 7
+QSCH_ARC3P_UNKNOWN2 = 8
+
+# «triangle (3050,1250) (3550,700) (3450,1400) 0 2 0xff0000 0x2000000 -1 -1»
+QSCH_TRIANGLE_POS1 = 1
+QSCH_TRIANGLE_POS2 = 2
+QSCH_TRIANGLE_POS3 = 3
+QSCH_TRIANGLE_UNKNOWN0 = 4
+QSCH_TRIANGLE_LINE_TYPE = 5  # 0=Normal 1=Dashed 2=Dotted 3=DashDot 4=DashDotDot
+QSCH_TRIANGLE_LINE_COLOR = 6
+QSCH_TRIANGLE_FILL_COLOR = 7
+QSCH_TRIANGLE_UNKNOWN1 = 8
+QSCH_TRIANGLE_UNKNOWN2 = 9
+
+# «coil (3050,400) (3450,600) 0 0 2 0xff0000 -1 -1»
+QSCH_COIL_POS1 = 1
+QSCH_COIL_POS2 = 2
+QSCH_COIL_UNKNOWN0 = 3
+QSCH_COIL_WIDTH = 4
+QSCH_COIL_LINE_TYPE = 5  # 0=Normal 1=Dashed 2=Dotted 3=DashDot 4=DashDotDot
+QSCH_COIL_LINE_COLOR = 6
+QSCH_COIL_UNKNOWN1 = 7
+QSCH_COIL_UNKNOWN2 = 8
+
+# «zigzag (3050,250) (3400,100) 0 0 2 0xff0000 -1 -1»
+QSCH_ZIGZAG_POS1 = 1
+QSCH_ZIGZAG_POS2 = 2
+QSCH_ZIGZAG_UNKNOWN0 = 3
+QSCH_ZIGZAG_WIDTH = 4
+QSCH_ZIGZAG_LINE_TYPE = 5  # 0=Normal 1=Dashed 2=Dotted 3=DashDot 4=DashDotDot
+QSCH_ZIGZAG_LINE_COLOR = 6
+QSCH_ZIGZAG_UNKNOWN1 = 7
+QSCH_ZIGZAG_UNKNOWN2 = 8
+
+
 
 class QschReadingError(IOError):
     ...
 
 
 class QschTag:
     """
@@ -101,15 +176,15 @@
         self.items = []
         self.tokens = []
         if tokens:
             for token in tokens:
                 self.tokens.append(str(token))
 
     @classmethod
-    def parse(cls, stream: str, start: int = 0) -> ('QschTag', int):
+    def parse(cls, stream: str, start: int = 0) -> Tuple['QschTag', int]:
         """
         Parses a tag from the stream starting at the given position. The stream should be a string.
 
         :param stream: The string to be parsed
         :param start: The position to start parsing
         :return: A tuple with the tag and the position after the tag
         """
@@ -159,15 +234,15 @@
 
         :param level: The indentation level
         :return: A string representation of the tag
         """
         spaces = '  ' * level
         if len(self.items):
             return (f"{spaces}«{' '.join(self.tokens)}\n"
-                    f"{''.join(tag.out(level+1) for tag in self.items)}"
+                    f"{''.join(tag.out(level + 1) for tag in self.items)}"
                     f"{spaces}»\n")
         else:
             return f"{'  ' * level}«{' '.join(self.tokens)}»\n"
 
     @property
     def tag(self) -> str:
         """Returns the tag id of the object. The tag id is the first token in the tag."""
@@ -225,15 +300,15 @@
             raise ValueError("Object not supported in set_attr")
         self.tokens[index] = value_str
 
     def get_text(self, label, default: str = None) -> str:
         """
         Returns the text of the first child tag that matches the given label.
         """
-        a = self.get_items(label+':')
+        a = self.get_items(label + ':')
         if len(a) != 1:
             if default is None:
                 raise IndexError(f"Label '{label}' not found in:{self}")
             else:
                 return default
         return a[0].tokens[1]
 
@@ -517,24 +592,34 @@
                 text = text.lstrip(QSCH_TEXT_INSTR_QUALIFIER)  # Eliminates the qualifer from the text.
             else:
                 type_text = TextTypeEnum.NULL
 
             # angle = text_tag.get_attr(QSCH_TEXT_ROTATION)  # TODO: Implement text Rotation
 
             text_obj = Text(
-                    point,
-                    text,
-                    text_size,
-                    type_text,
-                    # textAlignment,
-                    # verticalAlignment,
-                    # angle=angle,
-                )
+                point,
+                text,
+                text_size,
+                type_text,
+                # textAlignment,
+                # verticalAlignment,
+                # angle=angle,
+            )
             self.directives.append(text_obj)
 
+        for line_tag in self.schematic.get_items('line'):
+            x1, y1 = line_tag.get_attr(QSCH_LINE_POS1)
+            x2, y2 = line_tag.get_attr(QSCH_LINE_POS2)
+            width = line_tag.get_attr(QSCH_LINE_WIDTH)
+            line_type = line_tag.get_attr(QSCH_LINE_TYPE)
+            color = line_tag.get_attr(QSCH_LINE_COLOR)
+            line = Line(Point(x1, y1), Point(x2, y2))
+            line.style = LineStyle(width, line_type, color)
+            self.lines.append(line)
+
     def _get_text_matching(self, command, search_expression: re.Pattern):
         command_upped = command.upper()
         text_tags = self.schematic.get_items('text')
         for tag in text_tags:
             line = tag.get_attr(QSCH_TEXT_STR_ATTR)
             line = line.lstrip(QSCH_TEXT_INSTR_QUALIFIER)
             if line.upper().startswith(command_upped):
@@ -545,15 +630,15 @@
             return None, None
 
     def _qsch_file_find(self, filename) -> Optional[str]:
         for sym_root in self.lib_paths + [
             # os.path.curdir,  # The current script directory
             os.path.split(self._qsch_file_path)[0],  # The directory where the script is located
             os.path.expanduser(r"C:\Program Files\QSPICE"),
-            os.path.expanduser(r"~\Documents\QSPICE"),
+            os.path.expanduser("~/Documents/QSPICE"),
         ]:
             print(f"   {os.path.abspath(sym_root)}")
             if not os.path.exists(sym_root):  # Skipping invalid paths
                 continue
             file_found = find_file_in_directory(sym_root, filename)
             if file_found is not None:
                 return file_found
@@ -563,34 +648,34 @@
         subcircuit = self.get_component(reference)
         if '_SUBCKT' in subcircuit.attributes:  # Optimization: if it was already stored, return it
             return subcircuit.attributes['_SUBCKT']
         raise AttributeError(f"An associated subcircuit was not found for {reference}")
 
     def get_parameter(self, param: str) -> str:
         # docstring inherited from BaseEditor
-        param_regex = re.compile(PARAM_REGEX % param, re.IGNORECASE)
+        param_regex = re.compile(PARAM_REGEX(param), re.IGNORECASE)
         tag, match = self._get_text_matching(".PARAM", param_regex)
         if match:
             return match.group('value')
         else:
             raise ParameterNotFoundError(f"Parameter {param} not found in QSCH file")
 
     def set_parameter(self, param: str, value: Union[str, int, float]) -> None:
         # docstring inherited from BaseEditor
-        param_regex = re.compile(PARAM_REGEX % param, re.IGNORECASE)
+        param_regex = re.compile(PARAM_REGEX(param), re.IGNORECASE)
         tag, match = self._get_text_matching(".PARAM", param_regex)
         if match:
             _logger.debug(f"Parameter {param} found in QSCH file, updating it")
             if isinstance(value, (int, float)):
                 value_str = format_eng(value)
             else:
                 value_str = value
             text: str = tag.get_attr(QSCH_TEXT_STR_ATTR)
             match = param_regex.search(text)  # repeating the search, so we update the correct start/stop parameter
-            start, stop = match.span(param_regex.groupindex['replace'])
+            start, stop = match.span()
             text = text[:start] + "{}={}".format(param, value_str) + text[stop:]
             tag.set_attr(QSCH_TEXT_STR_ATTR, text)
             _logger.info(f"Parameter {param} updated to {value_str}")
             _logger.debug(f"Text at {tag.get_attr(QSCH_TEXT_POS)} Updated to {text}")
         else:
             # Was not found so we need to add it,
             _logger.debug(f"Parameter {param} not found in QSCH file, adding it")
@@ -599,49 +684,133 @@
                 f'«text ({x},{y}) 1 0 0 0x1000000 -1 -1 "{QSCH_TEXT_INSTR_QUALIFIER}.param {param}={value}"»'
             )
             self.schematic.items.append(tag)
             _logger.info(f"Parameter {param} added with value {value}")
             _logger.debug(f"Text added to {tag.get_attr(QSCH_TEXT_POS)} Added: {tag.get_attr(QSCH_TEXT_STR_ATTR)}")
         self.updated = True
 
-    def set_component_value(self, device: str, value: Union[str, int, float]) -> None:
+    def _get_component_symbol(self, reference: str) -> Tuple["BaseSchematic", str, QschTag]:
+        sub_circuit, ref = self._get_parent(reference)
+        if ref not in sub_circuit.components:
+            _logger.error(f"Component {ref} not found")
+            raise ComponentNotFoundError(f"Component {ref} not found in Schematic file")
+
+        component = sub_circuit.components[ref]
+        comp_tag: QschTag = component.attributes['tag']
+        symbol: QschTag = comp_tag.get_items('symbol')[0]
+        return sub_circuit, ref, symbol
+
+    def set_component_value(self, reference: str, value: Union[str, int, float]) -> None:
         # docstring inherited from BaseEditor
         if isinstance(value, str):
             value_str = value
         else:
             value_str = format_eng(value)
-        self.set_element_model(device, value_str)
+        self.set_element_model(reference, value_str)
 
     def set_element_model(self, device: str, model: str) -> None:
         # docstring inherited from BaseEditor
-        sub_circuit, ref = self._get_parent(device)
-        if ref not in sub_circuit.components:
-            _logger.error(f"Component {ref} not found")
-            raise ComponentNotFoundError(f"Component {ref} not found in Schematic file")
-
-        comp = sub_circuit.get_component(ref)
-        component: QschTag = comp.attributes['tag']
-        symbol: QschTag = component.get_items('symbol')[0]
+        sub_circuit, ref, symbol = self._get_component_symbol(device)
         texts = symbol.get_items('text')
         assert texts[QSCH_SYMBOL_TEXT_REFDES].get_attr(QSCH_TEXT_STR_ATTR) == ref
         texts[QSCH_SYMBOL_TEXT_VALUE].set_attr(QSCH_TEXT_STR_ATTR, model)
         sub_circuit.components[ref].attributes['value'] = model
         _logger.info(f"Component {device} updated to {model}")
-        _logger.debug(f"Component at :{component.get_attr(1)} Updated")
         sub_circuit.updated = True
 
     def get_component_value(self, element: str) -> str:
         # docstring inherited from BaseEditor
         component = self.get_component(element)
         if "value" not in component.attributes:
             _logger.error(f"Component {element} does not have a Value attribute")
             raise ComponentNotFoundError(f"Component {element} does not have a Value attribute")
         return component.attributes["value"]
 
-    def get_component_position(self, reference: str) -> (Point, ERotation):
+    def get_component_parameters(self, element: str) -> dict:
+        """
+        Returns the parameters of the component in a dictionary. Since QSpice stores attributes by their order of
+        appearance on the QSCH file, some parameters may not be found if they are not in the standard format.
+        If a line contains a parameter definition that is on the standard format, it will be parsed and stored in the
+        dictionary. The key of the dictionary is the line number where the parameter was found.
+
+        :param element: The reference of the component
+        :type element: str
+        :return: A dictionary with the parameters of the component
+        :rtype: dict
+        """
+        _, _, symbol = self._get_component_symbol(element)
+        texts = symbol.get_items('text')
+        parameters = {}
+        param_regex = re.compile(PARAM_REGEX(r'\w+'), re.IGNORECASE)
+        for i in range(2, len(texts)):
+            text = texts[i].get_attr(QSCH_TEXT_STR_ATTR)
+            matches = param_regex.finditer(text)
+            for match in matches:
+                parameters[match.group('name')] = match.group('value')
+            else:
+                parameters[i] = text
+
+        return parameters
+
+    def set_component_parameters(self, element: str, **kwargs) -> None:
+        """
+        Sets the parameters of the component. If key parameters that are integers, they represent the line number
+        where the parameter was found. If the key is a string, it represents the parameter name. If the parameter name
+        already exists, it will be replaced. If not found, it will be added as a new text line.
+        """
+        sub_circuit, ref, symbol = self._get_component_symbol(element)
+        texts = symbol.get_items('text')
+
+        for key, value in kwargs.items():
+            if isinstance(key, int):
+                if key < 2 or key > len(texts):
+                    raise ValueError(f"Invalid line number {key} for component {element}")
+                if key == len(texts):
+                    x, y = 0, 0  # TODO: Find a way to get the position of the last text
+                    tag, _ = QschTag.parse(
+                        f'«text ({x},{y}) 1 7 0 0x1000000 -1 -1 "{value}"»'
+                    )
+                    symbol.items.append(tag)
+
+                else:
+                    texts[key].set_attr(QSCH_TEXT_STR_ATTR, value)
+                sub_circuit.updated = True
+            else:
+                found = False
+                search_expression = re.compile(PARAM_REGEX(key), re.IGNORECASE)
+                for text in texts[QSCH_SYMBOL_TEXT_VALUE:]:
+                    text_value = text.get_attr(QSCH_TEXT_STR_ATTR)
+                    match = search_expression.search(text_value)
+                    if match:
+                        start, stop = match.span()
+                        text_value = text_value[:start] + f"{key}={value}" + text_value[stop:]
+                        text.set_attr(QSCH_TEXT_STR_ATTR, text_value)
+                        sub_circuit.updated = True
+                        found = True
+                        break
+                if not found:
+                    x, y = 0, 0  # TODO: Find a way to get the position of the last text
+                    new_tag, _ = QschTag.parse(
+                        f'«text ({x},{y}) 0.5 0 0 0x1000000 -1 -1 "{key}={value}"»'
+                    )
+                    # Inserting the new tag just after the last text and the first pin
+                    last_text = 0
+                    for i, tag in enumerate(symbol.items):
+                        if tag.tag == 'pin':
+                            last_text = i
+                            break
+                        elif tag.tag == 'text':
+                            last_text = i + 1  # The new text should be inserted after the last text
+                    if 0 <= last_text < len(symbol.items):
+                        symbol.items.insert(last_text, new_tag)
+                    else:
+                        symbol.items.append(new_tag)
+                    sub_circuit.updated = True
+
+    def get_component_position(self, reference: str) -> Tuple[Point, ERotation]:
         # docstring inherited from BaseSchematic
         component = self.get_component(reference)
         return component.position, component.rotation
 
     def set_component_position(self, reference: str,
                                position: Union[Point, tuple],
                                rotation: Union[ERotation, int],
@@ -659,15 +828,15 @@
         if isinstance(rotation, ERotation):
             rot = rotation.value / 45
         elif isinstance(rotation, int):
             rot = (rotation % 360) // 45
             if mirror:
                 rot += 8
         else:
-             raise ValueError("Invalid rotation parameter")
+            raise ValueError("Invalid rotation parameter")
 
         comp_tag.set_attr(QSCH_COMPONENT_POS, position)
         comp_tag.set_attr(QSCH_COMPONENT_ROTATION, rot)
         component.position = position
         component.rotation = rotation
 
     def get_components(self, prefixes='*') -> list:
@@ -790,12 +959,73 @@
             for wire in self.wires:
                 wire_tag, _ = QschTag.parse('«wire (0,0) (0,0) "0"»')
                 wire_tag.set_attr(QSCH_WIRE_POS1, (wire.V1.X, wire.V1.Y))
                 wire_tag.set_attr(QSCH_WIRE_POS2, (wire.V2.X, wire.V2.Y))
                 # wire_tag.set_attr(QSCH_WIRE_NET, wire.net)
                 self.schematic.items.append(wire_tag)
 
+            for line in self.lines:
+                line_tag, _ = QschTag.parse('«line (2000,1300) (3150,-100) 0 2 0xff0000 -1 -1»')
+                line_tag.set_attr(QSCH_LINE_POS1, (line.V1.X, line.V1.Y))
+                line_tag.set_attr(QSCH_LINE_POS2, (line.V2.X, line.V2.Y))
+                # TODO: Implement the style to width, type and color
+                # line_width = 0  # Default
+                # line_type = 0  # Default
+                # color = 0xff0000  # Default : Blue Color
+                # line_width, line_type, color = line.style.split(' ')
+                # line_tag.set_attr(QSCH_LINE_WIDTH, line_width)
+                # line_tag.set_attr(QSCH_LINE_TYPE, line_type)
+                # line_tag.set_attr(QSCH_LINE_COLOR, color)
+                self.schematic.items.append(line_tag)
+
+            for shape in self.shapes:
+                # TODO: Implement the line type and width conversion from LTSpice to QSpice.
+                if shape.name == "RECTANGLE" or shape.name == "rect":
+                    shape_tag, _ = QschTag.parse('«rect (1850,1550) (3650,-400) 0 0 2 0xff0000 0x1000000 -1 0 -1»')
+                    shape_tag.set_attr(QSCH_RECT_POS1, (shape.points[0].X, shape.points[0].Y))
+                    shape_tag.set_attr(QSCH_RECT_POS2, (shape.points[1].X, shape.points[1].Y))
+                    # shape_tag.set_attr(QSCH_RECT_LINE_TYPE, shape.line_style.pattern)
+                    # shape_tag.set_attr(QSCH_RECT_LINE_WIDTH, shape.line_style.width)
+                    # shape_tag.set_attr(QSCH_RECT_LINE_COLOR, shape.line_style.color)
+                elif shape.name == "CIRCLE" or shape.name == "ellipse":
+                    shape_tag, _ = QschTag.parse('«ellipse (2100,1150) (2650,150) 0 0 2 0xff0000 0x1000000 -1 -1»')
+                    shape_tag.set_attr(QSCH_ELLIPSE_POS1, (shape.points[0].X, shape.points[0].Y))
+                    shape_tag.set_attr(QSCH_ELLIPSE_POS2, (shape.points[1].X, shape.points[1].Y))
+                    # shape_tag.set_attr(QSCH_ELLIPSE_LINE_COLOR, shape.line_style.color)
+                    # shape_tag.set_attr(QSCH_ELLIPSE_FILL_COLOR, shape.fill)
+                elif shape.name == "ARC" or shape.name == "arc3p":
+                    shape_tag, _ = QschTag.parse('«arc3p (2700,300) (2250,1200) (2500,800) 0 2 0xff0000 -1 -1»')
+                    # TODO: Implement the ARC shape correctly.
+                    # In LTSpice the First two points defines the bounding box of the arc and the following
+                    # two points define the start and end of the arc.
+                    # QSpice uses the first two points to define the start and end of the arc and the third point
+                    # to define the curvature of the arc.
+                    if shape.name == "ARC":
+                        assert len(shape.points) == 4, "Invalid LTSpice shape"
+                        center_x = int((shape.points[0].X + shape.points[1].X) / 2)
+                        center_y = int((shape.points[0].Y + shape.points[1].Y) / 2)
+                        start_angle = math.atan2(shape.points[2].Y - center_y, shape.points[2].X - center_x)
+                        end_angle = math.atan2(shape.points[3].Y - center_y, shape.points[3].X - center_x)
+                        ellipse_width = abs(shape.points[1].X - shape.points[0].X)
+                        ellipse_height = abs(shape.points[1].Y - shape.points[0].Y)
+                        start_point_x = int(center_x + ellipse_width / 2 * math.cos(start_angle))
+                        start_point_y = int(center_y + ellipse_height / 2 * math.sin(start_angle))
+                        end_point_x = int(center_x + ellipse_width / 2 * math.cos(end_angle))
+                        end_point_y = int(center_y + ellipse_height / 2 * math.sin(end_angle))
+                        shape_tag.set_attr(QSCH_ARC3P_POS1, (start_point_x, start_point_y))
+                        shape_tag.set_attr(QSCH_ARC3P_POS2, (end_point_x, end_point_y))
+                        shape_tag.set_attr(QSCH_ARC3P_POS3, (center_x, center_y))
+                    else:
+                        shape_tag.set_attr(QSCH_ARC3P_POS1, (shape.points[0].X, shape.points[0].Y))
+                        shape_tag.set_attr(QSCH_ARC3P_POS2, (shape.points[1].X, shape.points[1].Y))
+                        shape_tag.set_attr(QSCH_ARC3P_POS3, (shape.points[2].X, shape.points[2].Y))
+                        # shape_tag.set_attr(QSCH_ARC3P_LINE_COLOR, shape.line_style.color)
+                else:
+                    print(f"Invalid shape {shape.name}. Being ignored. Ask Developper to implement this")
+
+                self.schematic.items.append(shape_tag)
+
             for text in self.directives:
                 text_tag, _ = QschTag.parse('«text (0,0) 1 7 0 0x1000000 -1 -1 "text"»')
                 text_tag.set_attr(QSCH_TEXT_STR_ATTR, QSCH_TEXT_INSTR_QUALIFIER + text.text)
                 text_tag.set_attr(QSCH_TEXT_POS, (text.coord.X, text.coord.Y))
                 self.schematic.items.append(text_tag)
```

### Comparing `spicelib-1.1.2/spicelib/editor/spice_editor.py` & `spicelib-1.1.3/spicelib/editor/spice_editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,71 +13,92 @@
 # Purpose:     Class made to update Generic Spice netlists
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import os
+from collections import OrderedDict
 from pathlib import Path
 import re
 import logging
 
 from .base_editor import BaseEditor, format_eng, ComponentNotFoundError, ParameterNotFoundError, PARAM_REGEX, \
     UNIQUE_SIMULATION_DOT_INSTRUCTIONS, Component, SUBCKT_DIVIDER
 
 from typing import Union, List, Callable, Any, Tuple, Optional
 from ..utils.detect_encoding import detect_encoding, EncodingDetectError
+from ..log.logfile_data import try_convert_value
 
 _logger = logging.getLogger("spicelib.SpiceEditor")
 
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2021, Fribourg Switzerland"
 
 END_LINE_TERM = '\n'  #: This controls the end of line terminator used
 
 # A Spice netlist can only have one of the instructions below, otherwise an error will be raised
 
-REPLACE_REGXES = {
-    'A': r"",  # LTSPice Only : Special Functions, Parameter substitution not supported
+# Regular expressions for the different components
+FLOAT_RGX = r"[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?"
+
+# Regular expression for a number with decimal qualifier and unit
+NUMBER_RGX = r"[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?(Meg|[kmuµnpfgt])?[a-zA-Z]*"
+
+# Parameters expression of the type: PARAM=value
+PARAM_RGX = r"(?P<params>(\s+\w+\s*(=\s*[\w\{\}\(\)\-\+\*\/%\.]+)?)*)?"
+
+
+def VALUE_RGX(number_regex):
+    return r"(?P<value>(?P<formula>{)?(?(formula).*}|" + number_regex + "))"
+
+
+REPLACE_REGEXS = {
+    'A': r"",  # LTspice Only : Special Functions, Parameter substitution not supported
     'B': r"^(?P<designator>B§?[VI]?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Behavioral source
-    'C': r"^(?P<designator>C§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+(?P<value>({)?(?(6).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?F?))).*$",
-    # Capacitor
-    'D': r"^(?P<designator>D§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>\w+).*$",  # Diode
+    'C': r"^(?P<designator>C§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+" +
+         VALUE_RGX(FLOAT_RGX + "[muµnpfgt]?F?") +
+         PARAM_RGX + ".*$",  # Capacitor
+    'D': r"^(?P<designator>D§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>\w+)" +
+         PARAM_RGX + ".*$",  # Diode
     'E': r"^(?P<designator>E§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>.*)$",  # Voltage Dependent Voltage Source
     # this only supports changing gain values
     'F': r"^(?P<designator>F§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Dependent Current Source
     # This implementation replaces everything after the 2 first nets
     'G': r"^(?P<designator>G§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>.*)$",  # Voltage Dependent Current Source
     # This only supports changing gain values
     'H': r"^(?P<designator>H§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Voltage Dependent Current Source
     # This implementation replaces everything after the 2 first nets
     'I': r"^(?P<designator>I§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Source
     # This implementation replaces everything after the 2 first nets
-    'J': r"^(?P<designator>J§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>\w+).*$",  # JFET
-    'K': r"^(?P<designator>K§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>[\+\-]?[0-9\.E+-]+[kmuµnpf]?).*$",
+    'J': r"^(?P<designator>J§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>\w+)" + 
+         PARAM_RGX + ".*$",  # JFET
+    'K': r"^(?P<designator>K§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>[\+\-]?[0-9\.E+-]+[kmuµgt]?).*$",
     # Mutual Inductance
-    'L': r"^(?P<designator>L§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>({)?(?(5).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?H?))).*$",
+    'L': r"^(?P<designator>L§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>({)?(?(5).*}|([0-9\.E+-]+(Meg|[kmuµgt])?H?))).*$",
     # Inductance
     'M': r"^(?P<designator>M§?\w+)(?P<nodes>(\s+\S+){3,4})\s+(?P<value>\w+).*$",
     # MOSFET TODO: Parameters substitution not supported
     'O': r"^(?P<designator>O§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>\w+).*$",
     # Lossy Transmission Line TODO: Parameters substitution not supported
-    'Q': r"^(?P<designator>Q§?\w+)(?P<nodes>(\s+\S+){3,4})\s+(?P<value>\w+).*$",
+    'Q': r"^(?P<designator>Q§?\w+)(?P<nodes>(\s+\S+){3,4})\s+(?P<value>\w+)" + PARAM_RGX + ".*$",
     # Bipolar TODO: Parameters substitution not supported
-    'R': r"^(?P<designator>R§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+(?P<value>(R=)?({)?(?(7).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?R?)\d*)).*$",
-    # Resistors
+    'R': r"^(?P<designator>R§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+" +
+         "(R=)?" + VALUE_RGX(FLOAT_RGX + r"(Meg|[kRmuµnpfgt])?\d*") +
+         PARAM_RGX + ".*$",  # Resistor
     'S': r"^(?P<designator>S§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>.*)$",  # Voltage Controlled Switch
     'T': r"^(?P<designator>T§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>.*)$",  # Lossless Transmission
     'U': r"^(?P<designator>U§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>.*)$",  # Uniform RC-line
     'V': r"^(?P<designator>V§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Voltage Source
     # This implementation replaces everything after the 2 first nets
     'W': r"^(?P<designator>W§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Controlled Switch
     # This implementation replaces everything after the 2 first nets
-    'X': r"^(?P<designator>X§?\w+)(?P<nodes>(\s+\S+){1,99}?)\s+(?P<value>\w+)(\s+params:)?(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",
-    # Sub-circuit, Parameter substitution not supported
+    'X': r"^(?P<designator>X§?\w+)(?P<nodes>(\s+\S+){1,99}?)\s+(?P<value>\w+)"
+         r"(\s+params:)?(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",
+    # Sub-circuit
     'Z': r"^(?P<designator>Z§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>\w+).*$",
     # MESFET and IBGT. TODO: Parameters substitution not supported
     '@': r"^(?P<designator>@§?\d+)(?P<nodes>(\s+\S+){2})\s?(?P<params>(.*)*)$",
     # Frequency Noise Analysis (FRA) wiggler
     # pattern = r'^@(\d+)\s+(\w+)\s+(\w+)(?:\s+delay=(\d+\w+))?(?:\s+fstart=(\d+\w+))?(?:\s+fend=(\d+\w+))?(?:\s+oct=(\d+))?(?:\s+fcoarse=(\d+\w+))?(?:\s+nmax=(\d+\w+))?\s+(\d+)\s+(\d+\w+)\s+(\d+)(?:\s+pp0=(\d+\.\d+))?(?:\s+pp1=(\d+\.\d+))?(?:\s+f0=(\d+\w+))?(?:\s+f1=(\d+\w+))?(?:\s+tavgmin=(\d+\w+))?(?:\s+tsettle=(\d+\w+))?(?:\s+acmag=(\d+))?$'
     'Ã': r"^(?P<designator>Ã\w+)(?P<nodes>(\s+\S+){16})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component Ã
     '¥': r"^(?P<designator>¥\w+)(?P<nodes>(\s+\S+){16})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component ¥
@@ -86,16 +107,22 @@
     'Ø': r"^(?P<designator>Ø\w+)(?P<nodes>(\s+\S+){1,99})\s+(?P<value>.*)(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # QSPICE Unique component Ø
     '×': r"^(?P<designator>×\w+)(?P<nodes>(\s+\S+){4,16})\s+(?P<value>.*)(?P<params>(\w+\s+){1,8})\s*\\?$",  # QSPICE proprietaty component ×
     'Ö': r"^(?P<designator>Ö\w+)(?P<nodes>(\s+\S+){5})\s+(?P<params>.*)\s*\\?$",  # LTspice proprietary component Ö
 }
 
 SUBCKT_CLAUSE_FIND = r"^.SUBCKT\s+"
 
+ # Debug code to test the regular expressions
+# for key, pattern in REPLACE_REGEXS.items():
+#     print(f"Testing {key}")
+#     print(f"Pattern: {pattern}")
+#     re.compile(pattern, re.IGNORECASE + re.MULTILINE)
+
 # Code Optimization objects, avoiding repeated compilation of regular expressions
-component_replace_regexs = {prefix: re.compile(pattern, re.IGNORECASE) for prefix, pattern in REPLACE_REGXES.items()}
+component_replace_regexs = {prefix: re.compile(pattern, re.IGNORECASE) for prefix, pattern in REPLACE_REGEXS.items()}
 subckt_regex = re.compile(r"^.SUBCKT\s+(?P<name>\w+)", re.IGNORECASE)
 lib_inc_regex = re.compile(r"^\.(LIB|INC)\s+(.*)$", re.IGNORECASE)
 
 LibSearchPaths = []
 
 
 def get_line_command(line) -> str:
@@ -106,15 +133,15 @@
     if isinstance(line, str):
         for i in range(len(line)):
             ch = line[i]
             if ch == ' ' or ch == '\t':
                 continue
             else:
                 ch = ch.upper()
-                if ch in REPLACE_REGXES:  # A circuit element
+                if ch in REPLACE_REGEXS:  # A circuit element
                     return ch
                 elif ch == '+':
                     return '+'  # This is a line continuation.
                 elif ch in "#;*\n\r":  # It is a comment or a blank line
                     return "*"
                 elif ch == '.':  # this is a directive
                     j = i + 1
@@ -259,27 +286,33 @@
         line_no = self._get_line_starting_with(subckt_ref)
         sub_circuit_instance = self.netlist[line_no]
         regex = component_replace_regexs['X']  # The sub-circuit instance regex
         m = regex.search(sub_circuit_instance)
         if m:
             subcircuit_name = m.group('value')  # last_token of the line before Params:
         else:
-            raise UnrecognizedSyntaxError(sub_circuit_instance, REPLACE_REGXES['X'])
+            raise UnrecognizedSyntaxError(sub_circuit_instance, REPLACE_REGEXS['X'])
 
         # Search for the sub-circuit in the netlist
-        sub_circuit = SpiceEditor.find_subckt_in_lib(self.circuit_file, subcircuit_name)
+        sub_circuit = None
+        for line in self.netlist:
+            if isinstance(line, SpiceCircuit):
+                if line.name() == subcircuit_name:
+                    return line
 
         if sub_circuit is None:  # If it was not found in the netlist, search on the declared libraries
             # If we reached here is because the subcircuit was not found. Search for it in declared libraries
             for line in self.netlist:
+                if isinstance(line, SpiceCircuit):  # If it is a sub-circuit it will simply ignore it.
+                    continue
                 m = lib_inc_regex.match(line)
                 if m:  # If it is a library include
                     lib = m.group(2)
                     if os.path.exists(lib):
-                        lib_filename = os.path.join(os.path.expanduser('~'), "Documents\\LTspiceXVII\\lib\\sub", lib)
+                        lib_filename = os.path.join(os.path.expanduser('~'), "Documents/LTspiceXVII/lib/sub", lib)
                         if os.path.exists(lib_filename):
                             sub_circuit = SpiceEditor.find_subckt_in_lib(lib_filename, subcircuit_name)
                             if sub_circuit:
                                 break
                     for path in LibSearchPaths:
                         lib_filename = os.path.join(path, lib)
                         if os.path.exists(lib_filename):
@@ -292,38 +325,39 @@
                 return sub_circuit.get_subcircuit(sub_subckts)
             else:
                 return sub_circuit
         else:
             # The search was not successful
             raise ComponentNotFoundError(f'Sub-circuit "{subcircuit_name}" not found')
 
-    def _set_model_and_value(self, component, value):
+    def _get_component_line_and_regex(self, reference: str) -> Tuple[int, re.Match]:
         """Internal function. Do not use."""
-        prefix = component[0]  # Using the first letter of the component to identify what is it
-        regex = component_replace_regexs.get(prefix, None)  # Obtain RegX to make the update
-
+        prefix = reference[0]
+        regex = component_replace_regexs.get(prefix, None)
         if regex is None:
-            error_msg = f"Component must start with one of these letters: {','.join(REPLACE_REGXES.keys())}\n" \
-                        f"Got {component}"
+            error_msg = f"Component must start with one of these letters: {','.join(REPLACE_REGEXS.keys())}\n" \
+                        f"Got {reference}"
             _logger.error(error_msg)
-            return
+            raise NotImplementedError(error_msg)
+        line_no = self._get_line_starting_with(reference)
+        line = self.netlist[line_no]
+        match = regex.match(line)
+        if match is None:
+            raise UnrecognizedSyntaxError(line, regex.pattern)
+        return line_no, match
 
+    def _set_model_and_value(self, reference, value):
+        """Internal function. Do not use."""
+        line_no, match = self._get_component_line_and_regex(reference)
         if isinstance(value, (int, float)):
             value = format_eng(value)
-
-        line_no = self._get_line_starting_with(component)
-
+        start = match.start('value')
+        end = match.end('value')
         line = self.netlist[line_no]
-        m = regex.match(line)
-        if m is None:
-            raise UnrecognizedSyntaxError(line, REPLACE_REGXES[prefix])
-        else:
-            start = m.start('value')
-            end = m.end('value')
-            self.netlist[line_no] = line[:start] + value + line[end:]
+        self.netlist[line_no] = line[:start] + value + line[end:]
 
     def reset_netlist(self, create_blank: bool = False) -> None:
         """
         Reverts all changes done to the netlist. If create_blank is set to True, then the netlist is blanked.
 
         :param create_blank: If True, the netlist is blanked. That is, all primitives and components are erased.
         :type create_blank: bool
@@ -417,43 +451,27 @@
         :raises: ComponentNotFoundError - In case the component is not found
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX.
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
         if SUBCKT_DIVIDER in reference:
             raise NotImplementedError("This method doesn't support hierarchical access. "
                                       "Please use set_component_value() and get_component_value() methods.")
-        prefix = reference[0]  # Using the first letter of the component to identify what is it
-        regex = component_replace_regexs.get(prefix, None)  # Obtain RegX to make the update
-
-        if regex is None:
-            error_msg = f"Component must start with one of these letters: {','.join(REPLACE_REGXES.keys())}\n" \
-                        f"Got {reference}"
-            _logger.warning(error_msg)
-            raise NotImplementedError("Unsuported prefix {}".format(prefix))
-
-        line_no = self._get_line_starting_with(reference)
-        line = self.netlist[line_no]
-        m = regex.match(line)
-        if m is None:
-            error_msg = 'Unsupported line "{}"\nExpected format is "{}"'.format(line, REPLACE_REGXES[prefix])
-            _logger.error(error_msg)
-            raise UnrecognizedSyntaxError(line, REPLACE_REGXES[prefix])
-
-        info = m.groupdict()
+        line_no, match = self._get_component_line_and_regex(reference)
+        info = match.groupdict()
         info['line'] = line_no  # adding the line number to the component information
         return info
 
     def get_component(self, reference: str) -> Union[Component, 'SpiceCircuit']:
         """
         Returns an object representing the given reference in the schematic file.
 
         :param reference: Reference of the component
         :type reference: str
         :return: The Component object or a SpiceSubcircuit in case of hierarchical design
-        :rtype: Component or SpiceSubcircuit
+        :rtype: Component or SpiceCircuit
         :raises: ComponentNotFoundError - In case the component is not found
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX.
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
         component_info = self.get_component_info(reference)
         component = Component()
         component.reference = reference
@@ -476,25 +494,69 @@
         :raises: ComponentNotFoundError - In case the component is not found
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX.
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
         component_info = self.get_component_info(reference)
         return component_info.get(attribute, None)
 
+    @staticmethod
+    def _parse_params(params_str: str) -> dict:
+        """
+        Parses the parameters string and returns a dictionary with the parameters.
+        """
+        params = OrderedDict()
+        for param in params_str.split():
+            key, value = param.split('=')
+            params[key] = try_convert_value(value)
+        return params
+
+    def get_component_parameters(self, reference: str) -> dict:
+        # docstring inherited from BaseEditor
+        line_no, match = self._get_component_line_and_regex(reference)
+        params_str = match.group('params')
+        return self._parse_params(params_str)
+
+    def set_component_parameters(self, reference: str, **kwargs) -> None:
+        # docstring inherited from BaseEditor
+        line_no, match = self._get_component_line_and_regex(reference)
+        params_str = match.group('params')
+        params = self._parse_params(params_str)
+
+        for key, value in kwargs.items():
+            # format the value
+            if value is None:
+                value_str = None
+            elif isinstance(value, str):
+                value_str = value.strip()
+            else:
+                value_str = format_eng(value)
+            if value_str is None:
+                # remove those that must disappear
+                if key in params:
+                    params.pop(key)
+            else:
+                # create or update
+                params[key] = value_str 
+        params_str = ' '.join([f'{key}={value}' for key, value in params.items()])
+        start = match.start('params')
+        end = match.end('params')
+        line = self.netlist[line_no]
+        self.netlist[line_no] = line[:start] + ' ' + params_str + line[end:]
+
     def get_parameter(self, param: str) -> str:
         """
         Returns the value of a parameter retrieved from the netlist.
 
         :param param: Name of the parameter to be retrieved
         :type param: str
         :return: Value of the parameter being sought
         :rtype: str
         :raises: ParameterNotFoundError - In case the component is not found
         """
-        regx = re.compile(PARAM_REGEX % param, re.IGNORECASE)
+        regx = re.compile(PARAM_REGEX(param), re.IGNORECASE)
         line_no, match = self._get_line_matching('.PARAM', regx)
         if match:
             return match.group('value')
         else:
             raise ParameterNotFoundError(param)
 
     def set_parameter(self, param: str, value: Union[str, int, float]) -> None:
@@ -515,102 +577,102 @@
         :type param: str
 
         :param value: Parameter Value to be set.
         :type value: str, int or float
 
         :return: Nothing
         """
-        regx = re.compile(PARAM_REGEX % param, re.IGNORECASE)
+        regx = re.compile(PARAM_REGEX(param), re.IGNORECASE)
         param_line, match = self._get_line_matching('.PARAM', regx)
         if match:
-            start, stop = match.span(regx.groupindex['replace'])
+            start, stop = match.span('value')
             line: str = self.netlist[param_line]
-            self.netlist[param_line] = line[:start] + "{}={}".format(param, value) + line[stop:]
+            self.netlist[param_line] = line[:start] + f"{value:g}" + line[stop:]
         else:
             # Was not found
             # the last two lines are typically (.backano and .end)
             insert_line = len(self.netlist) - 2
             self.netlist.insert(insert_line, '.PARAM {}={}  ; Batch instruction'.format(param, value) + END_LINE_TERM)
 
-    def set_component_value(self, device: str, value: Union[str, int, float]) -> None:
+    def set_component_value(self, reference: str, value: Union[str, int, float]) -> None:
         """
         Changes the value of a component, such as a Resistor, Capacitor or Inductor.
         For components inside sub-circuits, use the sub-circuit designator prefix with ':' as separator (Example X1:R1)
         Usage: ::
 
             LTC.set_component_value('R1', '3.3k')
             LTC.set_component_value('X1:C1', '10u')
 
-        :param device: Reference of the circuit element to be updated.
-        :type device: str
+        :param reference: Reference of the circuit element to be updated.
+        :type reference: str
         :param value:
             value to be set on the given circuit element. Float and integer values will be automatically
             formatted as per the engineering notations 'k' for kilo, 'm', for mili and so on.
         :type value: str, int or float
         :raises:
             ComponentNotFoundError - In case the component is not found
 
             ValueError - In case the value doesn't correspond to the expected format
 
             NotImplementedError - In case the circuit element is defined in a format which is not supported by this
             version.
 
             If this is the case, use GitHub to start a ticket.  https://github.com/nunobrum/spicelib
         """
-        self._set_model_and_value(device, value)
+        self._set_model_and_value(reference, value)
 
-    def set_element_model(self, element: str, model: str) -> None:
+    def set_element_model(self, reference: str, model: str) -> None:
         """Changes the value of a circuit element, such as a diode model or a voltage supply.
         Usage: ::
 
             LTC.set_element_model('D1', '1N4148')
             LTC.set_element_model('V1' "SINE(0 1 3k 0 0 0)")
 
-        :param element: Reference of the circuit element to be updated.
-        :type element: str
+        :param reference: Reference of the circuit element to be updated.
+        :type reference: str
         :param model: model name of the device to be updated
         :type model: str
 
         :raises:
             ComponentNotFoundError - In case the component is not found
 
             ValueError - In case the model format contains irregular characters
 
             NotImplementedError - In case the circuit element is defined in a format which is not supported by this version.
 
             If this is the case, use GitHub to start a ticket.  https://github.com/nunobrum/spicelib
         """
-        self._set_model_and_value(element, model)
+        self._set_model_and_value(reference, model)
 
-    def get_component_value(self, element: str) -> str:
+    def get_component_value(self, reference: str) -> str:
         """
         Returns the value of a component retrieved from the netlist.
 
-        :param element: Reference of the circuit element to get the value.
-        :type element: str
+        :param reference: Reference of the circuit element to get the value.
+        :type reference: str
 
         :return: value of the circuit element .
         :rtype: str
 
         :raises: ComponentNotFoundError - In case the component is not found
 
                  NotImplementedError - for not supported operations
         """
-        return self.get_component_info(element)['value']
+        return self.get_component_info(reference)['value']
 
-    def get_component_nodes(self, element: str) -> List[str]:
+    def get_component_nodes(self, reference: str) -> List[str]:
         """
         Returns the nodes to which the component is attached to.
 
-        :param element: Reference of the circuit element to get the nodes.
-        :type element: str
+        :param reference: Reference of the circuit element to get the nodes.
+        :type reference: str
         :return: List of nodes
         :rtype: list
         """
-        nodes = self.get_component_info(element)['nodes']
+        nodes = self.get_component_info(reference)['nodes']
         nodes = nodes.split()  # Remove any spaces if they exist. This considers \r \n \t characters as well
         return nodes
 
     def get_components(self, prefixes='*') -> list:
         """
         Returns a list of components that match the list of prefixes indicated on the parameter prefixes.
         In case prefixes is left empty, it returns all the ones that are defined by the REPLACE_REGEXES.
@@ -623,15 +685,15 @@
         :type prefixes: str
 
         :return:
             A list of components matching the prefixes demanded.
         """
         answer = []
         if prefixes == '*':
-            prefixes = ''.join(REPLACE_REGXES.keys())
+            prefixes = ''.join(REPLACE_REGEXS.keys())
         for line in self.netlist:
             if isinstance(line, SpiceCircuit):  # Only gets components from the main netlist,
                 # it currently skips sub-circuits
                 continue
             tokens = line.split()
             try:
                 if tokens[0][0] in prefixes:
@@ -795,45 +857,45 @@
                 subcircuit = self.modified_subcircuits[modified_path]
             else:
                 subcircuit = self.get_subcircuit(component)
             return subcircuit.get_component_info(component)
 
         return super().get_component_info(component)
 
-    def _set_model_and_value(self, component, value):
+    def _set_model_and_value(self, reference, value):
         """
         Internal method to set the model and value of a component.
         """
-        prefix = component[0]  # Using the first letter of the component to identify what is it
-        if prefix == 'X' and SUBCKT_DIVIDER in component:  # Relaces a component inside of a subciruit
+        prefix = reference[0]  # Using the first letter of the component to identify what is it
+        if prefix == 'X' and SUBCKT_DIVIDER in reference:  # Relaces a component inside of a subciruit
             # In this case the sub-circuit needs to be copied so that is copy is modified. A copy is created for each
             # instance of a sub-circuit.
-            component_split = component.split(SUBCKT_DIVIDER)
+            component_split = reference.split(SUBCKT_DIVIDER)
             modified_path = SUBCKT_DIVIDER.join(component_split[:-1])  # excludes last component
-            component = component_split[-1]  # This is the last component to modify
+            reference = component_split[-1]  # This is the last component to modify
 
             if modified_path in self.modified_subcircuits:  # See if this was already a modified sub-circuit instance
                 sub_circuit = self.modified_subcircuits[modified_path]
             else:
                 sub_circuit_original = self.get_subcircuit(modified_path)  # If not will look for it.
                 if sub_circuit_original:
                     new_name = sub_circuit_original.name() + '_' + '_'.join(
                         component_split[:-1])  # Creates a new name with the path appended
                     sub_circuit = sub_circuit_original.clone(new_name=new_name)
                     # Memorize that the copy is relative to that particular instance
                     self.modified_subcircuits[modified_path] = sub_circuit
                     # Change the call to the sub-circuit
                     self._set_model_and_value(modified_path, new_name)
                 else:
-                    raise ComponentNotFoundError(component)
+                    raise ComponentNotFoundError(reference)
             #  Change the copy of the sub-circuit related to that particular instance.
-            sub_circuit._set_model_and_value(component, value)
+            sub_circuit._set_model_and_value(reference, value)
             return
         # else: This is the generic case where the sub-circuit is changed
-        super()._set_model_and_value(component, value)
+        super()._set_model_and_value(reference, value)
 
     def add_instruction(self, instruction: str) -> None:
         """Adds a SPICE instruction to the netlist.
 
         For example:
 
         .. code-block:: text
```

### Comparing `spicelib-1.1.2/spicelib/log/logfile_data.py` & `spicelib-1.1.3/spicelib/log/logfile_data.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/log/ltsteps.py` & `spicelib-1.1.3/spicelib/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/log/qspice_log_reader.py` & `spicelib-1.1.3/spicelib/log/qspice_log_reader.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/log/semi_dev_op_reader.py` & `spicelib-1.1.3/spicelib/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/raw/raw_classes.py` & `spicelib-1.1.3/spicelib/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/raw/raw_convert.py` & `spicelib-1.1.3/spicelib/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/raw/raw_read.py` & `spicelib-1.1.3/spicelib/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/raw/raw_write.py` & `spicelib-1.1.3/spicelib/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/scripts/asc_to_qsch.py` & `spicelib-1.1.3/spicelib/scripts/asc_to_qsch.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,18 +50,22 @@
     asc_file = args[0]
     if len(args) > 1:
         qsch_file = args[1]
     else:
         qsch_file = os.path.splitext(asc_file)[0] + ".qsch"
 
     search_paths = [] if options.path is None else options.path
-    symbol_stock = {}
 
     print(f"Using {qsch_file} as output file")
+    convert_asc_to_qsch(asc_file, qsch_file, search_paths)
+
 
+def convert_asc_to_qsch(asc_file, qsch_file, search_paths=[]):
+    """Converts an ASC file to a QSCH schematic"""
+    symbol_stock = {}
     # Open the ASC file
     asc_editor = AscEditor(asc_file)
 
     # import the conversion data from xml file
     # need first to find the file. It is in the same directory as the script
     parent_dir = os.path.dirname(os.path.realpath(__file__))
     xml_file = os.path.join(parent_dir, 'asc_to_qsch_data.xml')
@@ -89,16 +93,16 @@
         symbol_tag = symbol_stock.get(comp.symbol, None)
         if symbol_tag is None:
             # Will try to get it from the sym folder
             print(f"Searching for symbol {comp.symbol}...")
             for sym_root in search_paths + [
                 # os.path.curdir,  # The current script directory
                 os.path.split(asc_file)[0],  # The directory where the scrip is located
-                os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
-                os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sym"),
+                os.path.expanduser("~/AppData/Local/LTspice/lib/sym"),
+                os.path.expanduser("~/Documents/LtspiceXVII/lib/sym"),
                 # os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"), # TODO: implement this
             ]:
                 print(f"   {os.path.abspath(sym_root)}")
                 if not os.path.exists(sym_root):  # Skipping invalid paths
                     continue
                 if sym_root.endswith('.zip'):  # TODO: test if it is a file
                     pass
```

### Comparing `spicelib-1.1.2/spicelib/scripts/asc_to_qsch_data.xml` & `spicelib-1.1.3/spicelib/scripts/asc_to_qsch_data.xml`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/scripts/histogram.py` & `spicelib-1.1.3/spicelib/scripts/histogram.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/scripts/ltsteps.py` & `spicelib-1.1.3/spicelib/scripts/ltsteps.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/scripts/rawplot.py` & `spicelib-1.1.3/spicelib/scripts/rawplot.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/scripts/readme_update.py` & `spicelib-1.1.3/spicelib/scripts/readme_update.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/scripts/run_server.py` & `spicelib-1.1.3/spicelib/scripts/run_server.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/process_callback.py` & `spicelib-1.1.3/spicelib/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/run_task.py` & `spicelib-1.1.3/spicelib/sim/run_task.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/sim_runner.py` & `spicelib-1.1.3/spicelib/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/sim_stepping.py` & `spicelib-1.1.3/spicelib/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/simulator.py` & `spicelib-1.1.3/spicelib/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/failure_modes.py` & `spicelib-1.1.3/spicelib/sim/tookit/failure_modes.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/fast_worst_case.py` & `spicelib-1.1.3/spicelib/sim/tookit/fast_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/montecarlo.py` & `spicelib-1.1.3/spicelib/sim/tookit/montecarlo.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/quick_sensitivity_analysis.py` & `spicelib-1.1.3/spicelib/sim/tookit/quick_sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/sim_analysis.py` & `spicelib-1.1.3/spicelib/sim/tookit/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/tolerance_deviations.py` & `spicelib-1.1.3/spicelib/sim/tookit/tolerance_deviations.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/sim/tookit/worst_case.py` & `spicelib-1.1.3/spicelib/sim/tookit/worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/simulators/ltspice_simulator.py` & `spicelib-1.1.3/spicelib/simulators/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/simulators/ngspice_simulator.py` & `spicelib-1.1.3/spicelib/simulators/ngspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/simulators/qspice_simulator.py` & `spicelib-1.1.3/spicelib/simulators/qspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/simulators/xyce_simulator.py` & `spicelib-1.1.3/spicelib/simulators/xyce_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/utils/detect_encoding.py` & `spicelib-1.1.3/spicelib/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/utils/file_search.py` & `spicelib-1.1.3/spicelib/utils/file_search.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/utils/sweep_iterators.py` & `spicelib-1.1.3/spicelib/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib/utils/windows_short_names.py` & `spicelib-1.1.3/spicelib/utils/windows_short_names.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/spicelib.egg-info/PKG-INFO` & `spicelib-1.1.3/spicelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicelib
-Version: 1.1.2
+Version: 1.1.3
 Summary: A set of tools to Automate Spice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1185,14 +1185,24 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+
+* Version 1.1.3
+  * Implementing a set_component_parameters() and get_component_parameters() method on the Editor classes. 
+    This method allows to set and get the parameters of a component.
+  * Bug Fixes:
+    * AscEditor was hanging in comments. Issue #43
+    * Supporting other text orientations on the AscEditor. Issue #44
+    * Allow other encodings in AscEditor. Issues #45 and #48
+  * Supporting lines, rectangles, circles and arcs in AscEditor.
+  * Improving the regex for the component values in the SpiceEditor. 
 * Version 1.1.2
   * Fixes on the readme_update.py script. Was not supporting spaces after the []
   * Solving issue PyLTspice Issue #138. Hierarchical edits to ASC files are now supported.
 * Version 1.1.1
   * Supporting hierarchical edits on both QSpice and LTspice schematics
   * Skipping the need of the rich library on examples
   * Giving feedback on the search for symbols on the ASC to QSCH conversion
```

### Comparing `spicelib-1.1.2/spicelib.egg-info/SOURCES.txt` & `spicelib-1.1.3/spicelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/unittests/sweep_iterators_unittest.py` & `spicelib-1.1.3/unittests/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/unittests/test_asc_editor.py` & `spicelib-1.1.3/unittests/test_asc_editor.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,55 +25,64 @@
 sys.path.append(
     os.path.abspath((os.path.dirname(os.path.abspath(__file__)) + "/../")))  # add project root to lib search path
 
 import spicelib
 
 test_dir = '../examples/testfiles/' if os.path.abspath(os.curdir).endswith('unittests') else './examples/testfiles/'
 golden_dir = './golden/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/golden/'
+temp_dir = './temp/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/temp/'
 
+if not os.path.exists(temp_dir):
+    os.mkdir(temp_dir)
 
 class ASC_Editor_Test(unittest.TestCase):
 
     def setUp(self):
         self.edt = spicelib.editor.asc_editor.AscEditor(test_dir + "DC sweep.asc")
 
     def test_component_editing(self):
         self.assertEqual(self.edt.get_component_value('R1'), '10k', "Tested R1 Value")  # add assertion here
         self.assertListEqual(self.edt.get_components(), ['Vin', 'R1', 'R2', 'D1'], "Tested get_components")  # add assertion here
         self.edt.set_component_value('R1', '33k')
-        self.edt.save_netlist(test_dir + 'test_components_output.asc')
-        self.equalFiles(test_dir + 'test_components_output.asc', golden_dir + 'test_components_output.asc')
+        self.edt.save_netlist(temp_dir + 'test_components_output.asc')
+        self.equalFiles(temp_dir + 'test_components_output.asc', golden_dir + 'test_components_output.asc')
         self.assertEqual(self.edt.get_component_value('R1'), '33k', "Tested R1 Value")  # add assertion here
+        self.edt.set_component_parameters('R1', Tc1='0', Tc2='0', pwr=None)
+        self.edt.save_netlist(temp_dir + 'test_components_output_2.asc')
+        self.equalFiles(temp_dir + 'test_components_output_2.asc', golden_dir + 'test_components_output_2.asc')
+        r1_params = self.edt.get_component_parameters('R1')
+        for key, value in {'Tc1': 0, 'Tc2': 0}.items():
+            self.assertEqual(r1_params[key], value, f"Tested R1 {key} Parameter")
         self.edt.remove_component('R1')
-        self.edt.save_netlist(test_dir + 'test_components_output_1.asc')
-        self.equalFiles(test_dir + 'test_components_output_1.asc', golden_dir + 'test_components_output_1.asc')
+        self.edt.save_netlist(temp_dir + 'test_components_output_1.asc')
+        self.equalFiles(temp_dir + 'test_components_output_1.asc', golden_dir + 'test_components_output_1.asc')
 
     def test_parameter_edit(self):
         self.assertEqual(self.edt.get_parameter('TEMP'), '0', "Tested TEMP Parameter")  # add assertion here
         self.edt.set_parameter('TEMP', 25)
         self.assertEqual(self.edt.get_parameter('TEMP'), '25', "Tested TEMP Parameter")  # add assertion here
-        self.edt.save_netlist(test_dir + 'test_parameter_output.asc')
-        self.equalFiles(test_dir + 'test_parameter_output.asc', golden_dir + 'test_parameter_output.asc')
+        self.edt.save_netlist(temp_dir + 'test_parameter_output.asc')
+        self.equalFiles(temp_dir + 'test_parameter_output.asc', golden_dir + 'test_parameter_output.asc')
         self.edt.set_parameter('TEMP', 0)  # reset to 0
         self.assertEqual(self.edt.get_parameter('TEMP'), '0', "Tested TEMP Parameter")  # add assertion here
 
     def test_instructions(self):
         self.edt.add_instruction('.ac dec 10 1 100k')
         self.edt.add_instruction('.save V(vout)')
         self.edt.add_instruction('.save I(R1)')
         self.edt.add_instruction('.save I(R2)')
         self.edt.add_instruction('.save I(D1)')
-        self.edt.save_netlist(test_dir + 'test_instructions_output.asc')
-        self.equalFiles(test_dir + 'test_instructions_output.asc', golden_dir + 'test_instructions_output.asc')
+        self.edt.save_netlist(temp_dir + 'test_instructions_output.asc')
+        self.equalFiles(temp_dir + 'test_instructions_output.asc', golden_dir + 'test_instructions_output.asc')
         self.edt.remove_instruction('.save I(R1)')
-        self.edt.save_netlist(test_dir + 'test_instructions_output_1.asc')
-        self.equalFiles(test_dir + 'test_instructions_output_1.asc', golden_dir + 'test_instructions_output_1.asc')
+        self.edt.save_netlist(temp_dir + 'test_instructions_output_1.asc')
+        self.equalFiles(temp_dir + 'test_instructions_output_1.asc', golden_dir + 'test_instructions_output_1.asc')
         self.edt.remove_Xinstruction(r"\.save\sI\(.*\)")  # removes all .save instructions for currents
-        self.edt.save_netlist(test_dir + 'test_instructions_output_2.asc')
-        self.equalFiles(test_dir + 'test_instructions_output_2.asc', golden_dir + 'test_instructions_output_2.asc')
+        self.edt.save_netlist(temp_dir + 'test_instructions_output_2.asc')
+        self.equalFiles(temp_dir + 'test_instructions_output_2.asc', golden_dir + 'test_instructions_output_2.asc')
 
     def equalFiles(self, file1, file2):
         with open(file1, 'r') as f1:
             lines1 = f1.readlines()
         with open(file2, 'r') as f2:
             lines2 = f2.readlines()
         self.assertEqual(len(lines1), len(lines2), "Number of lines is different")
```

### Comparing `spicelib-1.1.2/unittests/test_qsch_editor.py` & `spicelib-1.1.3/unittests/test_qsch_editor.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,28 +17,33 @@
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 import os
 import sys
 import unittest
+import logging
 
 sys.path.append(
     os.path.abspath((os.path.dirname(os.path.abspath(__file__)) + "/../")))  # add project root to lib search path
 
 import spicelib
 
 test_dir = '../examples/testfiles/' if os.path.abspath(os.curdir).endswith('unittests') else './examples/testfiles/'
 golden_dir = './golden/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/golden/'
 temp_dir = './temp/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/temp/'
 
 if not os.path.exists(temp_dir):
     os.mkdir(temp_dir)
 
 
+# set the logger to print to console and at info level
+spicelib.set_log_level(logging.INFO)
+
+
 def equalFiles(testcase, file1, file2):
     with open(file1, 'r', encoding='cp1252') as f1:
         lines1 = f1.readlines()
     with open(file2, 'r', encoding='cp1252') as f2:
         lines2 = f2.readlines()
     testcase.assertEqual(len(lines1), len(lines2), "Files have different number of lines")
     for i in range(len(lines1)):
@@ -57,14 +62,20 @@
     def test_component_editing(self):
         self.assertEqual(self.edt.get_component_value('R1'), '10K', "Tested R1 Value")  # add assertion here
         self.assertSetEqual(set(self.edt.get_components()), set(('Vin', 'R1', 'R2', 'D1')), "Tested get_components")  # add assertion here
         self.edt.set_component_value('R1', '33K')
         self.edt.save_netlist(temp_dir + 'test_components_output.qsch')
         equalFiles(self, temp_dir + 'test_components_output.qsch', golden_dir + 'test_components_output.qsch')
         self.assertEqual(self.edt.get_component_value('R1'), '33K', "Tested R1 Value")  # add assertion here
+        self.edt.set_component_parameters('R1', Tc1=0, Tc2=0)
+        self.edt.save_netlist(temp_dir + 'test_components_output_2.qsch')
+        equalFiles(self, temp_dir + 'test_components_output_2.qsch', golden_dir + 'test_components_output_2.qsch')
+        r1_params = self.edt.get_component_parameters('R1')
+        for key, value in {'Tc1': '0', 'Tc2': '0'}.items():
+            self.assertEqual(r1_params[key], value, f"Tested R1 {key} Parameter")
         self.edt.remove_component('R1')
         self.edt.save_netlist(temp_dir + 'test_components_output_1.qsch')
         equalFiles(self, temp_dir + 'test_components_output_1.qsch', golden_dir + 'test_components_output_1.qsch')
 
     def test_parameter_edit(self):
         self.assertEqual(self.edt.get_parameter('TEMP'), '0', "Tested TEMP Parameter")  # add assertion here
         self.edt.set_parameter('TEMP', 25)
@@ -85,15 +96,14 @@
         self.edt.remove_instruction('.save I(R1)')
         self.edt.save_netlist(temp_dir + 'test_instructions_output_1.qsch')
         equalFiles(self, temp_dir + 'test_instructions_output_1.qsch', golden_dir + 'test_instructions_output_1.qsch')
         self.edt.remove_Xinstruction(r"\.save\sI\(.*\)")  # removes all .save instructions for currents
         self.edt.save_netlist(temp_dir + 'test_instructions_output_2.qsch')
         equalFiles(self, temp_dir + 'test_instructions_output_2.qsch', golden_dir + 'test_instructions_output_2.qsch')
 
-
 class QschEditorRotation(unittest.TestCase):
 
     def test_component_rotations(self):
         self.edt = spicelib.editor.qsch_editor.QschEditor(test_dir + "qsch_rotation.qsch")
         self.edt.save_netlist(temp_dir + 'qsch_rotation.net')
         equalFiles(self, temp_dir + 'qsch_rotation.net', golden_dir + "qsch_rotation.net")
         self.qsch = spicelib.editor.qsch_editor.QschEditor(test_dir + 'qsch_rotation_set_test.qsch')
@@ -110,9 +120,22 @@
         self.edt.save_netlist(temp_dir + "top_circuit.net")
         if sys.platform.startswith("win"):
             equalFiles(self, temp_dir + 'top_circuit.net', golden_dir + "top_circuit_win32.net")
         else:
             equalFiles(self, temp_dir + 'top_circuit.net', golden_dir + "top_circuit.net")
 
 
+class QschEditorFromAscConversion(unittest.TestCase):
+
+    def test_asc_to_qsch(self):
+        from spicelib.scripts.asc_to_qsch import convert_asc_to_qsch
+        convert_asc_to_qsch(test_dir + "DC sweep.asc", temp_dir + "DC_sweep_from_asc.qsch")
+        equalFiles(self, temp_dir + 'DC_sweep_from_asc.qsch', golden_dir + "DC_sweep_from_asc.qsch")
+
+    # def test_qsch_to_asc(self):
+    #     self.edt = spicelib.editor.qsch_editor.QschEditor(test_dir + "DC sweep.qsch")
+    #     self.edt.save_asc(temp_dir + "DC sweep.asc")
+    #     equalFiles(self, temp_dir + 'DC sweep.asc', golden_dir + "DC sweep.asc")
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `spicelib-1.1.2/unittests/test_qspice_rawread.py` & `spicelib-1.1.3/unittests/test_qspice_rawread.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.1.2/unittests/test_spice_editor.py` & `spicelib-1.1.3/unittests/test_spice_editor.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,55 +25,64 @@
 sys.path.append(
     os.path.abspath((os.path.dirname(os.path.abspath(__file__)) + "/../")))  # add project root to lib search path
 
 import spicelib
 
 test_dir = '../examples/testfiles/' if os.path.abspath(os.curdir).endswith('unittests') else './examples/testfiles/'
 golden_dir = './golden/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/golden/'
+temp_dir = './temp/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/temp/'
 
+if not os.path.exists(temp_dir):
+    os.mkdir(temp_dir)
 
 class SpiceEditor_Test(unittest.TestCase):
 
     def setUp(self):
         self.edt = spicelib.editor.spice_editor.SpiceEditor(test_dir + "DC sweep.net")
 
     def test_component_editing(self):
         self.assertEqual(self.edt.get_component_value('R1'), '10k', "Tested R1 Value")  # add assertion here
         self.assertListEqual(self.edt.get_components(), ['Vin', 'R1', 'R2', 'D1'], "Tested get_components")  # add assertion here
         self.edt.set_component_value('R1', '33k')
-        self.edt.save_netlist(test_dir + 'test_components_output.net')
-        self.equalFiles(test_dir + 'test_components_output.net', golden_dir + 'test_components_output.net')
+        self.edt.save_netlist(temp_dir + 'test_components_output.net')
+        self.equalFiles(temp_dir + 'test_components_output.net', golden_dir + 'test_components_output.net')
         self.assertEqual(self.edt.get_component_value('R1'), '33k', "Tested R1 Value")  # add assertion here
+        self.edt.set_component_parameters('R1', Tc1=0, Tc2=0, pwr=None)
+        self.edt.save_netlist(temp_dir + 'test_components_output_2.net')
+        self.equalFiles(temp_dir + 'test_components_output_2.net', golden_dir + 'test_components_output_2.net')
+        r1_params = self.edt.get_component_parameters('R1')
+        for key, value in {'Tc1': 0, 'Tc2': 0}.items():
+            self.assertEqual(r1_params[key], value, f"Tested R1 {key} Parameter")
         self.edt.remove_component('R1')
-        self.edt.save_netlist(test_dir + 'test_components_output_1.net')
-        self.equalFiles(test_dir + 'test_components_output_1.net', golden_dir + 'test_components_output_1.net')
+        self.edt.save_netlist(temp_dir + 'test_components_output_1.net')
+        self.equalFiles(temp_dir + 'test_components_output_1.net', golden_dir + 'test_components_output_1.net')
 
     def test_parameter_edit(self):
         self.assertEqual(self.edt.get_parameter('TEMP'), '0', "Tested TEMP Parameter")  # add assertion here
         self.edt.set_parameter('TEMP', 25)
         self.assertEqual(self.edt.get_parameter('TEMP'), '25', "Tested TEMP Parameter")  # add assertion here
-        self.edt.save_netlist(test_dir + 'test_parameter_output.net')
-        self.equalFiles(test_dir + 'test_parameter_output.net', golden_dir + 'test_parameter_output.net')
+        self.edt.save_netlist(temp_dir + 'test_parameter_output.net')
+        self.equalFiles(temp_dir + 'test_parameter_output.net', golden_dir + 'test_parameter_output.net')
         self.edt.set_parameter('TEMP', 0)  # reset to 0
         self.assertEqual(self.edt.get_parameter('TEMP'), '0', "Tested TEMP Parameter")  # add assertion here
 
     def test_instructions(self):
         self.edt.add_instruction('.ac dec 10 1 100k')
         self.edt.add_instruction('.save V(vout)')
         self.edt.add_instruction('.save I(R1)')
         self.edt.add_instruction('.save I(R2)')
         self.edt.add_instruction('.save I(D1)')
-        self.edt.save_netlist(test_dir + 'test_instructions_output.net')
-        self.equalFiles(test_dir + 'test_instructions_output.net', golden_dir + 'test_instructions_output.net')
+        self.edt.save_netlist(temp_dir + 'test_instructions_output.net')
+        self.equalFiles(temp_dir + 'test_instructions_output.net', golden_dir + 'test_instructions_output.net')
         self.edt.remove_instruction('.save I(R1)')
-        self.edt.save_netlist(test_dir + 'test_instructions_output_1.net')
-        self.equalFiles(test_dir + 'test_instructions_output_1.net', golden_dir + 'test_instructions_output_1.net')
+        self.edt.save_netlist(temp_dir + 'test_instructions_output_1.net')
+        self.equalFiles(temp_dir + 'test_instructions_output_1.net', golden_dir + 'test_instructions_output_1.net')
         self.edt.remove_Xinstruction(r"\.save\sI\(.*\)")  # removes all .save instructions for currents
-        self.edt.save_netlist(test_dir + 'test_instructions_output_2.net')
-        self.equalFiles(test_dir + 'test_instructions_output_2.net', golden_dir + 'test_instructions_output_2.net')
+        self.edt.save_netlist(temp_dir + 'test_instructions_output_2.net')
+        self.equalFiles(temp_dir + 'test_instructions_output_2.net', golden_dir + 'test_instructions_output_2.net')
 
     def equalFiles(self, file1, file2):
         with open(file1, 'r') as f1:
             lines1 = f1.readlines()
         with open(file2, 'r') as f2:
             lines2 = f2.readlines()
         self.assertEqual(len(lines1), len(lines2), "Files have different number of lines")
```

### Comparing `spicelib-1.1.2/unittests/test_spicelib.py` & `spicelib-1.1.3/unittests/test_spicelib.py`

 * *Files identical despite different names*

