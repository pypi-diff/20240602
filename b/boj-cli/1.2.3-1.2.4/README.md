# Comparing `tmp/boj-cli-1.2.3.tar.gz` & `tmp/boj-cli-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boj-cli-1.2.3.tar", last modified: Sat Jun  1 08:17:37 2024, max compression
+gzip compressed data, was "boj-cli-1.2.4.tar", last modified: Sun Jun  2 12:07:08 2024, max compression
```

## Comparing `boj-cli-1.2.3.tar` & `boj-cli-1.2.4.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/major-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/minor-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/patch-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/release-template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/workflows/run-test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/boj-cli.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/.idea/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/dictionaries/jerry.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/material_theme_project_new.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-06-01 08:17:18.000000 boj-cli-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-06-01 08:17:37.555514 boj-cli-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-06-01 08:17:18.000000 boj-cli-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/args_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/browsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/browsers/login_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/add/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/add/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/case/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/case/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/clean/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/clean/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/init/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/init/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/login/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/login/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/open/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/open/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/random/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/random/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/run/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/run/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/submit/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/progress_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.551514 boj-cli-1.2.3/boj/core/fs/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/file_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/file_search_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.551514 boj-cli-1.2.3/boj/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/boj_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.551514 boj-cli-1.2.3/boj/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_main_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_problem_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_status_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_submit_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/solved_ac_search_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/boj_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-01 08:17:18.000000 boj-cli-1.2.3/config_example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-06-01 08:17:18.000000 boj-cli-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-01 08:17:18.000000 boj-cli-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 08:17:37.555514 boj-cli-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-01 08:17:18.000000 boj-cli-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/assets/config/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/config/test_filetype_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/config/test_filetype_no_lang_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/config/test_filetype_no_run_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/tests/assets/problems/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/assets/problems/3052/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/.boj-info.json
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/compile_flags.txt
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/testcase.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/core/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/core/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/test_args_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/web/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/web/test_solved_ac_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-01 08:17:18.000000 boj-cli-1.2.3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.905835 boj-cli-1.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.889835 boj-cli-1.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.github/major-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.github/minor-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.github/patch-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.github/release-template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.889835 boj-cli-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.github/workflows/run-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.889835 boj-cli-1.2.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/boj-cli.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.889835 boj-cli-1.2.4/.idea/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/dictionaries/jerry.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.889835 boj-cli-1.2.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/material_theme_project_new.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-02 12:06:47.000000 boj-cli-1.2.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-06-02 12:06:47.000000 boj-cli-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-06-02 12:07:08.905835 boj-cli-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-06-02 12:06:47.000000 boj-cli-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/args_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/browsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/browsers/login_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/add/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/add/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/case/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/case/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/clean/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/clean/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/init/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/login/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/login/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/open/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/open/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.893834 boj-cli-1.2.4/boj/commands/random/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/random/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.897835 boj-cli-1.2.4/boj/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/run/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.897835 boj-cli-1.2.4/boj/commands/submit/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/submit/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/submit/progress_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/commands/submit/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.897835 boj-cli-1.2.4/boj/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.901835 boj-cli-1.2.4/boj/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/file_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/file_search_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/fs/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/core/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.901835 boj-cli-1.2.4/boj/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/data/boj_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/data/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/data/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/data/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.901835 boj-cli-1.2.4/boj/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/web/boj_main_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/web/boj_problem_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/web/boj_status_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/web/boj_submit_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-02 12:06:47.000000 boj-cli-1.2.4/boj/web/solved_ac_search_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.901835 boj-cli-1.2.4/boj_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-06-02 12:07:08.000000 boj-cli-1.2.4/boj_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-06-02 12:07:08.000000 boj-cli-1.2.4/boj_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:07:08.000000 boj-cli-1.2.4/boj_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:07:08.000000 boj-cli-1.2.4/boj_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-02 12:07:08.000000 boj-cli-1.2.4/boj_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-02 12:07:08.000000 boj-cli-1.2.4/boj_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-02 12:06:47.000000 boj-cli-1.2.4/config_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-06-02 12:06:47.000000 boj-cli-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-02 12:06:47.000000 boj-cli-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 12:07:08.905835 boj-cli-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-02 12:06:47.000000 boj-cli-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.905835 boj-cli-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.885835 boj-cli-1.2.4/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.905835 boj-cli-1.2.4/tests/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/config/test_filetype_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/config/test_filetype_no_lang_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/config/test_filetype_no_run_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.885835 boj-cli-1.2.4/tests/assets/problems/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.905835 boj-cli-1.2.4/tests/assets/problems/3052/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/problems/3052/.boj-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/problems/3052/compile_flags.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/problems/3052/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/assets/problems/3052/testcase.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.905835 boj-cli-1.2.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/core/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/core/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/test_args_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:07:08.905835 boj-cli-1.2.4/tests/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-06-02 12:06:47.000000 boj-cli-1.2.4/tests/web/test_solved_ac_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-02 12:06:47.000000 boj-cli-1.2.4/version.py
```

### Comparing `boj-cli-1.2.3/.github/release-template.yaml` & `boj-cli-1.2.4/.github/release-template.yaml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/.github/workflows/release.yaml` & `boj-cli-1.2.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/.gitignore` & `boj-cli-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/.idea/boj-cli.iml` & `boj-cli-1.2.4/.idea/boj-cli.iml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/LICENSE` & `boj-cli-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/PKG-INFO` & `boj-cli-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boj-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: Command line interface for BOJ
 Author: xvzc
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # boj-cli
```

### Comparing `boj-cli-1.2.3/README.md` & `boj-cli-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/args_resolver.py` & `boj-cli-1.2.4/boj/args_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,17 +182,17 @@
         default=False,
         help="open a new testcase"
     )
     case_parser.add_argument(
         "-e",
         "--edit",
         dest="edit",
-        metavar="FILETYPE",
+        metavar="CASE_ID",
         default=None,
-        help="open a testcase with the editor command",
+        help="edit the testcase of given id with editor command",
     )
 
 
 def get_version():
     return f"boj-cli {boj.__version__}"
