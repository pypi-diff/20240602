# Comparing `tmp/codeflash-0.6.5.tar.gz` & `tmp/codeflash-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.6.5.tar", max compression
+gzip compressed data, was "codeflash-0.6.6.tar", max compression
```

## Comparing `codeflash-0.6.5.tar` & `codeflash-0.6.6.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.5/README.md
--rw-r--r--   0        0        0     4405 2024-05-31 21:03:43.421623 codeflash-0.6.5/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.5/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.5/codeflash/api/__init__.py
--rw-r--r--   0        0        0     8936 2024-05-31 21:03:09.269838 codeflash-0.6.5/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4833 2024-05-30 23:15:57.599950 codeflash-0.6.5/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.5/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     8042 2024-05-31 20:15:40.283230 codeflash-0.6.5/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0      305 2024-05-30 23:15:57.600218 codeflash-0.6.5/codeflash/cli_cmds/cli_common.py
--rw-r--r--   0        0        0    22606 2024-05-31 20:15:40.283425 codeflash-0.6.5/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      475 2024-05-30 23:15:57.600580 codeflash-0.6.5/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1835 2024-05-30 23:15:57.600684 codeflash-0.6.5/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.5/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     9586 2024-05-30 23:15:57.600858 codeflash-0.6.5/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     8556 2024-05-30 23:15:57.601031 codeflash-0.6.5/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2956 2024-05-30 23:15:57.601170 codeflash-0.6.5/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.5/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.5/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3464 2024-05-31 20:15:40.283606 codeflash-0.6.5/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2979 2024-05-30 23:15:57.601358 codeflash-0.6.5/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     2056 2024-05-30 23:15:57.601485 codeflash-0.6.5/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3143 2024-05-30 23:15:57.601623 codeflash-0.6.5/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0     1083 2024-05-30 23:15:57.601723 codeflash-0.6.5/codeflash/code_utils/github_utils.py
--rw-r--r--   0        0        0    24003 2024-05-30 23:15:57.601895 codeflash-0.6.5/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.5/codeflash/code_utils/main_calls_bubblesort.py
--rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.5/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0        0 2024-05-30 23:15:57.601953 codeflash-0.6.5/codeflash/code_utils/sqlalchemy_experiment.py
--rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.5/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1898 2024-05-30 23:15:57.602091 codeflash-0.6.5/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.5/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    18481 2024-05-30 23:15:57.602285 codeflash-0.6.5/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    20032 2024-05-30 23:15:57.602480 codeflash-0.6.5/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1291 2024-05-30 23:15:57.602653 codeflash-0.6.5/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.5/codeflash/github/__init__.py
--rw-r--r--   0        0        0      725 2024-05-29 01:00:54.268195 codeflash-0.6.5/codeflash/main.py
--rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.5/codeflash/models/ExperimentMetadata.py
--rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.5/codeflash/models/__init__.py
--rw-r--r--   0        0        0     1218 2024-05-31 20:15:40.283706 codeflash-0.6.5/codeflash/models/models.py
--rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.5/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    12006 2024-05-30 23:15:57.602810 codeflash-0.6.5/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0    52972 2024-05-31 21:03:09.270371 codeflash-0.6.5/codeflash/optimization/optimizer.py
--rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.5/codeflash/result/__init__.py
--rw-r--r--   0        0        0     4539 2024-05-30 23:15:57.603224 codeflash-0.6.5/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1667 2024-05-31 20:15:40.284056 codeflash-0.6.5/codeflash/result/critic.py
--rw-r--r--   0        0        0     1992 2024-05-30 23:15:57.603526 codeflash-0.6.5/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.5/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.5/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-05-31 21:03:09.270524 codeflash-0.6.5/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0    20467 2024-05-30 23:15:57.603649 codeflash-0.6.5/codeflash/tracer.py
--rw-r--r--   0        0        0        1 2024-05-30 23:15:57.603926 codeflash-0.6.5/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     2644 2024-05-30 23:15:57.604036 codeflash-0.6.5/codeflash/tracing/profile_stats.py
--rw-r--r--   0        0        0     5942 2024-05-30 23:15:57.604189 codeflash-0.6.5/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.5/codeflash/tracing/tracing_utils.py
--rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.5/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.5/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.5/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1241 2024-05-30 23:15:57.604500 codeflash-0.6.5/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14621 2024-05-30 23:15:57.604745 codeflash-0.6.5/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6830 2024-05-30 23:15:57.604952 codeflash-0.6.5/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1759 2024-05-30 23:15:57.605103 codeflash-0.6.5/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.5/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4189 2024-05-31 21:03:09.270676 codeflash-0.6.5/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-05-31 21:04:03.043254 codeflash-0.6.5/codeflash/version.py
--rw-r--r--   0        0        0     2963 2024-05-31 21:04:03.042230 codeflash-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.6.6/README.md
+-rw-r--r--   0        0        0     4405 2024-06-02 01:38:12.569772 codeflash-0.6.6/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.6.6/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.6.6/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     8936 2024-06-02 01:27:16.665257 codeflash-0.6.6/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4833 2024-06-01 04:35:39.379646 codeflash-0.6.6/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.6.6/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     8042 2024-06-01 04:35:39.379832 codeflash-0.6.6/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0      305 2024-06-01 04:35:39.379938 codeflash-0.6.6/codeflash/cli_cmds/cli_common.py
+-rw-r--r--   0        0        0    22606 2024-06-01 04:35:39.380100 codeflash-0.6.6/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      475 2024-06-01 04:35:39.380471 codeflash-0.6.6/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1835 2024-06-01 04:35:39.380833 codeflash-0.6.6/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.6.6/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     9586 2024-06-02 01:27:16.665741 codeflash-0.6.6/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     8556 2024-05-13 05:06:56.603994 codeflash-0.6.6/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2956 2024-05-11 03:50:31.230947 codeflash-0.6.6/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-04-15 22:14:14.315668 codeflash-0.6.6/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      228 2024-06-01 21:08:08.727677 codeflash-0.6.6/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3464 2024-06-01 04:35:39.381269 codeflash-0.6.6/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2979 2024-06-01 04:35:39.381687 codeflash-0.6.6/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-11 03:50:31.232101 codeflash-0.6.6/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3143 2024-06-01 04:35:39.381871 codeflash-0.6.6/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0     1083 2024-06-01 04:35:39.381957 codeflash-0.6.6/codeflash/code_utils/github_utils.py
+-rw-r--r--   0        0        0    26294 2024-06-01 21:08:08.727862 codeflash-0.6.6/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0     3497 2024-04-18 23:24:18.257591 codeflash-0.6.6/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0        0 2024-06-01 04:35:39.382170 codeflash-0.6.6/codeflash/code_utils/sqlalchemy_experiment.py
+-rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.6.6/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1898 2024-05-13 05:06:56.605285 codeflash-0.6.6/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.6.6/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    18481 2024-06-01 04:35:39.382794 codeflash-0.6.6/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    20032 2024-05-14 17:53:59.915027 codeflash-0.6.6/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1291 2024-05-29 19:28:20.152304 codeflash-0.6.6/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.6.6/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-05-07 21:23:45.633992 codeflash-0.6.6/codeflash/main.py
+-rw-r--r--   0        0        0      133 2024-05-11 03:50:31.233935 codeflash-0.6.6/codeflash/models/ExperimentMetadata.py
+-rw-r--r--   0        0        0        0 2024-05-11 03:50:31.233961 codeflash-0.6.6/codeflash/models/__init__.py
+-rw-r--r--   0        0        0     1218 2024-06-01 04:35:39.382925 codeflash-0.6.6/codeflash/models/models.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.6.6/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    13016 2024-06-01 21:08:08.728533 codeflash-0.6.6/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    53202 2024-06-02 01:28:34.083534 codeflash-0.6.6/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.6.6/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4539 2024-05-13 05:06:56.606567 codeflash-0.6.6/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1667 2024-06-01 04:35:39.383742 codeflash-0.6.6/codeflash/result/critic.py
+-rw-r--r--   0        0        0     1992 2024-05-13 05:06:56.607228 codeflash-0.6.6/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.6.6/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1319 2024-06-01 21:08:08.729489 codeflash-0.6.6/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-06-02 01:27:16.666468 codeflash-0.6.6/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0    20467 2024-05-11 03:50:31.235086 codeflash-0.6.6/codeflash/tracer.py
+-rw-r--r--   0        0        0        1 2024-05-11 03:50:31.235685 codeflash-0.6.6/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-11 03:50:31.235798 codeflash-0.6.6/codeflash/tracing/profile_stats.py
+-rw-r--r--   0        0        0     5942 2024-05-11 03:50:31.235999 codeflash-0.6.6/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0      210 2024-05-09 02:05:53.366617 codeflash-0.6.6/codeflash/tracing/tracing_utils.py
+-rw-r--r--   0        0        0     1905 2024-04-18 03:01:28.781529 codeflash-0.6.6/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.6.6/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4977 2024-05-11 03:50:31.236508 codeflash-0.6.6/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1556 2024-06-01 21:08:08.729617 codeflash-0.6.6/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    17658 2024-06-01 21:08:08.729925 codeflash-0.6.6/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6893 2024-06-01 21:08:08.730052 codeflash-0.6.6/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1856 2024-06-01 21:08:08.730188 codeflash-0.6.6/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2338 2024-05-09 02:05:53.368797 codeflash-0.6.6/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4189 2024-06-02 01:27:16.666628 codeflash-0.6.6/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-06-02 01:39:33.189922 codeflash-0.6.6/codeflash/version.py
+-rw-r--r--   0        0        0     3065 2024-06-02 01:39:33.188380 codeflash-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.6/PKG-INFO
```

### Comparing `codeflash-0.6.5/codeflash/LICENSE` & `codeflash-0.6.6/codeflash/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/api/aiservice.py` & `codeflash-0.6.6/codeflash/api/aiservice.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/api/cfapi.py` & `codeflash-0.6.6/codeflash/api/cfapi.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/cli_cmds/cli.py` & `codeflash-0.6.6/codeflash/cli_cmds/cli.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.6.6/codeflash/cli_cmds/cmd_init.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.6.6/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/code_extractor.py` & `codeflash-0.6.6/codeflash/code_utils/code_extractor.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/code_replacer.py` & `codeflash-0.6.6/codeflash/code_utils/code_replacer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/code_utils.py` & `codeflash-0.6.6/codeflash/code_utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/config_parser.py` & `codeflash-0.6.6/codeflash/code_utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/env_utils.py` & `codeflash-0.6.6/codeflash/code_utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/formatter.py` & `codeflash-0.6.6/codeflash/code_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/git_utils.py` & `codeflash-0.6.6/codeflash/code_utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/github_utils.py` & `codeflash-0.6.6/codeflash/code_utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.6.6/codeflash/code_utils/instrument_existing_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,14 +462,59 @@
                         ),
                     ],
                 ),
                 lineno=lineno + 8,
             ),
             ast.Expr(
                 value=ast.Call(
+                    func=ast.Name(id="print", ctx=ast.Load()),
+                    args=[
+                        ast.JoinedStr(
+                            values=[
+                                ast.Constant(value="!######"),
+                                ast.FormattedValue(
+                                    value=ast.Name(id="test_module_name", ctx=ast.Load()),
+                                    conversion=-1,
+                                ),
+                                ast.Constant(value=":"),
+                                ast.FormattedValue(
+                                    value=ast.IfExp(
+                                        test=ast.Name(id="test_class_name", ctx=ast.Load()),
+                                        body=ast.BinOp(
+                                            left=ast.Name(id="test_class_name", ctx=ast.Load()),
+                                            op=ast.Add(),
+                                            right=ast.Constant(value="."),
+                                        ),
+                                        orelse=ast.Constant(value=""),
+                                    ),
+                                    conversion=-1,
+                                ),
+                                ast.FormattedValue(
+                                    value=ast.Name(id="test_name", ctx=ast.Load()),
+                                    conversion=-1,
+                                ),
+                                ast.Constant(value=":"),
+                                ast.FormattedValue(
+                                    value=ast.Name(id="function_name", ctx=ast.Load()),
+                                    conversion=-1,
+                                ),
+                                ast.Constant(value=":"),
+                                ast.FormattedValue(
+                                    value=ast.Name(id="invocation_id", ctx=ast.Load()),
+                                    conversion=-1,
+                                ),
+                                ast.Constant(value="######!"),
+                            ],
+                        ),
+                    ],
+                    keywords=[],
+                ),
+            ),
+            ast.Expr(
+                value=ast.Call(
                     func=ast.Attribute(
                         value=ast.Name(id="gc", ctx=ast.Load()),
                         attr="disable",
                         ctx=ast.Load(),
                     ),
                     args=[],
                     keywords=[],
```

### Comparing `codeflash-0.6.5/codeflash/code_utils/shell_utils.py` & `codeflash-0.6.6/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.6.6/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/code_utils/time_utils.py` & `codeflash-0.6.6/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.6.6/codeflash/discovery/discover_unit_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.6.6/codeflash/discovery/functions_to_optimize.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/github/PrComment.py` & `codeflash-0.6.6/codeflash/github/PrComment.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/main.py` & `codeflash-0.6.6/codeflash/main.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/models/models.py` & `codeflash-0.6.6/codeflash/models/models.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/optimization/function_context.py` & `codeflash-0.6.6/codeflash/optimization/function_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import ast
 import logging
 import os
-from typing import Union
+import re
+from typing import Tuple, Union
 
 import jedi
 import tiktoken
 from jedi.api.classes import Name
 from pydantic.dataclasses import dataclass
 
-from codeflash.code_utils.code_extractor import get_code, get_code_no_skeleton
-from codeflash.code_utils.code_utils import path_belongs_to_site_packages
+from codeflash.code_utils.code_extractor import get_code
+from codeflash.code_utils.code_utils import module_name_from_file_path, path_belongs_to_site_packages
 from codeflash.discovery.functions_to_optimize import FunctionParent, FunctionToOptimize
 
 
 def belongs_to_class(name: Name, class_name: str) -> bool:
     """Check if the given name belongs to the specified class."""
     if name.full_name and name.full_name.startswith(f"{name.module_name}.{class_name}."):
         return True
@@ -49,14 +50,15 @@
     try:
         module: ast.Module = ast.parse(file_contents)
     except SyntaxError as e:
         logging.exception(f"get_type_annotation_context - Syntax error in code: {e}")
         return []
     sources: list[tuple[Source, str, str]] = []
     ast_parents: list[FunctionParent] = []
+    contextual_dunder_methods = set()
 
     def get_annotation_source(
         jedi_script: jedi.Script,
         name: str,
         node_parents,
         line_no: int,
         col_no: str,
@@ -89,29 +91,30 @@
                     [
                         FunctionToOptimize(
                             definition[0].name,
                             definition_path,
                             node_parents[:-1],
                         ),
                     ],
-                )[0]
-                if source_code:
+                )
+                if source_code[0]:
                     sources.append(
                         (
                             Source(
                                 definition[0].full_name,
                                 definition[0],
-                                source_code,
+                                source_code[0],
                             ),
                             definition_path,
                             definition[0].full_name.removeprefix(
                                 definition[0].module_name + ".",
                             ),
                         ),
                     )
+                    contextual_dunder_methods.update(source_code[1])
 
     def visit_children(
         node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module],
         node_parents: list[FunctionParent],
     ) -> None:
         child: Union[ast.AST, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module]
         for child in ast.iter_child_nodes(node):
