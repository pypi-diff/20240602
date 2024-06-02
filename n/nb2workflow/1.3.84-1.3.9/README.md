# Comparing `tmp/nb2workflow-1.3.84.tar.gz` & `tmp/nb2workflow-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb2workflow-1.3.84.tar", last modified: Sun Jun  2 16:57:08 2024, max compression
+gzip compressed data, was "nb2workflow-1.3.9.tar", last modified: Mon Nov 29 16:12:34 2021, max compression
```

## Comparing `nb2workflow-1.3.84.tar` & `nb2workflow-1.3.9.tar`

### file list

```diff
@@ -1,57 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:08.148559 nb2workflow-1.3.84/
--rw-r--r--   0 runner    (1001) docker     (127)    34951 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-06-02 16:57:08.148559 nb2workflow-1.3.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:08.144559 nb2workflow-1.3.84/nb2workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23249 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28206 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/health.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/logging_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/logstash.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    40255 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/nbadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/semantics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)    28382 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:08.144559 nb2workflow-1.3.84/nb2workflow/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/templates/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/templates/buildjob.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/templates/deployment.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/templates/dockerfile_cm.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/templates/pvc.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/templates/service.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/url_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/nb2workflow/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:08.148559 nb2workflow-1.3.84/nb2workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 16:57:08.000000 nb2workflow-1.3.84/nb2workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-02 16:57:08.152559 nb2workflow-1.3.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-06-02 16:57:02.000000 nb2workflow-1.3.84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:08.148559 nb2workflow-1.3.84/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_nbadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_semantic_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-06-02 16:56:57.000000 nb2workflow-1.3.84/tests/test_workflows.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.528756 nb2workflow-1.3.9/.github/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.528756 nb2workflow-1.3.9/.github/workflows/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1508 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/.github/workflows/python-package.yml
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      307 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/.gitignore
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      554 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/Dockerfile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    34951 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/LICENSE
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      204 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/MANIFEST
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      399 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/Makefile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      499 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      660 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/Pipfile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1069 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/README.md
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/TODO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        6 2021-11-29 16:12:31.000000 nb2workflow-1.3.9/VERSION
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/docs/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      608 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/docs/Makefile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5129 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/docs/conf.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      449 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/docs/index.rst
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/nb2workflow/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      149 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/__init__.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     7158 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/container.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5227 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/cwl.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1585 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/health.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1459 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/logstash.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       72 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/model.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    23465 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/nbadapter.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     4125 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/ontology.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      872 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/publish.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      310 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/schedule.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    25401 2021-11-29 15:39:20.000000 nb2workflow-1.3.9/nb2workflow/service.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5350 2021-11-29 15:40:28.000000 nb2workflow-1.3.9/nb2workflow/workflows.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/nb2workflow.egg-info/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      499 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      865 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      330 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/entry_points.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-29 14:42:53.000000 nb2workflow-1.3.9/nb2workflow.egg-info/not-zip-safe
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      276 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/requires.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       12 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/top_level.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      355 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/requirements.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      489 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/setup.cfg
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2120 2021-11-29 16:12:31.000000 nb2workflow-1.3.9/setup.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/tests/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3408 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/conftest.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      446 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_cwl.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3904 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_nbadapter.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      665 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_ontology.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1385 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_run.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3273 2021-11-29 14:24:34.000000 nb2workflow-1.3.9/tests/test_service.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2574 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_workflows.py
```

### Comparing `nb2workflow-1.3.84/LICENSE` & `nb2workflow-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.84/nb2workflow/container.py` & `nb2workflow-1.3.9/nb2workflow/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,26 +45,24 @@
 
     dockerfile = []
 
     dockerfile.append("FROM {}".format(from_image))
     dockerfile.append("ARG REPO_PATH=./{}".format(rel_repo_path))
 
     pipconf = os.path.join(repo_path, 'pip.conf')
-    logger.info("using pipconf %s", pipconf)
+    logger.info("using %s", pipconf)
     if os.path.exists(pipconf):
         dockerfile.append("ENV PIP_CONFIG_FILE=/etc/pip/pip.conf")
         dockerfile.append("ADD $REPO_PATH/pip.conf /etc/pip/pip.conf")
 
     dockerfile.append("ADD $REPO_PATH/requirements.txt /requirements.txt")
-    dockerfile.append("ADD $REPO_PATH/environment.yml /environment.yml")
     dockerfile.append("RUN {} pip install --upgrade pip".format(runprefix))
