# Comparing `tmp/cmake_pre_commit_hooks-1.9.5.tar.gz` & `tmp/cmake_pre_commit_hooks-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_pre_commit_hooks-1.9.5.tar", last modified: Fri Dec 15 12:46:32 2023, max compression
+gzip compressed data, was "cmake_pre_commit_hooks-1.9.6.tar", last modified: Sun Jun  2 10:32:56 2024, max compression
```

## Comparing `cmake_pre_commit_hooks-1.9.5.tar` & `cmake_pre_commit_hooks-1.9.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.880475 cmake_pre_commit_hooks-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.codespell.allow
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.872475 cmake_pre_commit_hooks-1.9.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.872475 cmake_pre_commit_hooks-1.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/workflows/draft_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17477 2023-12-15 12:46:32.880475 cmake_pre_commit_hooks-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15834 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.876475 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_call_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_cmake.py
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/clang_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/clang_tidy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/include_what_you_use.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1917 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/lizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.880475 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17477 2023-12-15 12:46:32.000000 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2023-12-15 12:46:32.000000 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 12:46:32.000000 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-15 12:46:32.000000 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-12-15 12:46:32.000000 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-15 12:46:32.000000 cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.876475 cmake_pre_commit_hooks-1.9.5/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/misc/license_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 12:46:32.880475 cmake_pre_commit_hooks-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.876475 cmake_pre_commit_hooks-1.9.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.876475 cmake_pre_commit_hooks-1.9.5/tests/cmake_bad/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_bad/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_bad/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_bad/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_bad/bad.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.880475 cmake_pre_commit_hooks-1.9.5/tests/cmake_good/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_good/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_good/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_good/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/cmake_good/good.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 12:46:32.880475 cmake_pre_commit_hooks-1.9.5/tests/python/
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/_argparse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/_call_process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19474 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/_cmake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/clang_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/clang_tidy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/cppcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/cpplint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/iwyu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/python/lizard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/run_tests.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)     3709 2023-12-15 12:46:24.000000 cmake_pre_commit_hooks-1.9.5/tests/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.126432 cmake_pre_commit_hooks-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.codespell.allow
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.118432 cmake_pre_commit_hooks-1.9.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.118432 cmake_pre_commit_hooks-1.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/workflows/draft_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-06-02 10:32:56.126432 cmake_pre_commit_hooks-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.118432 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_call_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19551 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_cmake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/clang_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/clang_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/include_what_you_use.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1917 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/lizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.122432 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-06-02 10:32:56.000000 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-06-02 10:32:56.000000 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:32:56.000000 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-02 10:32:56.000000 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-02 10:32:56.000000 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 10:32:56.000000 cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.122432 cmake_pre_commit_hooks-1.9.6/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/misc/license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:32:56.126432 cmake_pre_commit_hooks-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.122432 cmake_pre_commit_hooks-1.9.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.122432 cmake_pre_commit_hooks-1.9.6/tests/cmake_bad/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_bad/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_bad/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_bad/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_bad/bad.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.122432 cmake_pre_commit_hooks-1.9.6/tests/cmake_good/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_good/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_good/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_good/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/cmake_good/good.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:32:56.122432 cmake_pre_commit_hooks-1.9.6/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/_argparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/_call_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19508 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/_cmake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/clang_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/clang_tidy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/cppcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/cpplint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/iwyu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/python/lizard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/run_tests.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3709 2024-06-02 10:32:42.000000 cmake_pre_commit_hooks-1.9.6/tests/run_tests.sh
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.github/workflows/ci.yml` & `cmake_pre_commit_hooks-1.9.6/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,31 +18,39 @@
         runs-on: [ubuntu-latest, windows-latest, macos-latest]
         python:
           - 3.8
           - 3.9
           - '3.10'
           - '3.11'
           - '3.12'
