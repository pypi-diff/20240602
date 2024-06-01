# Comparing `tmp/gitlab_projects_issues-1.0.1.tar.gz` & `tmp/gitlab_projects_issues-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_issues-1.0.1.tar", last modified: Sat Jun  1 21:42:09 2024, max compression
+gzip compressed data, was "gitlab_projects_issues-1.0.2.tar", last modified: Sat Jun  1 22:26:20 2024, max compression
```

## Comparing `gitlab_projects_issues-1.0.1.tar` & `gitlab_projects_issues-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.752916 gitlab_projects_issues-1.0.1/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      714 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    13599 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.752916 gitlab_projects_issues-1.0.1/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7306 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5649 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7306 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.754916 gitlab_projects_issues-1.0.1/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2886 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.755916 gitlab_projects_issues-1.0.1/src/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.756916 gitlab_projects_issues-1.0.1/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9193 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     6171 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.756916 gitlab_projects_issues-1.0.1/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.757916 gitlab_projects_issues-1.0.1/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.758916 gitlab_projects_issues-1.0.1/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/prints/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.758916 gitlab_projects_issues-1.0.1/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.759916 gitlab_projects_issues-1.0.1/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/milestones.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.726417 gitlab_projects_issues-1.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.716417 gitlab_projects_issues-1.0.2/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      714 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    13612 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.716417 gitlab_projects_issues-1.0.2/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-06-01 22:26:20.726417 gitlab_projects_issues-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5649 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.725417 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-06-01 22:26:20.000000 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-06-01 22:26:20.000000 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 22:26:20.000000 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-06-01 22:26:20.000000 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-06-01 22:26:20.000000 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-01 22:26:20.000000 gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.719417 gitlab_projects_issues-1.0.2/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 22:26:20.726417 gitlab_projects_issues-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.719417 gitlab_projects_issues-1.0.2/src/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.720417 gitlab_projects_issues-1.0.2/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9193 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     6171 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.721417 gitlab_projects_issues-1.0.2/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.722417 gitlab_projects_issues-1.0.2/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.723417 gitlab_projects_issues-1.0.2/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.724417 gitlab_projects_issues-1.0.2/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 22:26:20.725417 gitlab_projects_issues-1.0.2/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/types/milestones.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/types/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-06-01 22:26:16.000000 gitlab_projects_issues-1.0.2/src/types/strings.py
```

### Comparing `gitlab_projects_issues-1.0.1/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_issues-1.0.2/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/.chglog/changelog.sh` & `gitlab_projects_issues-1.0.2/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/.chglog/config.yml` & `gitlab_projects_issues-1.0.2/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/.gitlab-ci.yml` & `gitlab_projects_issues-1.0.2/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,16 @@
       docker pull "${REGISTRY_HOST}/${REGISTRY_OWNER}/${REGISTRY_PROJECT}/${image}" || true
       buildah bud -t "${REGISTRY_HOST}/${REGISTRY_OWNER}/${REGISTRY_PROJECT}/${image}" -f - ./dist/ <<-EOF
       FROM ${REGISTRY_HOST}/${REGISTRY_OWNER}/${REGISTRY_PROJECT}/${base}
       COPY ./*.whl /tmp/
       RUN export PIP_DISABLE_PIP_VERSION_CHECK=1 \
        && pip3 install -q --no-cache-dir --upgrade /tmp/*.whl \
        && rm -f /tmp/*.whl
-      ENTRYPOINT ["/bin/sh"]
+      ENTRYPOINT []
+      CMD ["/bin/sh"]
       EOF
       echo ''
       echo " [INFO] Push: ${REGISTRY_HOST}/${REGISTRY_OWNER}/${REGISTRY_PROJECT}/${image}"
       echo ''
       buildah push "${REGISTRY_HOST}/${REGISTRY_OWNER}/${REGISTRY_PROJECT}/${image}" || true
   rules:
     - if: $CI_COMMIT_TAG
```

### Comparing `gitlab_projects_issues-1.0.1/.style.yapf` & `gitlab_projects_issues-1.0.2/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/.vscode/extensions.json` & `gitlab_projects_issues-1.0.2/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/.vscode/settings.json` & `gitlab_projects_issues-1.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/CHANGELOG.md` & `gitlab_projects_issues-1.0.2/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 
-<a name="1.0.1"></a>
-## [1.0.1](https://gitlab.com/AdrianDC/gitlab-projects-issues/compare/0.0.0...1.0.1) (2024-06-01)
+<a name="1.0.2"></a>
+## [1.0.2](https://gitlab.com/AdrianDC/gitlab-projects-issues/compare/1.0.1...1.0.2) (2024-06-02)
 
 ### CI
 
-* **gitlab-ci:** change commit messages to tag name
+* **gitlab-ci:** set '/bin/sh' as 'CMD' rather than 'ENTRYPOINT'
 
 
-<a name="0.0.0"></a>
-## [0.0.0](https://gitlab.com/AdrianDC/gitlab-projects-issues/compare/1.0.0...0.0.0) (2024-06-01)
+<a name="1.0.1"></a>
+## [1.0.1](https://gitlab.com/AdrianDC/gitlab-projects-issues/compare/1.0.0...1.0.1) (2024-06-01)
+
+### CI
+
+* **gitlab-ci:** change commit messages to tag name
 
 ### Documentation
 
 * **chglog:** add 'ci' as 'CI' configuration for 'CHANGELOG.md'
 * **readme:** update 'README.md' for 'gitlab-projects-issues'
```

### Comparing `gitlab_projects_issues-1.0.1/LICENSE` & `gitlab_projects_issues-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/PKG-INFO` & `gitlab_projects_issues-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-issues
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate GitLab project issues and milestones statistics automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-issues
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-issues/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-issues/blob/main/CHANGELOG.md
```

### Comparing `gitlab_projects_issues-1.0.1/README.md` & `gitlab_projects_issues-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/PKG-INFO` & `gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-issues
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate GitLab project issues and milestones statistics automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-issues
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-issues/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-issues/blob/main/CHANGELOG.md
```

### Comparing `gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/SOURCES.txt` & `gitlab_projects_issues-1.0.2/gitlab_projects_issues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/setup.py` & `gitlab_projects_issues-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/cli/entrypoint.py` & `gitlab_projects_issues-1.0.2/src/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/cli/main.py` & `gitlab_projects_issues-1.0.2/src/cli/main.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/features/gitlab.py` & `gitlab_projects_issues-1.0.2/src/features/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/package/bundle.py` & `gitlab_projects_issues-1.0.2/src/package/bundle.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/package/settings.py` & `gitlab_projects_issues-1.0.2/src/package/settings.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/package/updates.py` & `gitlab_projects_issues-1.0.2/src/package/updates.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/package/version.py` & `gitlab_projects_issues-1.0.2/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/prints/boxes.py` & `gitlab_projects_issues-1.0.2/src/prints/boxes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/prints/colors.py` & `gitlab_projects_issues-1.0.2/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/system/platform.py` & `gitlab_projects_issues-1.0.2/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/types/milestones.py` & `gitlab_projects_issues-1.0.2/src/types/milestones.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/types/statistics.py` & `gitlab_projects_issues-1.0.2/src/types/statistics.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.1/src/types/strings.py` & `gitlab_projects_issues-1.0.2/src/types/strings.py`

 * *Files identical despite different names*