@@ -160,25 +163,26 @@
                 node_parents.append(FunctionParent(node.name, type(node).__name__))
             visit_children(node, node_parents)
             if not isinstance(node, ast.Module):
                 node_parents.pop()
 
     visit(module, ast_parents)
 
-    return sources
+    return sources, contextual_dunder_methods
 
 
 def get_function_variables_definitions(
     function_to_optimize: FunctionToOptimize,
     project_root_path: str,
-) -> list[tuple[Source, str, str]]:
+) -> Tuple[list[tuple[Source, str, str]], set[tuple[str, str]]]:
     function_name = function_to_optimize.function_name
     file_path = function_to_optimize.file_path
     script = jedi.Script(path=file_path, project=jedi.Project(path=project_root_path))
     sources: list[tuple[Source, str, str]] = []
+    contextual_dunder_methods = set()
     # TODO: The function name condition can be stricter so that it does not clash with other class names etc.
     # TODO: The function could have been imported as some other name,
     #  we should be checking for the translation as well. Also check for the original function name.
     names = []
     for ref in script.get_names(all_scopes=True, definitions=False, references=True):
         if ref.full_name:
             if function_to_optimize.parents:
@@ -211,50 +215,66 @@
             # The definition is part of this project and not defined within the original function
             if (
                 definition_path.startswith(project_root_path + os.sep)
                 and not path_belongs_to_site_packages(definition_path)
                 and definition.full_name
                 and not belongs_to_function(definition, function_name)
             ):