+        exclude:
+          # macos-latest is now running on M1 macs
+          - runs-on: macos-latest
+            python: 3.8
+          - runs-on: macos-latest
+            python: 3.9
+          - runs-on: macos-latest
+            python: 3.10
 
     name: "Unit tests • ${{ matrix.python }} • ${{ matrix.runs-on }} • x64 ${{ matrix.args }}"
     runs-on: ${{ matrix.runs-on }}
     if: >-
       (github.event_name != 'pull_request'
         || (github.event_name == 'pull_request' && github.event.pull_request.merged != true))
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
 
       - name: Setup Python ${{ matrix.python }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
           architecture: 'x64'
           cache: 'pip'
           cache-dependency-path: '**/pyproject.toml'
 
       - name: Prepare env
@@ -51,15 +59,15 @@
       - name: Build and install package
         run: python -m pip install -e .[test]
 
       - name: Run Python tests
         run: python -m pytest -v --cov=cmake_pc_hooks --cov-report=xml --cov-report=term-missing --cov-branch
 
       - name: Upload coverage reports to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
 
       - name: Save coverage report
         if: matrix.python == '3.11' && runner.os == 'Linux'
         uses: actions/upload-artifact@v3
         with:
@@ -73,36 +81,45 @@
       matrix:
         runs-on: [ubuntu-latest, windows-latest, macos-latest]
         python:
           - 3.8
           - 3.9
           - '3.10'
           - '3.11'
+          - '3.12'
+        exclude:
+          # macos-latest is now running on M1 macs
+          - runs-on: macos-latest
+            python: 3.8
+          - runs-on: macos-latest
+            python: 3.9
+          - runs-on: macos-latest
+            python: 3.10
 
     name: "System tests ${{ matrix.python }} • ${{ matrix.runs-on }} • x64 ${{ matrix.args }}"
     runs-on: ${{ matrix.runs-on }}
     needs: unit-tests
     if: >-
       (github.event_name != 'pull_request'
         || (github.event_name == 'pull_request' && github.event.pull_request.merged != true))
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
 
       - name: Enable Developer Command Prompt
         if: runner.os == 'Windows'
-        uses: ilammy/msvc-dev-cmd@v1.12.1
+        uses: ilammy/msvc-dev-cmd@v1.13.0
 
       - name: Setup Python ${{ matrix.python }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
           architecture: 'x64'
           cache: 'pip'
           cache-dependency-path: '**/pyproject.toml'
 
       - name: Prepare env
@@ -166,15 +183,15 @@
         run: ./tests/run_tests.ps1
 
   sonarcloud:
     name: SonarCloud
     runs-on: ubuntu-latest
     needs: unit-tests
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Fetch coverage report
         uses: actions/download-artifact@v3
         with:
           name: coverage
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.github/workflows/codeql-analysis.yml` & `cmake_pre_commit_hooks-1.9.6/.github/workflows/codeql-analysis.yml`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,24 @@
     strategy:
       fail-fast: false
       matrix:
         language: ['python']
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@v2
+        uses: github/codeql-action/init@v3
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
           # queries: ./path/to/local/query, your-org/your-repo/queries@main
 
       - name: Autobuild
-        uses: github/codeql-action/autobuild@v2
+        uses: github/codeql-action/autobuild@v3
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@v2
+        uses: github/codeql-action/analyze@v3
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.github/workflows/draft_release.yml` & `cmake_pre_commit_hooks-1.9.6/.github/workflows/draft_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         required: true
 
 jobs:
   new-release:
     name: "Draft a new release"
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: '3.11'
           cache: 'pip'
           cache-dependency-path: '**/pyproject.toml'
 
       - name: Update CHANGELOG
         run: |
@@ -37,15 +37,15 @@
           create_branch: true
           file_pattern: 'CHANGELOG.md'
           commit_message: Preparing release ${{ github.event.inputs.tag }}
           commit_author: github-actions[bot] <noreply@github.com>
 
       # yamllint disable rule:line-length
       - name: Create pull request
-        uses: thomaseizinger/create-pull-request@1.3.1
+        uses: thomaseizinger/create-pull-request@1.4.0
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           head: release/${{ github.event.inputs.tag }}
           base: main
           title: Release version ${{ github.event.inputs.tag }}
           reviewers: ${{ github.actor }}
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.github/workflows/format.yml` & `cmake_pre_commit_hooks-1.9.6/.github/workflows/format.yml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     name: Parse CHANGELOG
     runs-on: ubuntu-latest
     if: >-
       github.event_name == 'pull_request'
       && (startsWith(github.event.pull_request.head.ref, 'release/')
           || startsWith(github.event.pull_request.head.ref, 'hotfix/'))
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Installing parse-changelog
         env:
           target: x86_64-unknown-linux-musl
           parse_changelog_tag: v0.5.4
           source_url: https://github.com/taiki-e/parse-changelog/releases/download
         run: |
           curl -LsSf "${source_url}/${parse_changelog_tag}/parse-changelog-${target}.tar.gz" | tar xzf -
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.github/workflows/publish_release.yml` & `cmake_pre_commit_hooks-1.9.6/.github/workflows/publish_release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if: >-
       startsWith(github.ref, 'refs/tags/')
       || (github.event_name == 'pull_request' && github.event.pull_request.merged == true
           && (startsWith(github.event.pull_request.head.ref, 'release/')
               || startsWith(github.event.pull_request.head.ref, 'hotfix/')))
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
 
       - name: Extract version from tag name
@@ -100,15 +100,15 @@
           fi
           gh release create "v${RELEASE_VERSION}" ${prerelease:-} \
           --title "cmake-pre-commit-hooks v${RELEASE_VERSION}" \
           --notes "${notes:-}" \
           dist/*
 
       - name: Setup Python for Pypi upload
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
 
       - name: Publish standard package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
           packages_dir: dist/
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.github/workflows/pull_request.yml` & `cmake_pre_commit_hooks-1.9.6/.github/workflows/pull_request.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
   update-changelog:
     runs-on: ubuntu-latest
     name: "Pre-commit CI CHANGELOG auto-update"
     if: >
       (github.event.pull_request.title == '[pre-commit.ci] pre-commit autoupdate') &&
       (github.event.action == 'opened')
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.ref }}
           fetch-depth: 0
           token: ${{ secrets.PRE_COMMIT_CI_CHANGELOG }}
 
       - name: Setup Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: '3.11'
           cache: 'pip'
           cache-dependency-path: '**/pyproject.toml'
 
       - name: Install dependencies
         run: |
@@ -44,15 +44,15 @@
 
   changelog:
     needs: update-changelog
     runs-on: ubuntu-latest
     name: CHANGELOG enforcer
     if: '!cancelled()'
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.ref }}
           fetch-depth: 0
 
       - uses: dangoslen/changelog-enforcer@v3
         with:
           changeLogPath: 'CHANGELOG.md'
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.gitignore` & `cmake_pre_commit_hooks-1.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.6/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -2,74 +2,74 @@
 
 repos:
   - repo: meta
     hooks:
       - id: check-useless-excludes
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.5.4
+    rev: v1.5.5
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/PyCQA/doc8/
     rev: v1.1.1
     hooks:
       - id: doc8
         require_serial: false
         additional_dependencies: [tomli]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.6
+    rev: v2.3.0
     hooks:
       - id: codespell
         files: .*\.(py|txt|cmake|md|rst|sh|ps1|hpp|tpp|cpp|cc)$
         args: [-I, .codespell.allow]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.6
+    rev: v0.10.0.1
     hooks:
       - id: shellcheck
         require_serial: false
         args: [-x, --severity=info]
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.33.0
+    rev: v1.35.1
     hooks:
       - id: yamllint
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.16.0
     hooks:
       - id: blacken-docs
         args: [-S, -l, '120']
         additional_dependencies: [black==22.12.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.8
+    rev: v0.4.7
     hooks:
       - id: ruff-format
         name: ruff (format)
         args: [--preview]
 
       - id: ruff
         name: ruff (fix)
         alias: ruff-fix
         args:
           - --fix
           - --exit-non-zero-on-fix
-          - --show-source
+          - --output-format=full
           - --show-fixes
           - --preview
```

### Comparing `cmake_pre_commit_hooks-1.9.5/.pre-commit-hooks.yaml` & `cmake_pre_commit_hooks-1.9.6/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/CHANGELOG.md` & `cmake_pre_commit_hooks-1.9.6/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,37 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v1.9.6] - 2024-06-02
+
+### Changed
+
+- Apply new linter/formatters
+
+### Fixed
+
+- Fixed a bug where a condition always evaluated to `true`
+
+### Repository
+
+- Update GitHub Action `action/setup-python` to v5
+- Update GitHub Action `codecov/codecov-action` from v3 to v4
+- Update GitHub Action `ilammy/msvc-dev-cmd` from v1.12.1 to v1.13.0
+- Update GitHub Action `thomaseizinger/create-pull-request` to v1.4.0
+- Update `adrienverge/yamllint` hook to v1.35.1
+- Update `astral-sh/ruff-pre-commit` hook to v0.4.5
+- Update `codespell-project/codespell` hook to v2.3.0
+- Update `Lucas-C/pre-commit-hook` hook to v1.5.5
+- Update `pre-commit/pre-commit-hooks` hook to v4.6.0
+- Update `shellcheck-py/shellcheck-py` hook to v0.10.0
+
 ## [v1.9.5] - 2023-12-15
 
 ### Added
 
 - Added metadata to mark support for Python 3.12 and enabled CI checks for it
 - Implemented PEP-621
 
@@ -182,15 +205,17 @@
   - codespell
   - yamllint
   - blacken-docs
   - pyupgrade
 
 ### Repository
 
-- Update `action/setup-python` GitHub Action to v4
+- Update `action/setup-python` GitHub Action to v5
+- Update `action/checkout` GitHub Action to v4
+- Update `github/codeql-action/analyze` GitHub Action to v3
 - Update `ilammy/msvc-dev-cmd` GitHub Action to v1.12.1
 - Update `thomaseizinger/create-pull-request` GitHub Action to v1.3.0
 - Update `Lucas-C/pre-commit-hooks` hook to v1.4.2
 - Update `asottile/pyupgrade` to v3.2.0
 - Update `black` hook to v22.10.0
 - Update `blacken-docs` hook to v1.13.0
 - Update `flake8` hook to v5.0.4
@@ -211,14 +236,15 @@
 
 - Correctly pass on the default argument list to `CLinters`
 - Fixed issues with release publishing workflows on GitHub
 
 ### Repository
 
 - Update GitHub's CodeQL action to v2
+- Update `astral-sh/ruff-pre-commit` hook to v0.4.7
 - Update `pre-commit/pre-commit-hooks` hook to v4.3.0
 - Update `Lucas-C/pre-commit-hooks` hook to v1.2.0
 - Update `pre-commit/mirrors-pylint` hook to v3.0.0a5
 - Update `dangoslen/changelog-enforcer` GitHub action to v3
 - Update `thomaseizinger/create-pull-request` GitHub action to v1.2.2
 - Update `black` hook to v22.3.0
 - Update `check-manifest` to v0.48
@@ -237,14 +263,15 @@
 
 ### Repository
 
 - New step in "Format" GitHub action to make sure the CHANGELOG is updated with proper version section for hotfix/\_
   and release/\_ branches
 - Update `isort` hook to v5.10.1
 - Update `black` hook to v21.12b0
+- Disable macOS CI for Python \< 3.11 (now runs on M1 macs on GitHub)
 
 ## [v1.5.0] - 2021-11-08
 
 ### Added
 
 - Support for `cpplint`
 - Support for `lizard`, a code complexity analyzer
@@ -369,15 +396,15 @@
 
 Initial release with support for:
 
 - clang-format
 - clang-tidy
 - cppcheck
 
-[unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.5...HEAD
+[unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.6...HEAD
 [v1.0.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/20b1113bf223273cda31a14a82c9d573a342de4a...v1.0.0
 [v1.0.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.0...v1.0.1
 [v1.1.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.1...v1.1.0
 [v1.1.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.0...v1.1.1
 [v1.1.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.1...v1.1.2
 [v1.2.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.2...v1.2.0
 [v1.3.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.2.0...v1.3.0
@@ -392,7 +419,8 @@
 [v1.8.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...v1.8.1
 [v1.9.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...v1.9.0
 [v1.9.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.0...v1.9.1
 [v1.9.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.1...v1.9.2
 [v1.9.3]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.2...v1.9.3
 [v1.9.4]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.3...v1.9.4
 [v1.9.5]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.4...v1.9.5
+[v1.9.6]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.5...v1.9.6
```

### Comparing `cmake_pre_commit_hooks-1.9.5/LICENSE` & `cmake_pre_commit_hooks-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/PKG-INFO` & `cmake_pre_commit_hooks-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake_pre_commit_hooks
-Version: 1.9.5
+Version: 1.9.6
 Summary: pre-commit hooks for CMake-based projects
 Author-email: Damien Nguyen <ngn.damien@gmail.com>
 License: Apache2
 Project-URL: Homepage, https://github.com/Takishima/cmake-pre-commit-hooks
 Project-URL: Pypi, https://pypi.org/project/cmake-pre-commit-hooks/
 Project-URL: Repository, https://github.com/Takishima/cmake-pre-commit-hooks
 Project-URL: Issues, https://github.com/Takishima/cmake-pre-commit-hooks/issues
```

### Comparing `cmake_pre_commit_hooks-1.9.5/README.md` & `cmake_pre_commit_hooks-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/__init__.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_argparse.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_argparse.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_call_process.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_call_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #   limitations under the License.
 
 """Sub-process handling classes and functions."""
 
 from __future__ import annotations
 
 import logging
-import subprocess as sp
+import subprocess as sp  # noqa: S404
 import sys
 
 import attrs
 
 
 @attrs.define(slots=True)
 class History:  # pylint: disable=too-few-public-methods
```

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_cmake.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_cmake.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import contextlib
 import json
 import logging
 import os
 import platform
 import re
 import shutil
-import subprocess as sp
+import subprocess as sp  # noqa: S404
 import sys
 from pathlib import Path
 
 import fasteners
 import filelock
 
 from . import _argparse, _call_process
@@ -62,17 +62,17 @@
         cmake_names (:obj:`list` of :obj:`str`): Names for the CMake command
             Defaults to ['cmake', 'cmake3']
     """
     if not cmake_names:
         cmake_names = ['cmake', 'cmake3']
 
     for cmake in cmake_names:
-        cmake_cmd = [shutil.which(cmake)]
-        if cmake_cmd is not None and _try_calling_cmake(cmake_cmd):
-            return cmake_cmd
+        cmake_cmd = shutil.which(cmake)
+        if cmake_cmd is not None and _try_calling_cmake([cmake_cmd]):
+            return [cmake_cmd]
 
         # CMake not in PATH, should have installed Python CMake module
         # -> try to find out where it is
         python_executable = Path(sys.executable)
         try:
             root_path = Path(os.environ['VIRTUAL_ENV'])
             python = python_executable.name
@@ -124,28 +124,33 @@
         """Add CMake options to an argparse.ArgumentParser."""
         # Create option group here to control the order
         cmake_options = parser.add_argument_group(
             title='CMake options',
             description='Options mirroring those of CMake and that will be passed onto CMake as-is.',
         )
         options = parser.add_argument_group(
-            title='Other CMake related options', description='Options used to configure how CMake is called'
+            title='Other CMake related options',
+            description='Options used to configure how CMake is called',
         )
         platform_specific_cmake = parser.add_argument_group(
             title='Options to define platform-dependent CMake variables',
             description=(
                 'This allows you to set CMake variables during the configuration depending on the platform the hooks '
                 'are currently running on.'
                 'For example --unix="CMAKE_CXX_COMPILER=g++" will only define this CMake variable on UNIX platforms.'
             ),
         )
 
         # Custom options
         options.add_argument('--clean', action='store_true', help='Start from a clean build directory')
-        options.add_argument('--cmake', type=_argparse.executable_path, help='Specify path to CMake executable.')
+        options.add_argument(
+            '--cmake',
+            type=_argparse.executable_path,
+            help='Specify path to CMake executable.',
+        )
         options.add_argument(
             '--detect-configured-files',
             action='store_true',
             help='Enable tracing of files generated  using the configure_file(...) CMake function',
         )
         options.add_argument(
             '--no-automatic-discovery',
@@ -167,66 +172,109 @@
         platform_specific_cmake.add_argument(
             '--unix',
             action=_argparse.OSSpecificAction,
             type=str,
             help='Unix-only (ie. Linux and MacOS) options for CMake',
         )
         platform_specific_cmake.add_argument(
-            '--linux', action=_argparse.OSSpecificAction, type=str, help='Linux-only options for CMake'
+            '--linux',
+            action=_argparse.OSSpecificAction,
+            type=str,
+            help='Linux-only options for CMake',
         )
         platform_specific_cmake.add_argument(
-            '--mac', action=_argparse.OSSpecificAction, type=str, help='Mac-only options for CMake'
+            '--mac',
+            action=_argparse.OSSpecificAction,
+            type=str,
+            help='Mac-only options for CMake',
         )
         platform_specific_cmake.add_argument(
-            '--win', action=_argparse.OSSpecificAction, type=str, help='Windows-only options for CMake'
+            '--win',
+            action=_argparse.OSSpecificAction,
+            type=str,
+            help='Windows-only options for CMake',
         )
 
         # CMake-like options
         cmake_options.add_argument('-S', '--source-dir', type=str, help='Path to build directory', default='.')
-        cmake_options.add_argument('-B', '--build-dir', action='append', type=str, help='Path to build directory')
         cmake_options.add_argument(
-            '-D', dest='defines', action='append', type=str, help='Create or update a cmake cache entry.', default=[]
+            '-B',
+            '--build-dir',
+            action='append',
+            type=str,
+            help='Path to build directory',
+        )
+        cmake_options.add_argument(
+            '-D',
+            dest='defines',
+            action='append',
+            type=str,
+            help='Create or update a cmake cache entry.',
+            default=[],
         )
         cmake_options.add_argument(
             '-U',
             dest='undefines',
             action='append',
             type=str,
             help='Remove matching entries from CMake cache.',
             default=[],
         )
         cmake_options.add_argument('-G', dest='generator', type=str, help='Specify a build system generator.')
         cmake_options.add_argument(
-            '-T', dest='toolset', type=str, help='Specify toolset name if supported by generator.'
+            '-T',
+            dest='toolset',
+            type=str,
+            help='Specify toolset name if supported by generator.',
         )
-        cmake_options.add_argument('-A', dest='platform', type=str, help='Specify platform if supported by generator.')
         cmake_options.add_argument(
-            '-Werror', dest='errors', choices=['dev'], help='Make developer warnings errors.', default=[]
+            '-A',
+            dest='platform',
+            type=str,
+            help='Specify platform if supported by generator.',
+        )
+        cmake_options.add_argument(
+            '-Werror',
+            dest='errors',
+            choices=['dev'],
+            help='Make developer warnings errors.',
+            default=[],
         )
         cmake_options.add_argument(
             '-Wno-error',
             dest='no_errors',
             choices=['dev'],
             help='Make developer warnings not errors.',
             default=[],
         )
         cmake_options.add_argument('--preset', type=str, help='Specify a configure preset.')
 
-        cmake_options.add_argument('-Wdev', dest='dev_warnings', action='store_true', help='Enable developer warnings.')
         cmake_options.add_argument(
-            '-Wno-dev', dest='no_dev_warnings', action='store_true', help='Suppress developer warnings.'
+            '-Wdev',
+            dest='dev_warnings',
+            action='store_true',
+            help='Enable developer warnings.',
+        )
+        cmake_options.add_argument(
+            '-Wno-dev',
+            dest='no_dev_warnings',
+            action='store_true',
+            help='Suppress developer warnings.',
         )
 
     def resolve_build_directory(self, build_dir_list=None, *, automatic_discovery=True):
         """Locate a valid build directory based on internal list and automatic discovery if enabled."""
         # First try to locate a valid build directory based on internal list
         build_dir_list = [] if build_dir_list is None else [Path(path) for path in build_dir_list]
         for build_dir in build_dir_list:
             if build_dir.exists() and Path(build_dir, 'CMakeCache.txt').exists():
-                logging.debug('Located valid build directory with CMakeCache.txt at: %s', str(build_dir))
+                logging.debug(
+                    'Located valid build directory with CMakeCache.txt at: %s',
+                    str(build_dir),
+                )
                 self.build_dir = build_dir.resolve()
                 return
 
         # If that fails or none have been passed, attempt automatic discovery
         if automatic_discovery:
             for path in sorted(self.source_dir.glob('*')):
                 if path.is_dir() and (path / 'CMakeCache.txt').exists():
@@ -239,15 +287,18 @@
             self.build_dir = None
             return
 
         if not build_dir_list:
             self.build_dir = self.source_dir / self.DEFAULT_BUILD_DIR
         else:
             self.build_dir = Path(build_dir_list[0]).resolve()
-        logging.info('Unable to locate a valid build directory. Will be creating one at %s', str(self.build_dir))
+        logging.info(
+            'Unable to locate a valid build directory. Will be creating one at %s',
+            str(self.build_dir),
+        )
 
     def setup_cmake_args(self, cmake_args):  # noqa: C901
         """
         Setup CMake arguments.
 
         Args:
             cmake_args: Dictionary-like data structure with following keys:
@@ -268,15 +319,16 @@
         """
         self.source_dir = Path(cmake_args.source_dir).resolve()
         if cmake_args.cmake:
             self.command = [Path(cmake_args.cmake).resolve()]
         self.no_cmake_configure = cmake_args.no_cmake_configure
 
         self.resolve_build_directory(
-            build_dir_list=cmake_args.build_dir, automatic_discovery=cmake_args.automatic_discovery
+            build_dir_list=cmake_args.build_dir,
+            automatic_discovery=cmake_args.automatic_discovery,
         )
 
         if cmake_args.detect_configured_files and self.build_dir:
             self.cmake_trace_log = self.build_dir / self.DEFAULT_TRACE_LOG
 
         keyword_args = {
             'defines': ([], '-D{}'),
@@ -340,21 +392,37 @@
         self.build_dir.mkdir(exist_ok=True)
 
         cmake_configure_try_lock = filelock.FileLock(cmake_configure_try_lock_file)
         cmake_configure_lock = fasteners.InterProcessReaderWriterLock(cmake_configure_lock_file)
         try:
             with cmake_configure_try_lock.acquire(blocking=False):  # noqa: SIM117
                 with cmake_configure_lock.write_lock():
-                    logging.debug('Command %s with id %s is running CMake configure', command, os.getpid())
+                    logging.debug(
+                        'Command %s with id %s is running CMake configure',
+                        command,
+                        os.getpid(),
+                    )
                     returncode = self._configure(
-                        lock_files=(cmake_configure_lock_file, cmake_configure_try_lock_file), clean_build=clean_build
+                        lock_files=(
+                            cmake_configure_lock_file,
+                            cmake_configure_try_lock_file,
+                        ),
+                        clean_build=clean_build,
+                    )
+                    logging.debug(
+                        'Command %s with id %s is done running CMake configure',
+                        command,
+                        os.getpid(),
                     )
-                    logging.debug('Command %s with id %s is done running CMake configure', command, os.getpid())
         except filelock.Timeout:
-            logging.debug('Command %s with id %s is not running CMake configure and waiting', command, os.getpid())
+            logging.debug(
+                'Command %s with id %s is not running CMake configure and waiting',
+                command,
+                os.getpid(),
+            )
             with cmake_configure_lock.read_lock():
                 logging.debug('Command %s with id %s is done waiting', command, os.getpid())
                 returncode = 0
 
         if returncode != 0:
             logging.error('CMake configure step failed. See output for more information.')
             sys.exit(returncode)
@@ -364,15 +432,16 @@
 
     def _call_cmake(self, extra_args=None):
         command = [str(cmd) for cmd in self.command]
         if extra_args is None:
             extra_args = []
 
         result = _call_process.call_process(
-            [*command, str(self.source_dir), *self.cmake_args, *extra_args], cwd=str(self.build_dir)
+            [*command, str(self.source_dir), *self.cmake_args, *extra_args],
+            cwd=str(self.build_dir),
         )
         result.stdout = '\n'.join([
             f'Running CMake with: {[*command, str(self.source_dir), *self.cmake_args]}',
             f'  from within {self.build_dir}',
             result.stdout,
             '',
         ])
@@ -388,15 +457,19 @@
                 if path.is_dir():
                     shutil.rmtree(path)
                 elif path not in lock_files:
                     path.unlink()
 
         extra_args = []
         if self.cmake_trace_log:
-            extra_args.extend(['--trace-expand', '--trace-format=json-v1', f'--trace-redirect={self.cmake_trace_log}'])
+            extra_args.extend([
+                '--trace-expand',
+                '--trace-format=json-v1',
+                f'--trace-redirect={self.cmake_trace_log}',
+            ])
 
         result = self._call_cmake(extra_args=extra_args)
 
         compiledb = Path(self.build_dir, 'compile_commands.json')
         if not compiledb.exists():
             result.returncode = 1
             result.stderr += f'\nUnable to locate {compiledb}\n\n'
@@ -447,12 +520,16 @@
         with self.cmake_trace_log.open('r') as fd:
             configure_file_calls = [json.loads(line) for line in fd.readlines()]
 
         for configure_file_call in (data for data in configure_file_calls if _is_relevant_configure_file_call(data)):
             input_file, configured_file = (Path(arg) for arg in configure_file_call['args'][:2])
             if not configured_file.is_absolute():
                 configured_file = self.build_dir / configured_file
-            logging.debug('detected call to configure_file(%s %s [...])', str(input_file), str(configured_file))
+            logging.debug(
+                'detected call to configure_file(%s %s [...])',
+                str(input_file),
+                str(configured_file),
+            )
             self.cmake_configured_files.append(str(configured_file))
 
 
 # ==============================================================================
```

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/_utils.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         hook_options.add_argument('positionals', metavar='filenames', nargs='*', help='Filenames to check')
 
         known_args, self.args = parser.parse_known_args(args[1:])
 
         self.all_at_once = known_args.all_at_once
         self.read_json_db = known_args.read_json_db
         self.clean_build = known_args.clean
-        self.build_dir_list.extend(known_args.build_dir if known_args.build_dir else [])
+        self.build_dir_list.extend(known_args.build_dir or [])
 
         if not known_args.build_dir and known_args.preset:
             raise CMakePresetError
 
         if self.setup_cmake:
             self.cmake.setup_cmake_args(known_args)
```

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/clang_format.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/clang_format.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/clang_tidy.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/clang_tidy.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/cppcheck.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/cppcheck.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/cpplint.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/cpplint.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/include_what_you_use.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/include_what_you_use.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pc_hooks/lizard.py` & `cmake_pre_commit_hooks-1.9.6/cmake_pc_hooks/lizard.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/PKG-INFO` & `cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmake-pre-commit-hooks
-Version: 1.9.5
+Name: cmake_pre_commit_hooks
+Version: 1.9.6
 Summary: pre-commit hooks for CMake-based projects
 Author-email: Damien Nguyen <ngn.damien@gmail.com>
 License: Apache2
 Project-URL: Homepage, https://github.com/Takishima/cmake-pre-commit-hooks
 Project-URL: Pypi, https://pypi.org/project/cmake-pre-commit-hooks/
 Project-URL: Repository, https://github.com/Takishima/cmake-pre-commit-hooks
 Project-URL: Issues, https://github.com/Takishima/cmake-pre-commit-hooks/issues
```

### Comparing `cmake_pre_commit_hooks-1.9.5/cmake_pre_commit_hooks.egg-info/SOURCES.txt` & `cmake_pre_commit_hooks-1.9.6/cmake_pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/misc/license_header.txt` & `cmake_pre_commit_hooks-1.9.6/misc/license_header.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/pyproject.toml` & `cmake_pre_commit_hooks-1.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 
 # ==============================================================================
 
 [tool.ruff]
 line-length = 120
 target-version = 'py38'
 
+[tool.ruff.lint]
+
 select = ['F',     # pyflakes
           'E',     # pycodestyle
           'W',     # pycodestyle
           'C90',   # mccabe
           'I',     # isort
           'N',     # pep8-naming
           'D',     # pydocstyle
@@ -144,37 +146,36 @@
 
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 line-ending = 'lf'
 skip-magic-trailing-comma = false
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 
 'tests/python/*.py' = ['S101', 'SLF001', 'PLR0913', 'PLR2004', 'D']
 
-
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 ignore-fully-untyped = true
 mypy-init-return = true
 suppress-dummy-args = true
 suppress-none-returning = true
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = 'double'
 inline-quotes = 'single'
 multiline-quotes = 'single'
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 section-order = ["future", "standard-library", "first-party", "third-party", "local-folder"]
 split-on-trailing-comma = false
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = 'google'
 
 # ------------------------------------------------------------------------------
 
 [tool.check-manifest]
 ignore = [
 'PKG-INFO',
```

### Comparing `cmake_pre_commit_hooks-1.9.5/setup.py` & `cmake_pre_commit_hooks-1.9.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Dummy setup script."""
 
 from __future__ import annotations
 
 import logging
 import os
 import shutil
-import subprocess
+import subprocess  # noqa: S404
 import sys
 from pathlib import Path
 
 from setuptools import setup
 from setuptools.command.egg_info import egg_info
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/cmake_bad/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.6/tests/cmake_bad/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/cmake_good/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.6/tests/cmake_good/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/_argparse_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/_argparse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 
 import argparse
 import contextlib
 import platform
 from textwrap import dedent
 
-from cmake_pc_hooks import _argparse
+from cmake_pc_hooks import _argparse  # noqa: PLC2701
 
 import pytest
-from _test_utils import ExitError
+from _test_utils import ExitError  # noqa: PLC2701
 
 # ==============================================================================
 
 
 def _add_simple_args(parser):
     parser.add_argument('--flag', action='store_true')
     parser.add_argument('--no-flag', action='store_false')
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/_call_process_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/_call_process_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import subprocess as sp
+import subprocess as sp  # noqa: S404
 
-from cmake_pc_hooks._call_process import History, call_process
+from cmake_pc_hooks._call_process import History, call_process  # noqa: PLC2701
 
 import pytest
 
 # ==============================================================================
 
 
 @pytest.mark.parametrize('disable_print', [False, True])
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/_cmake_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/_cmake_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 import argparse
 import platform
 import sys
 from pathlib import Path
 from textwrap import dedent
 
-from cmake_pc_hooks._cmake import CMakeCommand, _try_calling_cmake, get_cmake_command
+from cmake_pc_hooks._cmake import CMakeCommand, _try_calling_cmake, get_cmake_command  # noqa: PLC2701
 
 import fasteners
 import filelock
 import pytest
-from _test_utils import ExitError
+from _test_utils import ExitError  # noqa: PLC2701
 
 # ==============================================================================
 
 _has_cmake = get_cmake_command() is not None
 
 # ==============================================================================
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/_test_utils.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/_test_utils.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/_utils_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
-from cmake_pc_hooks import _utils
-from cmake_pc_hooks._cmake import CMakeCommand
+from cmake_pc_hooks import _utils  # noqa: PLC2701
+from cmake_pc_hooks._cmake import CMakeCommand  # noqa: PLC2701
 
 import pytest
-from _test_utils import run_command_default_assertions
+from _test_utils import run_command_default_assertions  # noqa: PLC2701
 
 # ==============================================================================
 
 
 def test_read_compile_commands_no_file(tmp_path):
     assert not _utils._read_compile_commands_json(tmp_path / 'compile_commands.json')
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/clang_format_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/clang_format_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from cmake_pc_hooks import clang_format
 
 import pytest
-from _test_utils import command_main_asserts
+from _test_utils import command_main_asserts  # noqa: PLC2701
 
 # ==============================================================================
 
 
 @pytest.mark.parametrize('format_success', [False, True])
 def test_clang_format_command(mocker, tmp_path, format_success):
     mocker.patch('hooks.utils.Command.check_installed', return_value=True)
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/clang_tidy_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/clang_tidy_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 from cmake_pc_hooks import clang_tidy
 
 import pytest
-from _test_utils import command_main_asserts, run_command_default_assertions
+from _test_utils import command_main_asserts, run_command_default_assertions  # noqa: PLC2701
 
 # ==============================================================================
 
 
 @pytest.mark.parametrize('stdout', ['', 'aaa'], ids=['<empty>', 'aaa'])
 @pytest.mark.parametrize(
     'error_msg', [None, '1 error generated.', '2 errors generated.'], ids=['<empty>', '1_error', '2_errors']
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/conftest.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import json
 from collections import namedtuple
 
 import pytest
-from _test_utils import ExitError
+from _test_utils import ExitError  # noqa: PLC2701
 
 # ==============================================================================
 
 
 @pytest.fixture()
 def compile_commands(tmp_path):
     path = tmp_path / 'build' / 'compile_commands.json'
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/cppcheck_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/cppcheck_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 from cmake_pc_hooks import cppcheck
 
-from _test_utils import command_main_asserts, run_command_default_assertions
+from _test_utils import command_main_asserts, run_command_default_assertions  # noqa: PLC2701
 
 # ==============================================================================
 
 
 def test_cppcheck_command(mocker, setup_command):
     path = setup_command.compile_db_path
     call_process = setup_command.call_process
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/cpplint_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/cpplint_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/iwyu_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/iwyu_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 from cmake_pc_hooks import include_what_you_use
 
 import pytest
-from _test_utils import command_main_asserts, run_command_default_assertions
+from _test_utils import command_main_asserts, run_command_default_assertions  # noqa: PLC2701
 
 # ==============================================================================
 
 
 def test_get_iwyu_tool_command(mocker):
     iwyu_tool_fname = 'iwyu_tool'
     shutil_which = mocker.patch('shutil.which', return_value=iwyu_tool_fname)
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/python/lizard_test.py` & `cmake_pre_commit_hooks-1.9.6/tests/python/lizard_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 from cmake_pc_hooks import lizard
 
-from _test_utils import command_main_asserts, run_command_default_assertions
+from _test_utils import command_main_asserts, run_command_default_assertions  # noqa: PLC2701
 
 # ==============================================================================
 
 
 def test_lizard_command(tmp_path, setup_command):
     path = setup_command.compile_db_path
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/run_tests.ps1` & `cmake_pre_commit_hooks-1.9.6/tests/run_tests.ps1`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 $build_dir = "build"
-$CMakeArgs = '-GNinja', '-DCMAKE_C_COMPILER="cl.exe"', '-DCMAKE_CXX_COMPILER="cl.exe"'
+$CMakeArgs = '-GNinja', '-DCMAKE_C_COMPILER=cl.exe', '-DCMAKE_CXX_COMPILER=cl.exe'
 
 Set-PSDebug -trace 1
 
 Function run_hook
 {
     Param($Hook,
           $Src,
```

### Comparing `cmake_pre_commit_hooks-1.9.5/tests/run_tests.sh` & `cmake_pre_commit_hooks-1.9.6/tests/run_tests.sh`

 * *Files identical despite different names*