```

### Comparing `boj-cli-1.2.3/boj/browsers/login_browser.py` & `boj-cli-1.2.4/boj/browsers/login_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
                     self.driver.find_element(By.NAME, "login_user_id").click()
                     continue
             except StaleElementReferenceException:
                 continue
             except NoSuchElementException:
                 break
             except Exception:
-                raise IllegalStatementError("Failed to login to BOJ")
+                raise FatalError("failed to login to BOJ")
 
         wait = WebDriverWait(self.driver, 10)
         element = wait.until(EC.element_to_be_clickable((By.CLASS_NAME, "username")))
         token = self.driver.get_cookie("bojautologin")
         if "value" not in token:
-            raise AuthenticationError("Failed to read session token")
+            raise FatalError("failed to read session token")
 
         return {"username": element.text, "token": token["value"]}
```

### Comparing `boj-cli-1.2.3/boj/commands/add/command.py` & `boj-cli-1.2.4/boj/commands/add/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 id_=args.problem_id,
                 title=problem_title,
                 config=config.filetype(filetype),
                 dir_=config.workspace.problem_dir(args.problem_id),
             )
 
             if not args.force and file_exists(boj_info.metadata.path):
-                raise IllegalStatementError(f"Problem {args.problem_id} already exists")
+                raise FatalError(f"problem {args.problem_id} already exists")
 
             # Create testcases
             # os.makedirs(boj_info.source_dir, exist_ok=True)
             testcases = self.testcase_parser.find(problem_page.html)
             for testcase in testcases:
                 input_, output = testcase.to_text_files(boj_info.testcase_dir(True))
                 self.text_file_repository.save(input_)
```

### Comparing `boj-cli-1.2.3/boj/commands/case/command.py` & `boj-cli-1.2.4/boj/commands/case/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                 cwd=tc_dir, query=os.path.join(args.edit, "input.txt")
             )
             output = self.text_file_repository.find(
                 cwd=tc_dir, query=os.path.join(args.edit, "output.txt")
             )
             _open_files(config.general.editor_command, input_, output)
         else:
-            raise IllegalStatementError("operation is not specified")
+            raise FatalError("operation is not specified: --new || -edit $id")
```

### Comparing `boj-cli-1.2.3/boj/commands/clean/command.py` & `boj-cli-1.2.4/boj/commands/clean/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/commands/init/command.py` & `boj-cli-1.2.4/boj/commands/init/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/commands/login/command.py` & `boj-cli-1.2.4/boj/commands/login/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,9 @@
                 username=credential_dict["username"],
                 token=credential_dict["token"],
             )
 
             status.update("Writing to file...")
             self.credential_repository.save(credential)
 