-                source_code = get_code_no_skeleton(definition_path, definitions[0].name)
-                if source_code:
+                module_name = module_name_from_file_path(definition_path, project_root_path)
+                m = re.match(rf"{module_name}\.(.*)\.{definitions[0].name}", definitions[0].full_name)
+                parents = []
+                if m:
+                    parents = [FunctionParent(m.group(1), "ClassDef")]
+
+                source_code = get_code(
+                    [
+                        FunctionToOptimize(
+                            function_name=definitions[0].name,
+                            file_path=definition_path,
+                            parents=parents,
+                        ),
+                    ],
+                )
+                if source_code[0]:
                     sources.append(
                         (
-                            Source(definition.full_name, definition, source_code),
+                            Source(definition.full_name, definition, source_code[0]),
                             definition_path,
                             definition.full_name.removeprefix(name.module_name + "."),
                         ),
                     )
-    annotation_sources = get_type_annotation_context(
+                    contextual_dunder_methods.update(source_code[1])
+    annotation_sources, annotation_dunder_methods = get_type_annotation_context(
         function_to_optimize,
         script,
         project_root_path,
     )
     sources[:0] = annotation_sources  # prepend the annotation sources
+    contextual_dunder_methods.update(annotation_dunder_methods)
     deduped_sources = []
     existing_full_names = set()
     for source in sources:
         if source[0].full_name not in existing_full_names:
             deduped_sources.append(source)
             existing_full_names.add(source[0].full_name)
-    return deduped_sources
+    return deduped_sources, contextual_dunder_methods
 
 
 MAX_PROMPT_TOKENS = 4096  # 128000  # gpt-4-128k
 
 
 def get_constrained_function_context_and_helper_functions(
     function_to_optimize: FunctionToOptimize,
     project_root_path: str,
     code_to_optimize: str,
     max_tokens: int = MAX_PROMPT_TOKENS,
-) -> tuple[str, list[tuple[Source, str, str]]]:
+) -> tuple[str, list[tuple[Source, str, str]], set[tuple[str, str]]]:
     # TODO: Not just do static analysis, but also find the datatypes of function arguments by running the existing
     #  unittests and inspecting the arguments to resolve the real definitions and dependencies.
