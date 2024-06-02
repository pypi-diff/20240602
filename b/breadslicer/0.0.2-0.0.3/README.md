# Comparing `tmp/breadslicer-0.0.2.tar.gz` & `tmp/breadslicer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breadslicer-0.0.2.tar", max compression
+gzip compressed data, was "breadslicer-0.0.3.tar", max compression
```

## Comparing `breadslicer-0.0.2.tar` & `breadslicer-0.0.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     9858 2024-06-01 16:57:48.639838 breadslicer-0.0.2/README.md
--rw-r--r--   0        0        0     1443 2024-06-01 16:57:48.640838 breadslicer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.680838 breadslicer-0.0.2/src/breadslicer/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.680838 breadslicer-0.0.2/src/breadslicer/application/__init__.py
--rw-r--r--   0        0        0     3019 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/application/app.py
--rw-r--r--   0        0        0     1950 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/application/renderer.py
--rw-r--r--   0        0        0     1849 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/application/slice.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.681838 breadslicer-0.0.2/src/breadslicer/components/__init__.py
--rw-r--r--   0        0        0      346 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/components/base.py
--rw-r--r--   0        0        0      655 2024-06-01 16:57:48.641838 breadslicer-0.0.2/src/breadslicer/components/choice.py
--rw-r--r--   0        0        0      494 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/confirm.py
--rw-r--r--   0        0        0      476 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/editor.py
--rw-r--r--   0        0        0      516 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/multiple_choice.py
--rw-r--r--   0        0        0      473 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/password.py
--rw-r--r--   0        0        0     1195 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/components/text.py
--rwxr-xr-x   0        0        0     1823 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/main.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/breadslicer/py.typed
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/breadslicer/utility/__init__.py
--rw-r--r--   0        0        0      349 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/abstractdataclass.py
--rw-r--r--   0        0        0     1841 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/command.py
--rw-r--r--   0        0        0      486 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/fs.py
--rw-r--r--   0        0        0      274 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/breadslicer/utility/git.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/__init__.py
--rw-r--r--   0        0        0     2975 2024-06-01 16:57:48.642838 breadslicer-0.0.2/src/opinionated/bread.py
--rw-r--r--   0        0        0     3231 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/cleanup.py
--rw-r--r--   0        0        0     1296 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/dependencies.py
--rw-r--r--   0        0        0      263 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.alpine
--rw-r--r--   0        0        0      334 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.debian
--rw-r--r--   0        0        0     1302 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.python
--rw-r--r--   0        0        0      339 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/Dockerfile.slim
--rw-r--r--   0        0        0     2905 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/app.gitlab-ci.yml
--rw-r--r--   0        0        0     1917 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/lib.gitlab-ci.yml
--rw-r--r--   0        0        0     2259 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/includes/utils.gitlab-ci.yml
--rw-r--r--   0        0        0      124 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/project_types.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/py.typed
--rw-r--r--   0        0        0     4512 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/questions.py
--rw-r--r--   0        0        0     2169 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/templates/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       61 2024-06-01 16:57:48.643838 breadslicer-0.0.2/src/opinionated/templates/.dockerignore
--rw-r--r--   0        0        0     1298 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.envrc
--rw-r--r--   0        0        0      121 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.flake8
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/.github/workflows/.keep
--rw-r--r--   0        0        0      208 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.gitignore
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/.gitlab/.keep
--rw-r--r--   0        0        0      146 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.gitlab-ci.yml
--rw-r--r--   0        0        0      186 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     3420 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.print_help.py
--rw-r--r--   0        0        0      685 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/extensions.json
--rw-r--r--   0        0        0     2666 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/launch.json
--rw-r--r--   0        0        0      643 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/settings.json
--rw-r--r--   0        0        0     1238 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/.vscode/tasks.json
--rw-r--r--   0        0        0      211 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/Dockerfile
--rw-r--r--   0        0        0     4888 2024-06-01 16:57:48.644838 breadslicer-0.0.2/src/opinionated/templates/Makefile
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/README.md
--rwxr-xr-x   0        0        0      674 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/manage.py-tpl
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.685838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      428 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/asgi.py-tpl
--rw-r--r--   0        0        0     3390 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/settings.py-tpl
--rw-r--r--   0        0        0      789 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0      428 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/wsgi.py-tpl
--rw-r--r--   0        0        0      929 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/doc_conf/conf.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flask/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flask/py.typed
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flat/__init__.py
--rwxr-xr-x   0        0        0     1844 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/flat/main.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/flat/py.typed
--rw-r--r--   0        0        0       75 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/poetry.toml
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/py.typed
--rw-r--r--   0        0        0     1617 2024-06-01 16:57:48.645838 breadslicer-0.0.2/src/opinionated/templates/pyproject.toml
--rwxr-xr-x   0        0        0       23 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/build.sh
--rwxr-xr-x   0        0        0      118 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/install_full_pkg.sh
--rwxr-xr-x   0        0        0       30 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/release.sh
--rwxr-xr-x   0        0        0       95 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/tests.sh
--rwxr-xr-x   0        0        0       56 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/scripts/verify.sh
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/__init__.py
--rwxr-xr-x   0        0        0     1844 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/main.py
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/py.typed
--rw-r--r--   0        0        0        0 2024-06-01 16:57:48.686838 breadslicer-0.0.2/src/opinionated/templates/tests/__init__.py
--rw-r--r--   0        0        0      178 2024-06-01 16:57:48.646838 breadslicer-0.0.2/src/opinionated/templates/tests/test_dummy.py
--rw-r--r--   0        0        0    10578 1970-01-01 00:00:00.000000 breadslicer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     9858 2024-06-01 21:27:31.441632 breadslicer-0.0.3/README.md
+-rw-r--r--   0        0        0     1551 2024-06-01 21:27:31.442632 breadslicer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.481632 breadslicer-0.0.3/src/breadslicer/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.481632 breadslicer-0.0.3/src/breadslicer/application/__init__.py
+-rw-r--r--   0        0        0     3019 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/application/app.py
+-rw-r--r--   0        0        0     1950 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/application/renderer.py
+-rw-r--r--   0        0        0     1849 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/application/slice.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.481632 breadslicer-0.0.3/src/breadslicer/components/__init__.py
+-rw-r--r--   0        0        0      346 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/components/base.py
+-rw-r--r--   0        0        0      655 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/components/choice.py
+-rw-r--r--   0        0        0      494 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/components/confirm.py
+-rw-r--r--   0        0        0      476 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/components/editor.py
+-rw-r--r--   0        0        0      516 2024-06-01 21:27:31.443632 breadslicer-0.0.3/src/breadslicer/components/multiple_choice.py
+-rw-r--r--   0        0        0      473 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/components/password.py
+-rw-r--r--   0        0        0     1272 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/components/text.py
+-rwxr-xr-x   0        0        0     1823 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/main.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.484632 breadslicer-0.0.3/src/breadslicer/py.typed
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.485632 breadslicer-0.0.3/src/breadslicer/utility/__init__.py
+-rw-r--r--   0        0        0      349 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/utility/abstractdataclass.py
+-rw-r--r--   0        0        0     1841 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/utility/command.py
+-rw-r--r--   0        0        0      486 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/utility/fs.py
+-rw-r--r--   0        0        0      274 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/breadslicer/utility/git.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.485632 breadslicer-0.0.3/src/opinionated/__init__.py
+-rw-r--r--   0        0        0     3006 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/opinionated/bread.py
+-rw-r--r--   0        0        0     3338 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/opinionated/cleanup.py
+-rw-r--r--   0        0        0     1296 2024-06-01 21:27:31.444632 breadslicer-0.0.3/src/opinionated/dependencies.py
+-rw-r--r--   0        0        0      263 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/Dockerfile.alpine
+-rw-r--r--   0        0        0      334 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/Dockerfile.debian
+-rw-r--r--   0        0        0     1302 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/Dockerfile.python
+-rw-r--r--   0        0        0      339 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/Dockerfile.slim
+-rw-r--r--   0        0        0     2905 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/app.gitlab-ci.yml
+-rw-r--r--   0        0        0     1917 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/lib.gitlab-ci.yml
+-rw-r--r--   0        0        0     2259 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/includes/utils.gitlab-ci.yml
+-rw-r--r--   0        0        0      124 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/project_types.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.485632 breadslicer-0.0.3/src/opinionated/py.typed
+-rw-r--r--   0        0        0     4512 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/questions.py
+-rw-r--r--   0        0        0     2169 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/templates/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       61 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/templates/.dockerignore
+-rw-r--r--   0        0        0     1298 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/templates/.envrc
+-rw-r--r--   0        0        0      121 2024-06-01 21:27:31.445632 breadslicer-0.0.3/src/opinionated/templates/.flake8
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.485632 breadslicer-0.0.3/src/opinionated/templates/.github/workflows/.keep
+-rw-r--r--   0        0        0      208 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.gitignore
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.485632 breadslicer-0.0.3/src/opinionated/templates/.gitlab/.keep
+-rw-r--r--   0        0        0      146 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.gitlab-ci.yml
+-rw-r--r--   0        0        0      186 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     3420 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.print_help.py
+-rw-r--r--   0        0        0      685 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.vscode/extensions.json
+-rw-r--r--   0        0        0     2666 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.vscode/launch.json
+-rw-r--r--   0        0        0      643 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.vscode/settings.json
+-rw-r--r--   0        0        0     1238 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/.vscode/tasks.json
+-rw-r--r--   0        0        0      211 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/Dockerfile
+-rw-r--r--   0        0        0     4888 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/Makefile
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.486632 breadslicer-0.0.3/src/opinionated/templates/README.md
+-rwxr-xr-x   0        0        0      674 2024-06-01 21:27:31.446632 breadslicer-0.0.3/src/opinionated/templates/django/project_template/manage.py-tpl
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.486632 breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      428 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/asgi.py-tpl
+-rw-r--r--   0        0        0     3390 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/settings.py-tpl
+-rw-r--r--   0        0        0      789 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0      428 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/wsgi.py-tpl
+-rw-r--r--   0        0        0      929 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/doc_conf/conf.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.486632 breadslicer-0.0.3/src/opinionated/templates/flask/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.486632 breadslicer-0.0.3/src/opinionated/templates/flask/py.typed
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.487632 breadslicer-0.0.3/src/opinionated/templates/flat/__init__.py
+-rwxr-xr-x   0        0        0     1844 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/flat/main.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.487632 breadslicer-0.0.3/src/opinionated/templates/flat/py.typed
+-rw-r--r--   0        0        0       75 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/poetry.toml
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.487632 breadslicer-0.0.3/src/opinionated/templates/py.typed
+-rw-r--r--   0        0        0     1617 2024-06-01 21:27:31.447632 breadslicer-0.0.3/src/opinionated/templates/pyproject.toml
+-rwxr-xr-x   0        0        0       23 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/scripts/build.sh
+-rwxr-xr-x   0        0        0      118 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/scripts/install_full_pkg.sh
+-rwxr-xr-x   0        0        0       30 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/scripts/release.sh
+-rwxr-xr-x   0        0        0       95 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/scripts/tests.sh
+-rwxr-xr-x   0        0        0       56 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/scripts/verify.sh
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.487632 breadslicer-0.0.3/src/opinionated/templates/src/{{project_slug}}/__init__.py
+-rwxr-xr-x   0        0        0     1844 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/src/{{project_slug}}/main.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.487632 breadslicer-0.0.3/src/opinionated/templates/src/{{project_slug}}/py.typed
+-rw-r--r--   0        0        0        0 2024-06-01 21:27:31.487632 breadslicer-0.0.3/src/opinionated/templates/tests/__init__.py
+-rw-r--r--   0        0        0      178 2024-06-01 21:27:31.448632 breadslicer-0.0.3/src/opinionated/templates/tests/test_dummy.py
+-rw-r--r--   0        0        0    10578 1970-01-01 00:00:00.000000 breadslicer-0.0.3/PKG-INFO
```

### Comparing `breadslicer-0.0.2/README.md` & `breadslicer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/pyproject.toml` & `breadslicer-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "breadslicer"
-version = "0.0.2"
+version = "0.0.3"
 description = "Commandline utililty to create python projects from templates"
 authors = ["Morten Rasmussen <netrom1337@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/mindsweeper/open-source/breadslicer"
 documentation = "https://mindsweeper.gitlab.io/open-source/breadslicer/"
 repository = "https://gitlab.com/mindsweeper/open-source/breadslicer"
 
@@ -53,9 +53,17 @@
 [[tool.mypy.overrides]]
 module = "inquirer.*,"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 python_files = ["test_*.py", "*_test.py", "testing/python/*.py", "tests.py", "**/tests.py"]
 addopts = "--ignore=src/opinionated/"  
+
+[tool.coverage.run]
+omit = [
+    "src/opinionated/templates/*",
+    "src/opinionated/includes/*",
+    ]
+
+
 [tool.bandit]
-exclude_dirs = [".venv/"]
+exclude_dirs = [".venv/"]
```

### Comparing `breadslicer-0.0.2/src/breadslicer/application/app.py` & `breadslicer-0.0.3/src/breadslicer/application/app.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/breadslicer/application/renderer.py` & `breadslicer-0.0.3/src/breadslicer/application/renderer.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/breadslicer/application/slice.py` & `breadslicer-0.0.3/src/breadslicer/application/slice.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/breadslicer/components/choice.py` & `breadslicer-0.0.3/src/breadslicer/components/choice.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/breadslicer/components/multiple_choice.py` & `breadslicer-0.0.3/src/breadslicer/components/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/breadslicer/components/text.py` & `breadslicer-0.0.3/src/breadslicer/components/text.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Callable, Dict, Optional
 
 import inquirer
 from inquirer.questions import Question
 
 from breadslicer.components.base import BaseComponent
 from breadslicer.utility.git import get_author_from_git, get_email_from_git
@@ -18,27 +18,31 @@
             message=self.message,
             default=self.default,
         )
 
 
 @dataclass
 class AuthorComponent(BaseComponent):