-        self.console.print("[green]Login succeeded")
+        self.console.print("[green]Successfully logged in")
+
```

### Comparing `boj-cli-1.2.3/boj/commands/open/command.py` & `boj-cli-1.2.4/boj/commands/open/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/commands/random/command.py` & `boj-cli-1.2.4/boj/commands/random/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/commands/run/command.py` & `boj-cli-1.2.4/boj/commands/run/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/commands/run/runner.py` & `boj-cli-1.2.4/boj/commands/run/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from subprocess import Popen, PIPE
 
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 from boj.data.boj_info import BojInfo
 from boj.data.testcase import Testcase
 from boj.data.config import FiletypeConfig
-from boj.core.error import RunCodeError
+from boj.core.error import RunCodeError, FatalError
 from rich.console import Console
 
 
 def create_case_label(width, label: str):
     label = label.ljust(width + 1, " ")
     return f"[cyan]CASE #{label}"
 
@@ -70,15 +70,15 @@
             if output:
                 self.__console.log(output)
 
             if error:
                 self.__console.log(error)
 
             if process.returncode != 0:
-                raise RunCodeError("Compile error")
+                raise FatalError("compile error")
 
         except Exception as e:
             raise e
 
     def run_testcases(self):
         progress = Progress(
             SpinnerColumn(style="white", finished_text="•"),
@@ -215,11 +215,11 @@
             if output:
                 self.__console.log(output)
 
             if error:
                 self.__console.log(error)
 
             if process.returncode != 0:
-                raise RunCodeError("Error while running 'after' command")
+                raise FatalError("error while running 'after' command")
 
         except Exception as e:
             raise e
```

### Comparing `boj-cli-1.2.3/boj/commands/submit/command.py` & `boj-cli-1.2.4/boj/commands/submit/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/commands/submit/progress_message.py` & `boj-cli-1.2.4/boj/commands/submit/progress_message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import json
 
-from boj.core.error import WebSocketError
+from boj.core.error import WebSocketError, FatalError
 
 
 class Detail:
     def __init__(self, name, description):
         self.name = name
         self.description = description
 
 
 class ProgressMessage:
     def __init__(
-        self,
-        keep_alive: bool,
-        status: str,
-        progress: int,
-        color: str,
-        error: bool,
-        details: list[Detail],
+            self,
+            keep_alive: bool,
+            status: str,
+            progress: int,
+            color: str,
+            error: bool,
+            details: list[Detail],
     ):
         self.keep_alive = keep_alive
         self.status = status
         self.progress = progress
         self.error = error
         self.color = color
         self.details = details
 
     def __repr__(self):
         return (
-            "Problem {"
-            + str(self.keep_alive)
-            + ", "
-            + self.color
-            + ", "
-            + self.status
-            + "}"
+                "Problem {"
+                + str(self.keep_alive)
+                + ", "
+                + self.color
+                + ", "
+                + self.status
+                + "}"
         )
 
     @staticmethod
     def unknown_error(progress, e: Exception):
         return ProgressMessage(
             keep_alive=False,
             error=True,
@@ -62,15 +62,15 @@
     @staticmethod
     def subscription_succeeded():
         return ProgressMessage(
             keep_alive=True,
             error=False,
             progress=0,
             color="white",
-            status="Subscription Succeeded",
+            status="Subscription started",
             details=[],
         )
 
     @staticmethod
     def waiting(progress: int):
         return ProgressMessage(
             keep_alive=True,
@@ -207,18 +207,18 @@
         if message["event"] == "pusher:connection_established":
             return cls.connection_established()
 
         if message["event"] == "pusher_internal:subscription_succeeded":
             return cls.subscription_succeeded()
 
         if message["event"] == "pusher:error":
-            raise WebSocketError("Websocket error")
+            raise FatalError("websocket error")
 
         if message["event"] != "update":
-            raise WebSocketError("Unknown websocket event")
+            raise FatalError("unknown websocket event")
 
         data = json.loads(message["data"])
         progress = data["progress"] if "progress" in data else 0
 
         if data["result"] <= 2:
             return cls.waiting(progress)
 
@@ -272,8 +272,8 @@
 
             return cls.partial_points(progress, details)
 
         # Runtime error investigation
         if data["result"] == 16:
             return cls.runtime_error_waiting(progress)
 
-        raise WebSocketError("Unknown websocket status")
+        raise FatalError(f"unknown websocket status {data['result']}")
```

### Comparing `boj-cli-1.2.3/boj/commands/submit/websocket.py` & `boj-cli-1.2.4/boj/commands/submit/websocket.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/containers.py` & `boj-cli-1.2.4/boj/containers.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/browser.py` & `boj-cli-1.2.4/boj/core/browser.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             service=Service(ChromeDriverManager(cache_manager=cache_manager).install()),
         )
     elif browser == "edge":
         return webdriver.Edge(
             service=Service(ChromeDriverManager(cache_manager=cache_manager).install()),
         )
     else:
-        raise IllegalStatementError(f"{browser} is not a valid browser")
+        raise FatalError(f"{browser} is not a valid browser")
 
 
 class Browser:
     driver: WebDriver
     url: str
 
     def __init__(self, url: str, browser: str):
```

### Comparing `boj-cli-1.2.3/boj/core/console.py` & `boj-cli-1.2.4/boj/core/console.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/constant.py` & `boj-cli-1.2.4/boj/core/constant.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/error.py` & `boj-cli-1.2.4/boj/core/error.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/fs/file_io.py` & `boj-cli-1.2.4/boj/core/fs/file_io.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/fs/file_object.py` & `boj-cli-1.2.4/boj/core/fs/file_object.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/fs/file_search_strategy.py` & `boj-cli-1.2.4/boj/core/fs/file_search_strategy.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/fs/repository.py` & `boj-cli-1.2.4/boj/core/fs/repository.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/fs/serializer.py` & `boj-cli-1.2.4/boj/core/fs/serializer.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/core/http.py` & `boj-cli-1.2.4/boj/core/http.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/data/boj_info.py` & `boj-cli-1.2.4/boj/data/boj_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from boj.core.fs.file_object import FileMetadata, FileObject
 from boj.data.config import FiletypeConfig
 
 
 def _convert_language_code(lang):
     lang_dict = constant.lang_dict()
     if lang not in lang_dict:
-        raise IllegalStatementError(lang + " is not a supported language")
+        raise FatalError(f"{lang} is not a supported language")
 
     return lang_dict[lang]
 
 
 class BojInfo(FileObject):
     def __init__(
         self,
```

### Comparing `boj-cli-1.2.3/boj/data/config.py` & `boj-cli-1.2.4/boj/data/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,25 +134,25 @@
                 run=v.get("run", None),
                 after=v.get("after", None),
                 source_templates=v.get("source_templates", []),
                 root_templates=v.get("root_templates", []),
             )
 
             if not config.language:
-                raise ParsingConfigError(
+                raise FatalError(
                     f"missing 'language' option for the filetype {ft}"
                 )
 
             if not config.main:
-                raise ParsingConfigError(
+                raise FatalError(
                     f"missing 'filename' option for the filetype {ft}"
                 )
 
             if not config.run:
-                raise ParsingConfigError(f"missing 'run' option for the filetype {ft}")
+                raise FatalError(f"missing 'run' option for the filetype {ft}")
 
             filetype_config[ft] = config
 
         return filetype_config
 
 
 class WorkspaceConfig:
@@ -206,15 +206,15 @@
             workspace_root=workspace_root,
             ongoing_dir=workspace.get("ongoing_dir", ""),
             archive_dir=workspace.get("archive_dir", "archives"),
             template_dir="templates",
         )
 
         if workspace_config.ongoing_dir(True) == workspace_config.archive_dir(True):
-            raise ParsingConfigError(
+            raise FatalError(
                 "'workspace.ongoing_dir' and 'workspace.archive_dir' can not be the same"
             )
 
         return workspace_config
 
 
 class Config(FileObject):
@@ -247,26 +247,26 @@
 
     @property
     def workspace(self) -> WorkspaceConfig:
         return self.__workspace
 
     def filetype(self, ft) -> FiletypeConfig:
         if ft not in self.__filetype:
-            raise ParsingConfigError(
+            raise FatalError(
                 f"filetype config for '{ft}' is not defined in 'config.yaml'"
             )
 
         filetype_config = self.__filetype[ft]
         if not filetype_config.language:
-            raise ParsingConfigError(
+            raise FatalError(
                 f"'language' option for filetype '{ft}' is not found."
             )
 
         if not filetype_config.run:
-            raise ParsingConfigError(f"'run' option for filetype '{ft}' is not found.")
+            raise FatalError(f"'run' option for filetype '{ft}' is not found.")
 
         return filetype_config
 
 
 class ConfigFileSerializer(Serializer):
     def marshal(self, raw: bytes, metadata: FileMetadata) -> Config:
         data = yaml.safe_load(raw.decode("utf-8")) or {}
@@ -283,15 +283,15 @@
             workspace_root=workspace_root,
             general=general_config,
             workspace=workspace_config,
             filetype_config=filetype_config,
         )
 
     def unmarshal(self, obj: Config) -> bytes:
-        raise IllegalStatementError("Config file object should not be unmarshalled")
+        raise FatalError("config file object should not be unmarshalled")
 
 
 class ConfigRepository(ReadOnlyRepository[Config]):
     def find(
         self,
         cwd: str = os.getcwd(),
         query: Optional[str] = None,
```

### Comparing `boj-cli-1.2.3/boj/data/credential.py` & `boj-cli-1.2.4/boj/data/credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from typing import Optional
 
 from boj.core import crypto
-from boj.core.error import ResourceNotFoundError, AuthenticationError
+from boj.core.error import ResourceNotFoundError, AuthenticationError, FatalError
 
 from boj.core.fs.file_object import FileObject, FileMetadata
 from boj.core.fs.repository import Repository, T
 from boj.core.fs.serializer import Serializer
 
 
 class Credential(FileObject):
@@ -60,16 +60,16 @@
             cipher_text = self._file_io.read(credential_path)
             plain_text = crypto.decrypt(key, cipher_text)
             return self._serializer.marshal(
                 raw=plain_text,
                 metadata=FileMetadata.of(credential_path),
             )
         except ResourceNotFoundError:
-            raise AuthenticationError(
-                "Failed to load credential. Did you run 'boj login'?"
+            raise FatalError(
+                "failed to load credential. Did you run 'boj login'?"
             )
 
     def save(self, obj: Credential) -> None:
         plain = self._serializer.unmarshal(obj=obj)
         key = crypto.create_key()
         cipher = crypto.encrypt(key, plain)
         self._file_io.write(cipher, obj.metadata.path)
```

### Comparing `boj-cli-1.2.3/boj/data/session.py` & `boj-cli-1.2.4/boj/data/session.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/data/testcase.py` & `boj-cli-1.2.4/boj/data/testcase.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/entry.py` & `boj-cli-1.2.4/boj/entry.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/web/boj_problem_page.py` & `boj-cli-1.2.4/boj/web/boj_problem_page.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj/web/boj_submit_page.py` & `boj-cli-1.2.4/boj/web/boj_submit_page.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,17 +70,17 @@
         # Parse the submit page
         soup = BeautifulSoup(html, "html.parser")
 
         # Check login status
         input_tags = soup.select("input")
         for tag in input_tags:
             if tag["name"] == "login_user_id":
-                raise AuthenticationError(
-                    "Authentication failed. Did you run 'boj login'?"
+                raise FatalError(
+                    "authentication failed. did you run 'boj login'?"
                 )
 
         # Get the csrf_key
         for tag in input_tags:
             if tag["name"] == "csrf_key":
                 return tag["value"]
 
-        raise AuthenticationError("Failed to query csrf token.")
+        raise FatalError("failed to query csrf token.")
```

### Comparing `boj-cli-1.2.3/boj/web/solved_ac_search_api.py` & `boj-cli-1.2.4/boj/web/solved_ac_search_api.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/boj_cli.egg-info/PKG-INFO` & `boj-cli-1.2.4/boj_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boj-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: Command line interface for BOJ
 Author: xvzc
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # boj-cli
```

### Comparing `boj-cli-1.2.3/boj_cli.egg-info/SOURCES.txt` & `boj-cli-1.2.4/boj_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .github/patch-release.yaml
 .github/release-template.yaml
 .github/workflows/release.yaml
 .github/workflows/run-test.yaml
 .idea/.gitignore
 .idea/boj-cli.iml
 .idea/material_theme_project_new.xml
+.idea/misc.xml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/dictionaries/jerry.xml
 .idea/inspectionProfiles/profiles_settings.xml
 boj/__init__.py
 boj/__main__.py
 boj/args_resolver.py
```

### Comparing `boj-cli-1.2.3/config_example.yaml` & `boj-cli-1.2.4/config_example.yaml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/pyproject.toml` & `boj-cli-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/requirements.txt` & `boj-cli-1.2.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/tests/assets/problems/3052/main.cpp` & `boj-cli-1.2.4/tests/assets/problems/3052/main.cpp`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/tests/core/test_constant.py` & `boj-cli-1.2.4/tests/core/test_constant.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/tests/test_args_resolver.py` & `boj-cli-1.2.4/tests/test_args_resolver.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/tests/web/test_solved_ac_search_api.py` & `boj-cli-1.2.4/tests/web/test_solved_ac_search_api.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.3/version.py` & `boj-cli-1.2.4/version.py`

 * *Files identical despite different names*