-    helper_functions: list[tuple[Source, str, str]] = get_function_variables_definitions(
+    helper_functions, dunder_methods = get_function_variables_definitions(
         function_to_optimize,
         project_root_path,
     )
     tokenizer = tiktoken.encoding_for_model("gpt-3.5-turbo")
     code_to_optimize_tokens = tokenizer.encode(code_to_optimize)
 
     if not function_to_optimize.parents:
@@ -275,8 +295,8 @@
         if context_len + source_len <= max_tokens:
             context_list.append(function_source)
             context_len += source_len
         else:
             break
     logging.debug(f"FINAL OPTIMIZATION CONTEXT TOKENS LENGTH: {context_len}")
     helper_code: str = "\n".join(context_list)
-    return helper_code, helper_functions
+    return helper_code, helper_functions, dunder_methods
```

### Comparing `codeflash-0.6.5/codeflash/optimization/optimizer.py` & `codeflash-0.6.6/codeflash/optimization/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from codeflash.code_utils.code_replacer import replace_function_definitions_in_module
 from codeflash.code_utils.code_utils import (
     get_all_function_names,
     get_run_tmp_file,
     module_name_from_file_path,
 )
 from codeflash.code_utils.config_consts import (
-    INDIVIDUAL_TEST_TIMEOUT,
+    INDIVIDUAL_TESTCASE_TIMEOUT,
     MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS,
     MAX_FUNCTION_TEST_SECONDS,
     MAX_TEST_FUNCTION_RUNS,
     MAX_TEST_RUN_ITERATIONS,
     N_CANDIDATES,
 )
 from codeflash.code_utils.formatter import format_code
@@ -617,14 +617,15 @@
             return Failure("Could not find function to optimize.")
         success, preexisting_functions = get_all_function_names(code_to_optimize)
         if not success:
             return Failure("Error in parsing the code, skipping optimization.")
         (
             helper_code,
             helper_functions,
+            helper_dunder_methods,
         ) = get_constrained_function_context_and_helper_functions(
             function_to_optimize,
             self.args.project_root,
             code_to_optimize,
         )
         if function_to_optimize.parents:
             function_class = function_to_optimize.parents[0].name
@@ -657,14 +658,15 @@
             function_to_optimize.file_path,
             function_to_optimize.file_path,
             project_root,
         )
         preexisting_functions.extend(
             [fn[0].full_name.split(".")[-1] for fn in helper_functions],
         )