-    default: Optional[str | Callable[[Dict[str, str]], str]] = get_author_from_git()
+    default: Optional[str | Callable[[Dict[str, str]], str]] = field(
+        default_factory=get_author_from_git
+    )
 
     def component_question(self) -> Question:
         return inquirer.Text(
             name=self.name,
             message=self.message,
             default=self.default,
         )
 
 
 @dataclass
 class EmailComponent(BaseComponent):
-    default: Optional[str | Callable[[Dict[str, str]], str]] = get_email_from_git()
+    default: Optional[str | Callable[[Dict[str, str]], str]] = field(
+        default_factory=get_email_from_git
+    )
 
     def component_question(self) -> Question:
         return inquirer.Text(
             name=self.name,
             message=self.message,
             default=self.default,
         )
```

### Comparing `breadslicer-0.0.2/src/breadslicer/main.py` & `breadslicer-0.0.3/src/breadslicer/main.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/breadslicer/utility/command.py` & `breadslicer-0.0.3/src/breadslicer/utility/command.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/bread.py` & `breadslicer-0.0.3/src/opinionated/bread.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         match ProjectTypes[answers["project_type"]]:
             case ProjectTypes.app:
                 deps.app()
                 finalize.app()
             case ProjectTypes.lib:
                 deps.lib()
                 finalize.remove_main()