-   
-    dockerfile.append(('RUN {} conda env update -f /environment.yml && '
-                       'pip install -r /requirements.txt').format(runprefix))
- 
+    # ,repo_hash))
+    dockerfile.append(
+        "RUN {} pip install -r /requirements.txt --upgrade".format(runprefix))
     dockerfile.append("ADD $REPO_PATH /repo")
     dockerfile.append(
         "RUN {} touch /repo-hash-{}; pip install -r /repo/requirements.txt --upgrade".format(runprefix, repo_hash))
     dockerfile.append("RUN useradd -ms /bin/bash oda")
 
     if nb2w_path is None:
         dockerfile.append(
@@ -76,18 +74,16 @@
         dockerfile.append(
             "RUN {} cd /nb2workflow; pip install .".format(runprefix))
 
     dockerfile.append("USER oda")
     dockerfile.append("WORKDIR /workdir")
 
     if service:
-        logger.info('service mode')
         dockerfile.append("ENTRYPOINT nb2service /repo/ --host 0.0.0.0")
     else:
-        logger.info('not service mode')
         dockerfile.append('ENTRYPOINT []')
         #dockerfile.append('ENTRYPOINT ["bash"]' )
         #dockerfile.append('ENTRYPOINT ["nbrun", "/repo/"]' )
 
     open(os.path.join(tempdir, "Dockerfile"), "w").write(
         ("\n".join(dockerfile))+"\n")
 
@@ -127,15 +123,15 @@
                         type=str, default="python:3.6")
     parser.add_argument('--tag-image', metavar='TAG', type=str, default="")
     parser.add_argument('--host', metavar='host',
                         type=str, default="127.0.0.1")
     parser.add_argument('--port', metavar='port', type=int, default=9191)
     parser.add_argument('--nb2wrev', metavar='TAG', type=str, default="master")
     parser.add_argument('--nb2wpath', metavar='PATH', type=str)
-    parser.add_argument('--volume', metavar='mount:mount', type=str, nargs="*", default=[])
+    parser.add_argument('--volume', metavar='mount:mount', type=str, nargs="*")
     parser.add_argument('--docker-run-prefix',  type=str, default="")
     parser.add_argument('--store-dockerfile',
                         metavar='location', type=str, default=None)
     parser.add_argument('--docker-command', type=str, default=None)
     parser.add_argument('--entrypoint', type=str, default=None)
 
     args = parser.parse_args()
```

### Comparing `nb2workflow-1.3.84/nb2workflow/cwl.py` & `nb2workflow-1.3.9/nb2workflow/cwl.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.84/nb2workflow/health.py` & `nb2workflow-1.3.9/nb2workflow/health.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.84/nb2workflow/logstash.py` & `nb2workflow-1.3.9/nb2workflow/logstash.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,33 +17,38 @@
         else:
             items.append((new_key, v))
     return dict(items)
 
 
 class LogStasher:
     def __init__(self, url=None):
-        self.url = url
+        if url is None:
+            self.url = os.environ.get("LOGSTASH_ENTRYPOINT", open("/cdci-resources/logstash-entrypoint").read().strip())
+        else:
+            self.url = url
 
-        if self.url is None:
-            self.url = os.environ.get("LOGSTASH_ENTRYPOINT", None)
-            
         self.context = {}
 
     def set_context(self, c):
         self.context = c
     
     def log(self, msg):
-        if self.url is not None:
-            HOST, PORT = self.url.split(":")
-            PORT = int(PORT)
-
-            msg = flatten(dict(list(self.context.items()) + list(msg.items())))
+        HOST, PORT = self.url.split(":")
+        PORT = int(PORT)
+
+        msg = flatten(dict(list(self.context.items()) + list(msg.items())))
+
+
+        try:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        except Exception as e:
+            print("[ERROR] %s\n" % repr(e)) 
+            
 
+        try:
+            sock.connect((HOST, PORT))
+        except Exception as e:
+            print("[ERROR] %s\n" % repr(e)) 
 
-            try:
-                sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-                sock.connect((HOST, PORT))
-                sock.send(json.dumps(msg).encode())
-                sock.close()
-            except Exception as e:
-                print("[ERROR] %s\n" % repr(e)) 
+        sock.send(json.dumps(msg).encode())
 
+        sock.close()
```

### Comparing `nb2workflow-1.3.84/nb2workflow/publish.py` & `nb2workflow-1.3.9/nb2workflow/publish.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.84/nb2workflow/service.py` & `nb2workflow-1.3.9/nb2workflow/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,10 @@
 from __future__ import print_function
-import pickle
 import re
-
-from werkzeug.routing import RequestRedirect
-
-try:
-    from werkzeug.exceptions import MethodNotAllowed, NotFound
-except ImportError:
-    from werkzeug.routing import MethodNotAllowed, NotFound
-
-
+from werkzeug.routing import RequestRedirect, MethodNotAllowed, NotFound
 import queue
 from nb2workflow import ontology, publish, schedule
 from nb2workflow.nbadapter import NotebookAdapter, find_notebooks, PapermillWorkflowIncomplete
 
 import os
 import json
 import glob
@@ -25,25 +16,25 @@
 import hashlib
 import datetime
 import tempfile
 import nbformat
 import yaml
 
 from io import BytesIO
-from bs4 import BeautifulSoup
 
 
 from flask import Flask, make_response, jsonify, request, url_for, send_file, Response
+from flask.json import JSONEncoder
 from flask_caching import Cache
 from flask_cors import CORS
 