+        contextual_dunder_methods.update(helper_dunder_methods)
         return Success(
             CodeOptimizationContext(
                 code_to_optimize_with_helpers=code_to_optimize_with_helpers_and_imports,
                 contextual_dunder_methods=contextual_dunder_methods,
                 helper_functions=helper_functions,
                 preexisting_functions=preexisting_functions,
             ),
@@ -1004,23 +1006,25 @@
                         f"Existing unit tests results for candidate: {candidate_existing_test_results.get_test_pass_fail_report()}",
                     )
                     return_values_are_equal = compare_test_results(
                         original_existing_test_results,
                         candidate_existing_test_results,
                     )
                     for test_invocation in candidate_existing_test_results:
+                        original_test_invocation = original_existing_test_results.get_by_id(
+                            test_invocation.id,
+                        )
                         if (
-                            overall_original_test_results.get_by_id(test_invocation.id) is None
-                            or test_invocation.did_pass
-                            != overall_original_test_results.get_by_id(
-                                test_invocation.id,
-                            ).did_pass
-                            or not return_values_are_equal
-                        ):
-                            logging.info("Test results did not match the test results of the original code.")
+                            original_test_invocation is not None
+                            and not original_test_invocation.timed_out
+                            and (test_invocation.did_pass != original_test_invocation.did_pass)
+                        ) or not return_values_are_equal:
+                            logging.info(
+                                "Test results did not match the test results of the original code.",
+                            )
                             logging.info(
                                 f"Test {test_invocation.id} failed. Skipping this candidate.",
                             )
                             equal_results = False
                             do_break = True
                             break
                     if not equal_results:
@@ -1111,15 +1115,15 @@
         optimization_iteration: int,
         test_function: str | None = None,
     ) -> TestResults:
         result_file_path, run_result = run_tests(
             test_file,
             test_framework=self.args.test_framework,
             cwd=self.args.project_root,
-            pytest_timeout=INDIVIDUAL_TEST_TIMEOUT,
+            pytest_timeout=INDIVIDUAL_TESTCASE_TIMEOUT,
             pytest_cmd=self.test_cfg.pytest_cmd,
             verbose=True,
             test_env=test_env,
             only_run_this_test_function=test_function,
         )
         if run_result.returncode != 0:
             logging.debug(
@@ -1148,15 +1152,15 @@
         tests = generate_tests(
             self.aiservice_client,
             source_code_being_tested=source_code_being_tested,
             function_to_optimize=function_to_optimize,
             helper_function_names=helper_function_names,
             module_path=module_path,
             test_cfg=self.test_cfg,
-            test_timeout=INDIVIDUAL_TEST_TIMEOUT,
+            test_timeout=INDIVIDUAL_TESTCASE_TIMEOUT,
             use_cached_tests=self.args.use_cached_tests,
             function_trace_id=function_trace_id,
         )
         if tests is None:
             logging.error(
                 f"Failed to generate and instrument tests for {function_to_optimize.function_name}",
             )
```

### Comparing `codeflash-0.6.5/codeflash/result/create_pr.py` & `codeflash-0.6.6/codeflash/result/create_pr.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/result/critic.py` & `codeflash-0.6.6/codeflash/result/critic.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/result/explanation.py` & `codeflash-0.6.6/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/telemetry/posthog.py` & `codeflash-0.6.6/codeflash/telemetry/posthog.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         return
 
     global _posthog
     _posthog = Posthog(
         project_api_key="phc_aUO790jHd7z1SXwsYCz8dRApxueplZlZWeDSpKc5hol",
         host="https://us.posthog.com",
     )
+    _posthog.log.setLevel(logging.CRITICAL)  # Suppress PostHog logging
     ph("cli-telemetry-enabled")
 
 
 def ph(event: str, properties: Optional[Dict[str, Any]] = None) -> None:
     """Log an event to PostHog.
     :param event: The name of the event.
     :param properties: A dictionary of properties to attach to the event.
```

### Comparing `codeflash-0.6.5/codeflash/telemetry/sentry.py` & `codeflash-0.6.6/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/tracer.py` & `codeflash-0.6.6/codeflash/tracer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/tracing/profile_stats.py` & `codeflash-0.6.6/codeflash/tracing/profile_stats.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/tracing/replay_test.py` & `codeflash-0.6.6/codeflash/tracing/replay_test.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/update_license_version.py` & `codeflash-0.6.6/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/verification/comparator.py` & `codeflash-0.6.6/codeflash/verification/comparator.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/verification/equivalence.py` & `codeflash-0.6.6/codeflash/verification/equivalence.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,18 +10,27 @@
     if len(original_results) == 0 or len(candidate_results) == 0:
         return False  # empty test results are not equal
     original_recursion_limit = sys.getrecursionlimit()
     if original_recursion_limit < INCREASED_RECURSION_LIMIT:
         sys.setrecursionlimit(INCREASED_RECURSION_LIMIT)  # Increase recursion limit to avoid RecursionError
     test_ids_superset = set(original_results.get_all_ids()).union(set(candidate_results.get_all_ids()))
     are_equal: bool = True
+    did_all_timeout: bool = True
     for test_id in test_ids_superset:
         original_test_result = original_results.get_by_id(test_id)
         cdd_test_results = candidate_results.get_by_id(test_id)
+        if cdd_test_results is not None and original_test_result is None:
+            continue
+
         if original_test_result is None or cdd_test_results is None:
             are_equal = False
             break
+        did_all_timeout = did_all_timeout and original_test_result.timed_out
+        if original_test_result.timed_out:
+            continue
         if not comparator(original_test_result.return_value, cdd_test_results.return_value):
             are_equal = False
             break
     sys.setrecursionlimit(original_recursion_limit)
+    if did_all_timeout:
+        return False
     return are_equal
```

### Comparing `codeflash-0.6.5/codeflash/verification/parse_test_output.py` & `codeflash-0.6.6/codeflash/verification/parse_test_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import pathlib
+import re
 import sqlite3
 import subprocess
 from collections import defaultdict
 from typing import Optional
 
 import dill as pickle
 import sentry_sdk
@@ -64,14 +65,15 @@
                     id=InvocationId.from_str_id(encoded_test_name, invocation_id),
                     file_name=test_file_path,
                     did_pass=True,
                     runtime=duration,
                     test_framework=test_framework,
                     test_type=test_type,
                     return_value=test_pickle,
+                    timed_out=False,
                 ),
             )
             # Hardcoding the test result to True because the test did execute and we are only interested in the return values,
             # the did_pass comes from the xml results file
     return test_results
 
 
@@ -106,14 +108,15 @@
                 ),
                 file_name=test_py_file_path,
                 did_pass=True,
                 runtime=val[5],
                 test_framework=test_config.test_framework,
                 test_type=test_type,
                 return_value=pickle.loads(val[6]),
+                timed_out=False,
             ),
         )
         # return_value is only None temporarily as this is only being used for the existing tests. This should generalize
         # to read the return_value from the sqlite file as well.
         # Hardcoding the test result to True because the test did execute and we are only interested in the return values,
         # the did_pass comes from the xml results file
     return test_results
@@ -175,36 +178,65 @@
                 with sentry_sdk.push_scope() as scope:
                     xml_file_contents = open(test_xml_file_path).read()
                     scope.set_extra("file", xml_file_contents)
                     sentry_sdk.capture_message(
                         f"testcase.name is None in parse_test_xml for testcase {testcase!r} in file {xml_file_contents}",
                     )
                 continue
-            # Parse test timing
-            # system_out_content = ""
-            # for system_out in testcase.system_out:
+            timed_out = False
+            if test_config.test_framework == "pytest":
+                if len(testcase.result) > 1:
+                    print(f"!!!!!Multiple results for {testcase.name} in {test_xml_file_path}!!!")
+                if len(testcase.result) == 1:
+                    message = testcase.result[0].message.lower()
+                    if "failed: timeout >" in message:
+                        timed_out = True
+            matches = re.findall(
+                r"!######(.*?):(.*?)([^\.:]*?):(.*?):(.*?)######!", testcase.system_out or ""
+            )
+            if not matches or not len(matches):
 
-            #     system_out_content += system_out.text
-            test_results.add(
-                FunctionTestInvocation(
-                    id=InvocationId(
-                        test_module_path=test_module_path,
-                        test_class_name=test_class,
-                        test_function_name=test_function,
-                        function_getting_tested="",  # FIXME,
-                        iteration_id=None,
+                test_results.add(
+                    FunctionTestInvocation(
+                        id=InvocationId(
+                            test_module_path=test_module_path,
+                            test_class_name=test_class,
+                            test_function_name=test_function,
+                            function_getting_tested="",  # FIXME,
+                            iteration_id=None,
+                        ),
+                        file_name=file_name,
+                        runtime=None,
+                        test_framework=test_config.test_framework,
+                        did_pass=result,
+                        test_type=test_type,
+                        return_value=None,
+                        timed_out=timed_out,
                     ),
-                    file_name=file_name,
-                    runtime=None,
-                    test_framework=test_config.test_framework,
-                    did_pass=result,
-                    test_type=test_type,
-                    return_value=None,
-                ),
-            )
+                )
+            else:
+                for match in matches:
+                    test_results.add(
+                        FunctionTestInvocation(
+                            id=InvocationId(
+                                test_module_path=match[0],
+                                test_class_name=None if match[1] == "" else match[1],
+                                test_function_name=match[2],
+                                function_getting_tested=match[3],
+                                iteration_id=match[4],
+                            ),
+                            file_name=file_name,
+                            runtime=None,
+                            test_framework=test_config.test_framework,
+                            did_pass=result,
+                            test_type=test_type,
+                            return_value=None,
+                            timed_out=timed_out,
+                        ),
+                    )
     if len(test_results) == 0:
         logging.info(f"Test '{test_py_file_path}' failed to run, skipping it")
         if run_result is not None:
             logging.info(
                 f"Test log - STDOUT : {run_result.stdout.decode()} \n STDERR : {run_result.stderr.decode()}",
             )
     return test_results
@@ -254,48 +286,75 @@
         if not bin_results:
             merged_test_results.merge(xml_results)
             continue
 
         if len(xml_results) == 1:
             xml_result = xml_results[0]
             # This means that we only have one FunctionTestInvocation for this test xml. Match them to the bin results
+            # Either a whole test function fails or passes.
             for result_bin in bin_results:
                 merged_test_results.add(
                     FunctionTestInvocation(
                         id=result_bin.id,
                         file_name=xml_result.file_name,
                         runtime=result_bin.runtime,
                         test_framework=xml_result.test_framework,
                         did_pass=xml_result.did_pass,
                         test_type=xml_result.test_type,
                         return_value=result_bin.return_value,
+                        timed_out=xml_result.timed_out,
+                    ),
+                )
+        elif xml_results.test_results[0].id.iteration_id is not None:
+            # This means that we have multiple iterations of the same test function
+            # We need to match the iteration_id to the bin results
+            for i in range(len(xml_results.test_results)):
+                xml_result = xml_results.test_results[i]
+                try:
+                    bin_result = bin_results.get_by_id(xml_result.id)
+                except AttributeError:
+                    bin_result = None
+                if bin_result is None:
+                    merged_test_results.add(xml_result)
+                    continue
+                merged_test_results.add(
+                    FunctionTestInvocation(
+                        id=xml_result.id,
+                        file_name=xml_result.file_name,
+                        runtime=bin_result.runtime,
+                        test_framework=xml_result.test_framework,
+                        did_pass=bin_result.did_pass,
+                        test_type=xml_result.test_type,
+                        return_value=bin_result.return_value,
+                        timed_out=xml_result.timed_out
+                        if bin_result.runtime is None
+                        else False,  # If runtime was measured in the bin file, then the testcase did not time out
                     ),
                 )
         else:
+            # Should happen only if the xml did not have any test invocation id info
             for i in range(len(bin_results.test_results)):
                 bin_result = bin_results.test_results[i]
                 try:
                     xml_result = xml_results.test_results[i]
                 except IndexError:
                     xml_result = None
                 if xml_result is None:
-                    # if xml_result.test_type == TestType.EXISTING_UNIT_TEST:
-                    # only support
-                    # logging.warning(f"Could not find xml result for bin result: {bin_result.id}")
                     merged_test_results.add(bin_result)
                     continue
                 merged_test_results.add(
                     FunctionTestInvocation(
                         id=bin_result.id,
                         file_name=bin_result.file_name,
                         runtime=bin_result.runtime,
                         test_framework=bin_result.test_framework,
                         did_pass=bin_result.did_pass,
                         test_type=bin_result.test_type,
                         return_value=bin_result.return_value,
+                        timed_out=xml_result.timed_out,  # only the xml gets the timed_out flag
                     ),
                 )
 
     return merged_test_results
 
 
 def parse_test_results(
```

### Comparing `codeflash-0.6.5/codeflash/verification/test_results.py` & `codeflash-0.6.6/codeflash/verification/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     test_class_name: Optional[str]  # The name of the class where the test is defined
     test_function_name: str  # The name of the test_function. Does not include the components of the file_name
     function_getting_tested: str
     iteration_id: Optional[str]
 
     # test_module_path:TestSuiteClass.test_function_name:function_tested:iteration_id
     def id(self):
-        return f"{self.test_module_path}:{self.test_class_name or ''}.{self.test_function_name}:{self.function_getting_tested}:{self.iteration_id}"
+        return f"{self.test_module_path}:{(self.test_class_name + '.' if self.test_class_name else '')}{self.test_function_name}:{self.function_getting_tested}:{self.iteration_id}"
 
     @staticmethod
     def from_str_id(string_id: str, iteration_id: Optional[str] = None) -> InvocationId:
         components = string_id.split(":")
         assert len(components) == 4
         second_components = components[1].split(".")
         if len(second_components) == 1:
@@ -64,14 +64,15 @@
     id: InvocationId  # The fully qualified name of the function invocation (id)
     file_name: str  # The file where the test is defined
     did_pass: bool  # Whether the test this function invocation was part of, passed or failed
     runtime: Optional[int]  # Time in nanoseconds
     test_framework: str  # unittest or pytest
     test_type: TestType
     return_value: Optional[object]  # The return value of the function invocation
+    timed_out: Optional[bool]
 
 
 class TestResults(BaseModel):
     test_results: list[FunctionTestInvocation] = []
 
     def add(self, function_test_invocation: FunctionTestInvocation) -> None:
         self.test_results.append(function_test_invocation)
```

### Comparing `codeflash-0.6.5/codeflash/verification/test_runner.py` & `codeflash-0.6.6/codeflash/verification/test_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,25 @@
     assert test_framework in ["pytest", "unittest"]
     if only_run_this_test_function and "__replay_test" in test_path:
         test_path = test_path + "::" + only_run_this_test_function
 
     if test_framework == "pytest":
         result_file_path = get_run_tmp_file("pytest_results.xml")
         pytest_cmd_list = [chunk for chunk in pytest_cmd.split(" ") if chunk != ""]
+
         results = subprocess.run(
             pytest_cmd_list
             + [
                 test_path,
-                "-q",
+                "--capture=tee-sys",
                 f"--timeout={pytest_timeout}",
+                "-q",
                 f"--junitxml={result_file_path}",
+                "-o",
+                "junit_logging=all",
             ],
             capture_output=True,
             cwd=cwd,
             env=test_env,
             text=True,
             timeout=600,
         )
```

### Comparing `codeflash-0.6.5/codeflash/verification/verification_utils.py` & `codeflash-0.6.6/codeflash/verification/verification_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/codeflash/verification/verifier.py` & `codeflash-0.6.6/codeflash/verification/verifier.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.6.5/pyproject.toml` & `codeflash-0.6.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.6.5" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.6.6" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
 ]
 keywords = ["codeflash", "performance", "optimization", "ai", "code", "machine learning", "LLM"]
 
+# Don't forget to install the poetry plugins we use too:
+# poetry self add poetry-dynamic-versioning
+
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 unidiff = ">=0.7.4"
 pytest = ">=7.0.0"
 gitpython = ">=3.1.31"
 libcst = ">=1.0.1"
 jedi = ">=0.19.1"
@@ -122,9 +125,9 @@
 module-root = "codeflash"
 tests-root = "tests"
 test-framework = "pytest"
 ignore-paths = []
 
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.2.0,<2.0.0"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `codeflash-0.6.5/PKG-INFO` & `codeflash-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.6.5
+Version: 0.6.6
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
```