+                finalize.lib()
             case ProjectTypes.django:
                 deps.django()
                 finalize.django()
             case ProjectTypes.flask:
                 deps.flask()
                 finalize.flask()
         finalize.docs()
```

### Comparing `breadslicer-0.0.2/src/opinionated/cleanup.py` & `breadslicer-0.0.3/src/opinionated/cleanup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,21 @@
     def app(self):
         layout = self.answers["project_layout"]
         if layout == "flat":
             self.flat()
         elif layout == "str":
             self.src()
 
+    def lib(self):
+        layout = self.answers["project_layout"]
+        if layout == "flat":
+            self.flat()
+        elif layout == "src":
+            self.src()
+
     def django(self):
         """Install django packages and remove unused directory"""
 
         project_slug = self.answers["project_slug"]
         remove_paths([Path("flask"), Path("flat"), Path("src")])
 
         poetry_run(
@@ -98,11 +105,9 @@
                 Path("src"),
                 Path("templates"),
             ]
         )
         rename_path(Path("flat"), Path(project_slug))
 
     def src(self):
-        rename_path(Path("lib.gitlab-ci.yml"), Path(".gitlab-ci.yml"))
-        remove_paths(
-            [Path("django"), Path("flask"), Path("flat"), Path("app.gitlab-ci.yml")]
-        )
+        print("expected to remove some directories")
+        remove_paths([Path("django"), Path("flask"), Path("flat")])
```

### Comparing `breadslicer-0.0.2/src/opinionated/dependencies.py` & `breadslicer-0.0.3/src/opinionated/dependencies.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/includes/Dockerfile.python` & `breadslicer-0.0.3/src/opinionated/includes/Dockerfile.python`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/includes/app.gitlab-ci.yml` & `breadslicer-0.0.3/src/opinionated/includes/app.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/includes/lib.gitlab-ci.yml` & `breadslicer-0.0.3/src/opinionated/includes/lib.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/includes/utils.gitlab-ci.yml` & `breadslicer-0.0.3/src/opinionated/includes/utils.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/questions.py` & `breadslicer-0.0.3/src/opinionated/questions.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.devcontainer/devcontainer.json` & `breadslicer-0.0.3/src/opinionated/templates/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.envrc` & `breadslicer-0.0.3/src/opinionated/templates/.envrc`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.print_help.py` & `breadslicer-0.0.3/src/opinionated/templates/.print_help.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.vscode/extensions.json` & `breadslicer-0.0.3/src/opinionated/templates/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.vscode/launch.json` & `breadslicer-0.0.3/src/opinionated/templates/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.vscode/settings.json` & `breadslicer-0.0.3/src/opinionated/templates/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/.vscode/tasks.json` & `breadslicer-0.0.3/src/opinionated/templates/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/Makefile` & `breadslicer-0.0.3/src/opinionated/templates/Makefile`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/django/project_template/manage.py-tpl` & `breadslicer-0.0.3/src/opinionated/templates/django/project_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/settings.py-tpl` & `breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/django/project_template/project_name/urls.py-tpl` & `breadslicer-0.0.3/src/opinionated/templates/django/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/doc_conf/conf.py` & `breadslicer-0.0.3/src/opinionated/templates/doc_conf/conf.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/flat/main.py` & `breadslicer-0.0.3/src/opinionated/templates/flat/main.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/pyproject.toml` & `breadslicer-0.0.3/src/opinionated/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/src/opinionated/templates/src/{{project_slug}}/main.py` & `breadslicer-0.0.3/src/opinionated/templates/src/{{project_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `breadslicer-0.0.2/PKG-INFO` & `breadslicer-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breadslicer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Commandline utililty to create python projects from templates
 Home-page: https://gitlab.com/mindsweeper/open-source/breadslicer
 Author: Morten Rasmussen
 Author-email: netrom1337@gmail.com
 Requires-Python: >=3.10.7,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