-from flasgger import LazyString, Swagger, swag_from
+from flasgger import LazyJSONEncoder, LazyString, Swagger, swag_from
+
 
 from nb2workflow.workflows import serialize_workflow_exception
-from nb2workflow.json import CustomJSONEncoder
 
 import threading
 
 verify_tls = False
 
 
 logger = logging.getLogger('nb2workflow.service')
@@ -66,14 +57,27 @@
 
         scheme = environ.get('HTTP_X_SCHEME', '')
         if scheme:
             environ['wsgi.url_scheme'] = scheme
         return self.app(environ, start_response)
 
 
+class CustomJSONEncoder(LazyJSONEncoder):
+    def default(self, obj, *args, **kwargs):
+        try:
+            if isinstance(obj, type):
+                return dict(type_object=repr(obj))
+            iterable = iter(obj)
+        except TypeError:
+            pass
+        else:
+            return list(iterable)
+        return JSONEncoder.default(self, obj)
+
+
 cache = Cache(config={'CACHE_TYPE': 'simple'})
 
 
 def create_app():
     app = Flask(__name__)
 
     template = {
@@ -91,38 +95,42 @@
             "termsOfService": "http://me.com/terms",
             "version": "0.0.1"
         }
     }
     swagger = Swagger(app, template=template)
     app.wsgi_app = ReverseProxied(app.wsgi_app)
     app.json_encoder = CustomJSONEncoder
-    app.config["JSON_SORT_KEYS"] = False
-    cache.init_app(app, config={'CACHE_TYPE': 'SimpleCache'})
+    cache.init_app(app, config={'CACHE_TYPE': 'simple'})
 
 
 #    CORS(app)
     return app
 
 
 app = create_app()
 
 app.async_workflows = dict()
-app.async_workflow_jobdirs = dict()
 app.started_at = datetime.datetime.now()
 
 
 @app.after_request
 def after_request(response):
     response.headers.add('Access-Control-Allow-Origin', '*')
     response.headers.add('Access-Control-Allow-Headers',
                          'Content-Type,Authorization')
     response.headers.add('Access-Control-Allow-Methods',
                          'GET,PUT,POST,DELETE,OPTIONS')
     return response
 
+
+def make_key():
+    """Make a key that includes GET parameters."""
+    return request.full_path
+
+
 class AsyncWorker(threading.Thread):
     def __init__(self, worker_id):
         self.worker_id = worker_id
         super(AsyncWorker, self).__init__()
 
     def run(self):
         while True:
@@ -131,26 +139,19 @@
 
     def run_one(self):
         logger.info("worker_id %s", self.worker_id)
         async_workflow = async_queue.get(block=True)
         async_workflow.run()
 
 class AsyncWorkflow:
-    def __init__(self, key, target, params, context={}):
+    def __init__(self, key, target, params, callback=None):
         self.key = key
         self.target = target
         self.params = params
-        self.context = context
-
-        logger.info("%s initializing callback %s", self, self.callback)
-
-    @property
-    def callback(self):
-        return self.context.get('callback', None)
-
+        self.callback = callback
 
     def run(self):
         try:
             self._run()
         except Exception as e:
             logger.error("run failed unexplicably: %s", repr(e))
             app.async_workflows[self.key] = dict(
@@ -172,39 +173,32 @@
     def _run(self):
         if self.blocked_until > time.time():
             logger.info("workflow still blocked, waiting %i",
                         self.blocked_until - time.time())
             async_queue.put(self)
             app.async_workflows[self.key] = 'submitted'
             return
-       
-        template_nba = app.notebook_adapters.get(self.target)
-        nba = NotebookAdapter(template_nba.notebook_fn, tempdir_cache=app.async_workflow_jobdirs,
-                              n_download_max_tries=template_nba.n_download_max_tries,
-                              download_retry_sleep_s=template_nba.download_retry_sleep_s,
-                              max_download_size=template_nba.max_download_size)
-        
+
         app.async_workflows[self.key] = 'started'
-        self.perform_callback(action='progress')
+
+        template_nba = app.notebook_adapters.get(self.target)
+
+        nba = NotebookAdapter(template_nba.notebook_fn)
 
         try:
-            thread_id = threading.get_ident()
-            process_id = os.getpid()
-            logger.info(f'nba.execute thread id: {thread_id} ; process id: {process_id}')
-            exceptions = nba.execute(self.params['request_parameters'], context=self.context, tmpdir_key=self.key)
+            exceptions = nba.execute(self.params['request_parameters'])
         except PapermillWorkflowIncomplete as e:
             logger.info("found incomplete workflow: %s, rescheduling", repr(e))
 
             self.note("rescheduled")
 
             self.blocked_until = time.time() + 10
 
             async_queue.put(self)
-            app.async_workflows[self.key] = 'submitted'            
-
+            app.async_workflows[self.key] = 'submitted'
             return
 
         logger.info("exceptions: %s", repr(exceptions))
 
         if len(exceptions) > 0:
             output = 'incomplete'
             logger.error("exceptions: %s", repr(exceptions))
@@ -225,67 +219,57 @@
                 except Exception as e:
                     logger.debug(
                         "output notebook incomplte or does not exist %s attempts left: %s", e, nretry)
 
                 nretry -= 1
                 time.sleep(1)
 
-        logger.debug("output: %s", output)
+        logger.error("output: %s", output)
 
         logger.info("updating key %s", self.key)
         app.async_workflows[self.key] = dict(output=output, exceptions=list(
             map(serialize_workflow_exception, exceptions)), jobdir=nba.tmpdir)
 
         self.perform_callback()
 
-    def perform_callback(self, action='done'):
+    def perform_callback(self):
         if self.callback is None:
-            logger.info('no callback registered, skipping')
+            logger.debug('no callback registered, skipping')
             return
 
-        logger.info('will perform callback: %s', self.callback)
-
-
         result = app.async_workflows[self.key]
 
         callback_payload = dict(
-            action=action
+            status='done'
         )
         
         if re.match('^file://', self.callback):
             with open(self.callback.replace('file://', ''), "w") as f:
                  json.dump(callback_payload, f)
-            logger.info('stored callback in a file %s', self.callback)
 
         elif re.match('^https?://', self.callback):
-            r = requests.get(self.callback, params=callback_payload)
-            logger.info('callback %s returns %s : %s', self.callback, r, r.text)
+            requests.get(self.callback, params=callback_payload)
         
         else:
             raise NotImplementedError
 
 
 def workflow(target, background=False, async_request=False):
     issues = []
 
     async_request = request.args.get('_async_request', async_request)
     async_request_callback = request.args.get('_async_request_callback', None)
-    token = request.args.get("_token", None)
-    context = dict(callback=async_request_callback, token=token)
 
     logger.debug("target %s", target)
 
     if not background:
         logger.debug("raw parameters %s", request.args)
 
     template_nba = app.notebook_adapters.get(target)
-    nba = NotebookAdapter(template_nba.notebook_fn,
-                          n_download_max_tries=template_nba.n_download_max_tries,
-                          download_retry_sleep_s=template_nba.download_retry_sleep_s,
-                          max_download_size=template_nba.max_download_size)
+    nba = NotebookAdapter(template_nba.notebook_fn)
 
     if nba is None:
         interpreted_parameters = None
         issues.append("target not known: %s; available targets: %s" %
                       (target, app.notebook_adapters.keys()))
     else:
         if not background:
@@ -295,55 +279,39 @@
             interpreted_parameters = dict(request_parameters=[])
 
     logger.debug("interpreted parameters %s", interpreted_parameters)
 
     # async
     if async_request:
         key = hashlib.sha224(json.dumps(
-            dict(target=target, params=interpreted_parameters)).encode('utf-8')).hexdigest()
+            dict(target=target, params=interpreted_parameters, callback=async_request_callback)).encode('utf-8')).hexdigest()
 
         value = app.async_workflows.get(key, None)
 
         print('cache key/value', key, value)
 
         if value is None:
-            async_task = AsyncWorkflow(key=key,
-                                       target=target,
-                                       params=interpreted_parameters,
-                                       context=context
-                                       )
+            async_task = AsyncWorkflow(
+                key=key, target=target, params=interpreted_parameters, callback=async_request_callback)
 
-            app.async_workflows[key] = 'submitted'
             async_queue.put(async_task)
 
-            return make_response(jsonify(workflow_status="submitted",
-                                         comment="task created"),
-                                 201)
-
-        elif value == 'submitted':
-            return make_response(jsonify(workflow_status=value,
-                                         comment="task is "+value),
-                                 201)
-
-        elif value == 'started':
-            return make_response(jsonify(workflow_status=value,
-                                         comment="task is "+value,
-                                         jobdir=app.async_workflow_jobdirs.get(key)),
-                                 201)
+            app.async_workflows[key] = 'submitted'
+            return make_response(jsonify(workflow_status="submitted", comment="task created"), 201)
+
+        elif value in ['started', 'submitted']:
+            return make_response(jsonify(workflow_status=value, comment="task is "+value), 201)
 
         else:
-            return make_response(jsonify(workflow_status="done",
-                                         data=value,
-                                         comment=""),
-                                 200)
+            return make_response(jsonify(workflow_status="done", data=value, comment=""), 200)
 
     if len(issues) > 0:
         return make_response(jsonify(issues=issues), 400)
     else:
-        exceptions = nba.execute(interpreted_parameters['request_parameters'], context=context)
+        exceptions = nba.execute(interpreted_parameters['request_parameters'])
 
         nretry = 10
         while nretry > 0:
             try:
                 output = nba.extract_output()
                 if len(output) == 0:
                     logger.debug(
@@ -457,28 +425,22 @@
             if isinstance(rv, tuple) and isinstance(rv[0], Response) and rv[1] != 200:
                 logger.info("NOT caching response %s", rv[1])
                 return False
             elif isinstance(rv, Response) and rv.status != 200:
                 logger.info("NOT caching response %s", rv)
                 return False
             else:
-                logger.info("should cache response %s", rv)                
-                try:
-                    pickle.dumps(rv)
-                except pickle.PicklingError as e:
-                    logger.info("the response can not be pickled and cached %s", e)
-                    return False
-
+                logger.info("caching response %s", rv)
                 return True
 
         cache_timeout = nba.get_system_parameter_value('cache_timeout', 0)
         try:
             app.route('/api/v1.0/get/'+target, methods=['GET'], endpoint=endpoint)(
                 swag_from(target_specs)(
-                    cache.cached(timeout=cache_timeout, response_filter=response_filter, query_string=True)(
+                    cache.cached(timeout=cache_timeout, key_prefix=make_key, response_filter=response_filter, query_string=True)(
                         funcg(target)
                     )))
         except AssertionError as e:
             logger.warning("unable to add route: %s, ignoring the endpoint", e)
             continue
 
         schedule_interval = nba.get_system_parameter_value(
@@ -497,18 +459,18 @@
 # list input -> output function signatures and identities
 
 
 @app.route('/api/v1.0/options', methods=['GET'])
 def workflow_options():
     return jsonify(dict([
         (
-            target,
-            dict(output=nba.extract_output_declarations(),
-                    parameters=nba.extract_parameters()),
-            )
+                        target,
+                        dict(output=nba.extract_output_declarations(),
+                             parameters=nba.extract_parameters()),
+                        )
         for target, nba in app.notebook_adapters.items()
     ]))
 
 
 @app.route('/api/v1.0/get-<mode>/<target>/<filename>', methods=['GET'])
 def workflow_filename(mode, target, filename):
 
@@ -627,15 +589,14 @@
 
 
 @app.route('/test')
 def test():
     results = {}
     expecting = []
 
-    #TODO: use generalized testing
     for template_nba in app.notebook_adapters.values():
         if template_nba.name.startswith('test_'):
             key = template_nba.name
 
             if key in app.async_workflows:
                 print("found", app.async_workflows[key])
 
@@ -676,20 +637,15 @@
 
 
 @app.route('/')
 def root():
     issues = []
 
     if len(issues) == 0:
-        return {
-                    "message": "all is ok!",
-                    "version": os.getenv("ODA_WORKFLOW_VERSION"),
-                    "last_author": os.getenv("ODA_WORKFLOW_LAST_AUTHOR"),
-                    "last_changed": os.getenv("ODA_WORKFLOW_LAST_CHANGED")                    
-            }
+        return "all is ok!"
     else:
         return make_response(jsonify(issues=issues), 500)
 
 
 def main():
     import argparse
 
@@ -704,15 +660,14 @@
                         type=str, default=None)
     parser.add_argument(
         '--publish-as', metavar='published url', type=str, default=None)
     parser.add_argument(
         '--profile', metavar='service profile', type=str, default="oda")
     parser.add_argument('--debug', action="store_true")
     parser.add_argument('--one-shot', metavar='workflow', type=str)
-    parser.add_argument('--pattern', type=str, default=r'.*')
 
     args = parser.parse_args()
 
     handler = logging.StreamHandler()
     handler.setLevel(logging.INFO)
 
     root = logging.getLogger()
@@ -726,15 +681,15 @@
     if args.debug:
         root.setLevel(logging.DEBUG)
         handler.setLevel(logging.DEBUG)
     else:
         root.setLevel(logging.INFO)
         handler.setLevel(logging.INFO)
 
-    app.notebook_adapters = find_notebooks(args.notebook, pattern=args.pattern)
+    app.notebook_adapters = find_notebooks(args.notebook)
     setup_routes(app)
     app.service_semantic_signature = ontology.service_semantic_signature(
         app.notebook_adapters)
 
     if args.publish:
         logger.info("publishing to %s", args.publish)
 
@@ -743,18 +698,14 @@
             publish_host, publish_port = ":".join(s[:-1]), int(s[-1])
         else:
             publish_host, publish_port = args.host, args.port
 
         for nba_name, nba in app.notebook_adapters.items():
             publish.publish(args.publish, nba_name, publish_host, publish_port)
 
-    thread_id = threading.get_ident()
-    process_id = os.getpid()
-    logger.info(f'service main thread id: {thread_id} ; process id: {process_id}')
-
   #  for rule in app.url_map.iter_rules():
  #       logger.debug("==>> %s %s %s %s",rule,rule.endpoint,rule.__class__,rule.__dict__)
 
     for worker_i in range(args.async_workers):
         async_worker = AsyncWorker('default-%i' % worker_i)
         async_worker.start()
 
@@ -850,32 +801,21 @@
 
 
 @app.route('/trace/<string:job>/<string:func>')
 def trace_get_func(job, func):
     if func == "custom.css":
         return ""
 
-    include_glued_output = request.args.get('include_glued_output', True) == 'True'
-
     from nbconvert.exporters import HTMLExporter
     exporter = HTMLExporter()
 
     fn = os.path.join(tempfile.gettempdir(), job, func+"_output.ipynb")
 
     output, resources = exporter.from_filename(fn)
 
-    if not include_glued_output:
-        logger.info("include_glued_output arg passed")
-        soup = BeautifulSoup(output, 'html.parser')
-        div_glued_output = soup.find('div', {'class': 'celltag_injected-gather-outputs'})
-        if div_glued_output is not None:
-            div_glued_output.decompose()
-        output = str(soup)
-        logger.info("div element removed form html")
-
     return output
 
 
 @app.route('/clear-cache')
 def clear_cache():
     n_entries = None
     try:
```

### Comparing `nb2workflow-1.3.84/nb2workflow/workflows.py` & `nb2workflow-1.3.9/nb2workflow/workflows.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 import json
 import os
 import requests
 import time
 import datetime
 import logging
 from collections import OrderedDict
-from . import logstash
-from .sentry import sentry
 
 from diskcache import Cache
 
 from nb2workflow import nbadapter
 
-cache = Cache('.nb2workflow/cache')
+cache = Cache('data/default-cache')
 enable_cache = False
 
-logstasher = logstash.LogStasher()
+try:
+    from nb2workflow import logstash
+    logstasher = logstash.LogStasher()
+except Exception as e:
+    import logging
+    logging.warning("unable to setup logstash %s",repr(e))
+
+    logstasher = None
+
+try:
+    import sentry_sdk
+    sentry_sdk.init(os.environ.get("SENTRY_URI", open("/cdci-resources/sentry-uri").read().strip()))
+except ImportError:
+    sentry_sdk = None
+except Exception as e:
+    import logging
+    logging.debug("big problem with sentry: %s",repr(e))
+    sentry_sdk = None
+
 
 class WorkflowException(Exception):
     pass
 
 def serialize_workflow_exception(e):
     try:
         return dict(
                     ename = e[0].ename,
                     evalue = e[0].evalue,
                     edump = e[1][0],
                 )
-    except (TypeError, AttributeError):
+    except TypeError:
         return dict(
                     ename = repr(e),
                     evalue = "",
                     edump = repr(e)
                 )
 
     
@@ -55,16 +71,17 @@
     ntries = kwargs.pop('_ntries', 30)
     async_request = kwargs.pop('_async_request', True)
     cached = kwargs.pop('_cached', True)
 
     print("async_request is not used here, but is set to", async_request)
 
 
-    logstasher.set_context(dict(router=router, args=args, kwargs=kwargs))
-    logstasher.log(dict(event='starting'))
+    if logstasher:
+        logstasher.set_context(dict(router=router, args=args, kwargs=kwargs))
+        logstasher.log(dict(event='starting'))
 
     if cached and enable_cache and key in cache:
         v = cache.get(key)
         print("restored from cache, key:", key)
         print("restored from cache, value:", v)
 
         if v == {} or v is None:
@@ -143,29 +160,31 @@
 
             except Exception as e:
                 print("problem from service", repr(e))
 
                 logstasher.log(dict(event='problem evaluating',exception=repr(e)))
                 
                 if ntries <= 1:
-                    sentry.capture_exception(e)
+                    if sentry_sdk:
+                        sentry_sdk.capture_exception()
                     raise
 
                 time.sleep(5)
 
                 ntries -= 1
 
         if 'output' not in result:
             result = dict(output=result)
 
                 #raise
     else:
         raise NotImplementedError
 
 
-    logstasher.log(dict(event='done'))
+    if logstasher:
+        logstasher.log(dict(event='done'))
 
     cache.set(key, result)
     print("stored to cache", key)
 
     return result
```

### Comparing `nb2workflow-1.3.84/nb2workflow.egg-info/SOURCES.txt` & `nb2workflow-1.3.9/nb2workflow.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,42 @@
+.gitignore
+Dockerfile
 LICENSE
+MANIFEST
+Makefile
+Pipfile
 README.md
+TODO
+VERSION
+requirements.txt
 setup.cfg
 setup.py
+.github/workflows/python-package.yml
+docs/Makefile
+docs/conf.py
+docs/index.rst
 nb2workflow/__init__.py
 nb2workflow/container.py
 nb2workflow/cwl.py
-nb2workflow/deploy.py
-nb2workflow/galaxy.py
 nb2workflow/health.py
-nb2workflow/json.py
-nb2workflow/logging_setup.py
 nb2workflow/logstash.py
 nb2workflow/model.py
 nb2workflow/nbadapter.py
 nb2workflow/ontology.py
 nb2workflow/publish.py
 nb2workflow/schedule.py
-nb2workflow/semantics.py
-nb2workflow/sentry.py
 nb2workflow/service.py
-nb2workflow/testing.py
-nb2workflow/url_helper.py
-nb2workflow/validate.py
 nb2workflow/workflows.py
 nb2workflow.egg-info/PKG-INFO
 nb2workflow.egg-info/SOURCES.txt
 nb2workflow.egg-info/dependency_links.txt
 nb2workflow.egg-info/entry_points.txt
 nb2workflow.egg-info/not-zip-safe
 nb2workflow.egg-info/requires.txt
 nb2workflow.egg-info/top_level.txt
-nb2workflow/templates/Dockerfile.jinja
-nb2workflow/templates/buildjob.yaml.jinja
-nb2workflow/templates/deployment.yaml.jinja
-nb2workflow/templates/dockerfile_cm.yaml.jinja
-nb2workflow/templates/pvc.yaml.jinja
-nb2workflow/templates/service.yaml.jinja
-tests/test_callback.py
+tests/conftest.py
 tests/test_cwl.py
-tests/test_deploy.py
-tests/test_input_types.py
-tests/test_json.py
 tests/test_nbadapter.py
 tests/test_ontology.py
 tests/test_run.py
-tests/test_semantic_comment.py
 tests/test_service.py
-tests/test_testing.py
-tests/test_token.py
 tests/test_workflows.py
```

### Comparing `nb2workflow-1.3.84/setup.py` & `nb2workflow-1.3.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,111 +2,83 @@
 import sys
 
 setup_requires = ['setuptools >= 30.3.0', 'setuptools-git-version']
 if {'pytest', 'test', 'ptr'}.intersection(sys.argv):
     setup_requires.append('pytest-runner')
 
 setup(name='nb2workflow',
-      version = '1.3.84',
+      version = '1.3.9',
       description='convert notebook to workflow',
       author='Volodymyr Savchenko',
       author_email='contact@volodymyrsavchenko.com',
       license='GPLv3',
       packages=['nb2workflow'],
-      package_data={'nb2workflow': ['templates/*.jinja']},
       zip_safe=False,
 
-      python_requires='>=3.9,<3.12',
-
       entry_points={
           'console_scripts': [
             'nb2service=nb2workflow.service:main',
             'nb2worker=nb2workflow.container:main',
             'nb2workflow-version=nb2workflow:version',
             'nb2cwl=nb2workflow.cwl:main',
             'nb2rdf=nb2workflow.ontology:main',
-            'nb2deploy=nb2workflow.deploy:main',
             'nbrun=nb2workflow.nbadapter:main',
             'nbinspect=nb2workflow.nbadapter:main_inspect',
             'nbreduce=nb2workflow.nbadapter:main_reduce',
-            'nb2galaxy=nb2workflow.galaxy:main',
             ]
       },
       
       extras_require={
         "service":[
-            'flask==2.0.3',
+            'flask',
             'pytest-flask',
-            'flask-caching', 
+            'flask-caching', #'Flask-Caching',
             'flask-cors',
             'flasgger',
             'python-consul',
             'apscheduler',
-            'beautifulsoup4'
         ],
         "rdf":[
             'rdflib',
             'owlready2==0.11',
-            'oda-knowledge-base',
         ],
         "cwl":[
             "cwlgen",
         ],
         "docker":[
             'docker',
             'checksumdir',
-            'Jinja2'
         ],
         "domains":[
             'numpy',
             'astropy',
             'pandas',
-            'matplotlib'
-        ],
-        "mmoda":[
-        ],
-        "k8s":[
-            'kubernetes',
-            'Jinja2'
         ],
-        'galaxy':[
-            'ensureconda',
-            'bibtexparser >= 2.0.0b3',
-            'pypandoc_binary',
-            'black',
-            'isort',
-            'autoflake'
-        ]
       },
 
       tests_require=[
         'pytest',
         'pytest-xprocess',
         'matplotlib',
         'cwl-runner',
-        'psutil'
       ],
 
       install_requires=[
         'papermill',
         'ipykernel',
         'nbconvert', 
         'psutil',
         'diskcache',
         'requests',
         'pyyaml',
-        'scrapbook', 
-        'werkzeug==2.0.3',
-        'validators==0.28.3',
-        'sentry_sdk',
-        'rdflib',
-        'GitPython',
-        'oda_api'
+        'nteract-scrapbook', 
       ],
 
 
       url = 'https://github.com/volodymyrss/nb2workflow',
       download_url = 'https://github.com/volodymyrss/nb2workflow/archive/1.0.1.tar.gz',
       keywords = ['jupyter', 'docker'],
       classifiers = [],
       setup_requires=setup_requires)
 
+
+
```

### Comparing `nb2workflow-1.3.84/tests/test_nbadapter.py` & `nb2workflow-1.3.9/tests/test_nbadapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,25 +35,25 @@
 
     nba = NotebookAdapter(fn)
     parameters = nba.extract_parameters()
 
     for k, v in parameters.items():
         print("\033[31m", k, ":", v, "\033[0m")
 
-    assert len(parameters) == 6
+    assert len(parameters) == 5
 
     assert 'comment' in parameters['scwid']
     assert parameters['scwid']['owl_type'] == "http://odahub.io/ontology/integral#ScWID"
 
-    assert parameters['enabled']['owl_type'] == "http://odahub.io/ontology#Boolean"
+    assert parameters['enabled']['owl_type'] == "http://www.w3.org/2001/XMLSchema#bool"
 
     outputs = nba.extract_output_declarations()
     print("outputs", outputs)
 
-    assert len(outputs) == 4
+    assert len(outputs) == 3
 
     if os.path.exists(nba.output_notebook_fn):
         os.remove(nba.output_notebook_fn)
 
     if os.path.exists(nba.preproc_notebook_fn):
         os.remove(nba.preproc_notebook_fn)
 
@@ -63,93 +63,49 @@
 
     if morph_notebook == "mimick_convert_minor_version":
         assert 'will attempt to convert, but expect other warnings' in caplog.text
 
         os.remove(fn)
 
     print(output)
-    assert len(output) == 6
+    assert len(output) == 4
 
     assert 'spectrum' in output
 
-def test_find_notebooks(caplog):
-    from nb2workflow.nbadapter import find_notebooks, NotebookAdapter
-    testfiles_path = os.path.join(os.path.dirname(__file__), 'testfiles')
-    nb_dir = testfiles_path
-    single_nb = os.path.join(testfiles_path, 'lightcurve.ipynb')
-    
-    nbas = find_notebooks(single_nb)
-    assert len(nbas) == 1
-    
-    nbas = find_notebooks(single_nb, pattern=r'.*bool')
-    assert len(nbas) == 1
-    assert 'Ignoring pattern.' in caplog.text
-    
-    nbas = find_notebooks(nb_dir)
-    assert len(nbas) == 7
-    
-    nbas = find_notebooks(nb_dir, pattern=r'.*bool')
-    assert len(nbas) == 1
-    
 
 def test_nbadapter_repo(test_notebook_repo):
-    from nb2workflow.nbadapter import NotebookAdapter, find_notebooks, validate_oda_dispatcher
+    from nb2workflow.nbadapter import NotebookAdapter, find_notebooks
 
     nbas = find_notebooks(test_notebook_repo)
 
     assert len(nbas) == 1
 
     for nba_name, nba in nbas.items():
         print("notebook", nba_name)
 
         parameters = nba.extract_parameters()
 
         print(parameters)
-        assert len(parameters) == 6
+        assert len(parameters) == 5
 
         if os.path.exists(nba.output_notebook_fn):
             os.remove(nba.output_notebook_fn)
 
         if os.path.exists(nba.preproc_notebook_fn):
             os.remove(nba.preproc_notebook_fn)
 
         nba.execute(dict())
 
         output = nba.extract_output()
 
         print(output)
 
-        assert len(output) == 6
+        assert len(output) == 4
         assert 'spectrum' in output
 
-        validate_oda_dispatcher(nba)
-
-@pytest.mark.skip(reason="Reproducing this condition in the test is difficult")
-def test_nbadapter_lfs_repo(test_notebook_lfs_repo):
-    from nb2workflow.nbadapter import NotebookAdapter, find_notebooks, validate_oda_dispatcher
-
-    nbas = find_notebooks(test_notebook_lfs_repo)
-
-    assert len(nbas) >= 1
-
-    for nba_name, nba in nbas.items():
-        print("notebook", nba_name)
-
-        if os.path.exists(nba.output_notebook_fn):
-            os.remove(nba.output_notebook_fn)
-
-        if os.path.exists(nba.preproc_notebook_fn):
-            os.remove(nba.preproc_notebook_fn)
-
-        try:
-            nba.execute(dict())
-            assert False, 'nba.execute is expected to fail'
-        except Exception as ex:
-            assert ex.message == "git-lfs is not initialized"
-        break
 
 def test_nbreduce(test_notebook):
     from nb2workflow.nbadapter import NotebookAdapter, nbreduce, setup_logging
 
     setup_logging()
 
     nba = NotebookAdapter(test_notebook)
@@ -160,15 +116,15 @@
     if os.path.exists(nba.preproc_notebook_fn):
         os.remove(nba.preproc_notebook_fn)
 
     nba.execute(dict())
 
     output = nba.extract_output()
 
-    assert len(output) == 6
+    assert len(output) == 4
 
     assert 'spectrum' in output
 
     print("will reduce", nba.output_notebook_fn)
 
     nbsize_b = os.path.getsize(nba.output_notebook_fn)
```

### Comparing `nb2workflow-1.3.84/tests/test_workflows.py` & `nb2workflow-1.3.9/tests/test_workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     
     from nb2workflow import workflows
 
     result = workflows.evaluate("localfile", test_notebook_repo, "workflow-notebook")
 
     print(result)
     assert result['output']
-    assert len(result['output']) == 6
+    assert len(result['output']) == 4
     assert result['exceptions'] == []
 
     assert 'spectrum' in result['output']
 
 @pytest.mark.xfail
 def test_workflow_exception_localfile(test_notebook):
```

