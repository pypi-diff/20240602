# Comparing `tmp/seamm_dashboard-2024.5.24.tar.gz` & `tmp/seamm_dashboard-2024.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_dashboard-2024.5.24.tar", last modified: Fri May 24 17:14:13 2024, max compression
+gzip compressed data, was "seamm_dashboard-2024.6.2.tar", last modified: Sun Jun  2 19:08:13 2024, max compression
```

## Comparing `seamm_dashboard-2024.5.24.tar` & `seamm_dashboard-2024.6.2.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4850 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8236 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2120 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/flask_authorize_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/jwt_patch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      498 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/results_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/flowcharts.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.309807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18322 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.313807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/
--rwxr-xr-x   0 runner    (1001) docker     (127)      255 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1209 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.313807 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/setup_argparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/setup_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.313807 seamm_dashboard-2024.5.24/seamm_dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.317807 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/bootstrap-select.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    29130 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom_flowchart.css
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/jobs_list.css
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/prism.css
--rw-r--r--   0 runner    (1001) docker     (127)   281191 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)   647497 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232121 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   876516 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.317807 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/Banner_AllCaps.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    26358 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/briefcase.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon-inverted.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/object-group.svg
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/images/project-diagram.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.317807 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/3.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/4.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/5.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/6.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/7.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    20466 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/8.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/sygnet.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/buildings.js
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/collapsible.js
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/colors.js
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/flowchart_list.js
--rw-r--r--   0 runner    (1001) docker     (127)    19705 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/job_report.js
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/jobs_list.js
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/login.js
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/logout.js
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_groups.js
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_user.js
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_users.js
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/popovers.js
--rw-r--r--   0 runner    (1001) docker     (127)    32221 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/prism.js
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/project_list.js
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/render_flowchart.js
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/table_api.js
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/timer.js
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/tooltips.js
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/js/widgets.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.297807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)    31892 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.321807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1196706 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)    62563 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   372530 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/js/
--rw-r--r--   0 runner    (1001) docker     (127)    87278 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/css/
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/js/
--rw-r--r--   0 runner    (1001) docker     (127)    19994 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/js/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/js/
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    87533 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.325807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-24 17:13:01.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   141969 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png
--rw-r--r--   0 runner    (1001) docker     (127)    31730 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/dist/
--rw-r--r--   0 runner    (1001) docker     (127)  1120787 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/dist/ngl.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/pace-progress/
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/pace-progress/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/
--rw-r--r--   0 runner    (1001) docker     (127)    19549 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.329807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/plotly.js-dist-min/
--rw-r--r--   0 runner    (1001) docker     (127)  3478174 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.301807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.333807 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/umd/
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-05-24 17:13:02.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/only_needed_files.py
--rw-r--r--   0 runner    (1001) docker     (127)   101936 2024-05-24 17:13:25.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.333807 seamm_dashboard-2024.5.24/seamm_dashboard/static/tmp/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/static/tmp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/swagger.yml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/template_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.337807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/401.html
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.337807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/change_email.html
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/change_password.html
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_group.html
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_group.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_user.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.337807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/change_email.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/change_email.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/confirm.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/confirm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/reset_password.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_users.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/register.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/unconfirmed.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/confirm_login.html
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/manage_account.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/flowchart_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/render_flowchart.html
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/index_full.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/edit_job.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/import_job.html
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/job_parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/job_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/jobs_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/submit_job.html
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/login_coreui.html
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/login_script.html
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/logout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_access.html
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.341807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)    41683 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/card.html
--rw-r--r--   0 runner    (1001) docker     (127)    17627 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/cards.html
--rw-r--r--   0 runner    (1001) docker     (127)    16183 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)    47501 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/forms.html
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/jumbotron.html
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/list-group.html
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navs.html
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/popovers.html
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/progress.html
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/scrollspy.html
--rw-r--r--   0 runner    (1001) docker     (127)    40822 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/switches.html
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tables.html
--rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tabs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tooltips.html
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/blank.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)    41831 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/brand-buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/button-group.html
--rw-r--r--   0 runner    (1001) docker     (127)    27328 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/dropdowns.html
--rw-r--r--   0 runner    (1001) docker     (127)    38782 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/social-buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/charts.html
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/colors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    44734 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/flags.html
--rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/font-awesome.html
--rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/simple-line-icons.html
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.345807 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/alerts.html
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/modals.html
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/typography.html
--rw-r--r--   0 runner    (1001) docker     (127)    32244 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/widgets.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_authenticated.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/seamm_dashboard/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:13:26.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 17:14:13.000000 seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 17:14:13.349808 seamm_dashboard-2024.5.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-24 17:12:00.000000 seamm_dashboard-2024.5.24/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.515604 seamm_dashboard-2024.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-06-02 19:08:13.515604 seamm_dashboard-2024.6.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4850 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.515604 seamm_dashboard-2024.6.2/seamm_dashboard/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8236 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-02 19:08:13.515604 seamm_dashboard-2024.6.2/seamm_dashboard/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2120 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/flask_authorize_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/jwt_patch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      498 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/results_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.459604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.471604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.471604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/flowcharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.475604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.475604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/flowcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/flowcharts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/flowcharts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.475604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/jobs/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18322 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/jobs/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.475604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/main/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      255 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/main/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/main/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1209 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/main/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.475604 seamm_dashboard-2024.6.2/seamm_dashboard/routes/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/projects/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/routes/projects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/setup_argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/setup_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.475604 seamm_dashboard-2024.6.2/seamm_dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.479604 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/bootstrap-select.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29130 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/custom_flowchart.css
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/jobs_list.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/prism.css
+-rw-r--r--   0 runner    (1001) docker     (127)   281191 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)   647497 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232121 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   876516 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.479604 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/Banner_AllCaps.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    26358 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/briefcase.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/molssi-favicon-inverted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/molssi-favicon.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/object-group.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/images/project-diagram.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.483604 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.483604 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/4.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/5.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/6.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/7.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    20466 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/8.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.483604 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/brand/
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/brand/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/brand/sygnet.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/img/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/buildings.js
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/collapsible.js
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/colors.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/flowchart_list.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19705 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/job_report.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/jobs_list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/logout.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/manage_groups.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/manage_user.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/manage_users.js
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/popovers.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32221 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/prism.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/project_list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/render_flowchart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/table_api.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/timer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/js/widgets.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.467604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@coreui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@coreui/coreui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@coreui/coreui/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    31892 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@fortawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1196706 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/bootstrap/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/bootstrap/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    62563 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/cytoscape/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/cytoscape/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   372530 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    87278 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-06-02 19:06:59.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    19994 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.487604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-06-02 19:06:59.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-dt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-dt/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select-dt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-06-02 19:06:59.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    87533 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery-csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery-csv/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-06-02 19:06:59.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   141969 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.463604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31730 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.467604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/ngl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/ngl/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)  1120787 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/ngl/dist/ngl.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/pace-progress/
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/pace-progress/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.467604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/perfect-scrollbar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.491604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)    19549 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.495604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/plotly.js-dist-min/
+-rw-r--r--   0 runner    (1001) docker     (127)  3478174 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.467604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/popper.js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.467604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/popper.js/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.499604 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/popper.js/dist/umd/
+-rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-06-02 19:07:00.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/only_needed_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102009 2024-06-02 19:07:22.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.499604 seamm_dashboard-2024.6.2/seamm_dashboard/static/tmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/static/tmp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/swagger.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/template_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.499604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/401.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.503604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/change_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/create_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/create_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/delete_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/delete_user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.503604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/change_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/change_email.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/confirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/confirm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/reset_password.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/manage_users.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.503604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/confirm_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/manage_account.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.503604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/flowcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/flowcharts/flowchart_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/flowcharts/render_flowchart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    31853 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/index_full.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.503604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/edit_job.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/import_job.html
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/job_parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/job_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/jobs_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/submit_job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/login_coreui.html
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/login_script.html
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/logout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.503604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/projects/project_access.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/projects/project_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.507604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.511604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)    41683 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/card.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17627 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/cards.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16183 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47501 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/forms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/jumbotron.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/list-group.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/navs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/popovers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/scrollspy.html
+-rw-r--r--   0 runner    (1001) docker     (127)    40822 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/switches.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/tables.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/tooltips.html
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/blank.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.511604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)    41831 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/brand-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/button-group.html
+-rw-r--r--   0 runner    (1001) docker     (127)    27328 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/dropdowns.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38782 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/social-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/charts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/colors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.511604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    44734 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/flags.html
+-rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/font-awesome.html
+-rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/simple-line-icons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.511604 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/badge.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/modals.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/typography.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32244 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/widgets.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.511604 seamm_dashboard-2024.6.2/seamm_dashboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api_authenticated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/seamm_dashboard/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:08:13.511604 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-06-02 19:08:13.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-06-02 19:08:13.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:08:13.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-02 19:08:13.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:07:24.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-02 19:08:13.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 19:08:13.000000 seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-06-02 19:08:13.515604 seamm_dashboard-2024.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-06-02 19:06:05.000000 seamm_dashboard-2024.6.2/versioneer.py
```

### Comparing `seamm_dashboard-2024.5.24/LICENSE` & `seamm_dashboard-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/PKG-INFO` & `seamm_dashboard-2024.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-dashboard
-Version: 2024.5.24
+Version: 2024.6.2
 Summary: The Web Dashboard for SEAMM (Simulation Environment for Atomistic and Molecular Simulations).
 Home-page: https://github.com/molssi-seamm/seamm_dashboard.git
 Author: Jessica Nash
 Author-email: janash@vt.edu
 License: BSD-3C
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `seamm_dashboard-2024.5.24/README.md` & `seamm_dashboard-2024.6.2/README.md`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/__init__.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/config.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/config.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/flask_authorize_patch.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/flask_authorize_patch.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/jwt_patch.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/jwt_patch.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/forms.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/admin/forms.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/admin/views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/admin/views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/auth.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/auth.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/flowcharts.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/flowcharts.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/groups.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/groups.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/jobs.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/jobs.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/projects.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/projects.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/status.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/status.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/api/users.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/api/users.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,28 +28,32 @@
     if not original_user_data:
         # Check that both username and password are supplied
         if username is None or password is None:
             return Response(
                 "Both username and password must be supplied to create new user",
                 status=400,
             )
+        # Check if username exists.
+        if User.query.filter_by(username=username).first() is not None:
+            return Response(
+                f"User with username '{username}'' already exists", status=400
+            )
+
         # Create starting user object with the appropriate information
         user_info = {
             "username": username,
             "password": password,
             "roles": [],
-            "groups": [],
+            "groups": request_data.get("groups", []),
+            "first_name": request_data.get("first_name", None),
+            "last_name": request_data.get("last_name", None),
+            "email": request_data.get("email", None),
         }
-        user = User(**user_info)
 
-        # Check if username exists.
-        if User.query.filter_by(username=username).first() is not None:
-            return Response(
-                f"User with username '{username}'' already exists", status=400
-            )
+        user = User.create(**user_info)
 
     else:
         user = original_user_data
         user.roles = []
         user.groups = []
 
         # Check if username exists. First we check if the name is in the database. If
@@ -66,43 +70,30 @@
         # After check, update username and password.
         user.username = username
 
         # only set the password if the password is not blank
         if password:
             user.password = password
 
-    possible_keys = ["roles", "groups", "first_name", "last_name", "email"]
+        model_map = {"roles": Role, "groups": Group}
+        keys = ["roles", "groups", "first_name", "last_name", "email"]
 
-    map_values = {
-        "roles": Role,
-        "roles_values": [],
-        "groups": Group,
-        "group_values": [],
-    }
-
-    for key in possible_keys:
-        try:
-            if key == "roles" or key == "groups":
-                model = map_values[key]
-                for listed_value in request_data[key]:
-                    is_model = model.query.filter_by(name=listed_value).first()
-                    if not is_model:
+        for key in keys:
+            if key in model_map:
+                model = model_map[key]
+                values = request_data.get(key, [])
+                for value in values:
+                    item = model.query.filter_by(name=value).first()
+                    if not item:
                         return Response(
-                            f"{listed_value} is not an available value for {key}.",
-                            status=400,
+                            f"{value} is not an available value for {key}.", status=400
                         )
-                    else:
-                        if getattr(user, key) is None:
-                            setattr(user, key, [])
-                        getattr(user, key).append(is_model)
+                    getattr(user, key).append(item)
             else:
-                setattr(user, key, request_data[key])
-        except KeyError:
-            # Not a key in the body. Pass.
-            pass
+                setattr(user, key, request_data.get(key))
 
     return user
 
 
 @jwt_required(optional=True)
 @authorize.has_role("admin")
 def add_user(body):
```

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/forms.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/auth/forms.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/auth/views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/auth/views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/flowcharts/views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/flowcharts/views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/forms.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/jobs/forms.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/jobs/views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/jobs/views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/main/views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/main/views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/forms.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/projects/forms.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/routes/projects/views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/routes/projects/views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/setup_argparsing.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/setup_argparsing.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/setup_logging.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/setup_logging.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/bootstrap-select.min.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/custom_flowchart.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/custom_flowchart.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/prism.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/prism.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.css.map` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.min.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/css/style.min.css.map` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/css/style.min.css.map`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/Banner_AllCaps.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/images/Banner_AllCaps.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/images/MolSSI-Logo-xl.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon-inverted.svg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/images/molssi-favicon-inverted.svg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/molssi-favicon.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/images/molssi-favicon.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/images/object-group.svg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/images/object-group.svg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/1.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/1.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/2.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/2.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/3.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/3.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/4.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/4.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/5.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/5.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/6.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/6.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/7.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/7.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/avatars/8.jpg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/avatars/8.jpg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/logo.svg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/brand/logo.svg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/brand/sygnet.svg` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/brand/sygnet.svg`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.ico` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/img/favicon.png` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/buildings.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/buildings.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/colors.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/colors.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/flowchart_list.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/flowchart_list.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/job_report.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/job_report.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/jobs_list.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/jobs_list.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/main.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/main.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_groups.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/manage_groups.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_user.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/manage_user.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/manage_users.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/manage_users.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/prism.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/prism.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/project_list.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/project_list.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/render_flowchart.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/render_flowchart.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/setup.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/setup.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/table_api.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/table_api.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/timer.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/timer.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/util.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/util.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/js/widgets.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/js/widgets.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@coreui/coreui/dist/js/coreui.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/@fortawesome/fontawesome-free/js/all.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/cytoscape/dist/cytoscape.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/css/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-bs4/js/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-buttons-bs4/css/buttons.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-dt/js/dataTables.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select/js/dataTables.select.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/datatables.net-select-dt/css/select.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jquery-csv/src/jquery.csv.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/jstree.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/jstree/dist/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/ngl/dist/ngl.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/ngl/dist/ngl.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/pace-progress/pace.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/pace-progress/pace.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/perfect-scrollbar/dist/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/plotly.js-dist-min/plotly.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/node_modules/popper.js/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/only_needed_files.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/only_needed_files.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/package-lock.json` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999729437229437%*

 * *Differences: {"'packages'": "{'node_modules/glob': {'deprecated': 'Glob versions prior to v9 are no longer "*

 * *               "supported'}}"}*

```diff
@@ -1228,14 +1228,15 @@
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
                 "minimatch": "^3.1.1",
                 "once": "^1.3.0",
                 "path-is-absolute": "^1.0.0"
             },
+            "deprecated": "Glob versions prior to v9 are no longer supported",
             "engines": {
                 "node": "*"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==",
```

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/static/package.json` & `seamm_dashboard-2024.6.2/seamm_dashboard/static/package.json`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/swagger.yml` & `seamm_dashboard-2024.6.2/seamm_dashboard/swagger.yml`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/401.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/401.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/404.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/404.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/500.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/500.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/base.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_group.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/create_group.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/create_user.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/create_user.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_group.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/delete_group.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/delete_user.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/delete_user.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/email/reset_password.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_groups.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/manage_groups.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/manage_users.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/manage_users.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/admin/unconfirmed.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/admin/unconfirmed.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/base.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/auth/manage_account.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/auth/manage_account.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/flowchart_list.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/flowcharts/flowchart_list.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/flowcharts/render_flowchart.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/flowcharts/render_flowchart.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/index.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/index_full.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/index_full.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/edit_job.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/edit_job.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/job_report.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/job_report.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/jobs/jobs_list.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/jobs/jobs_list.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/login_coreui.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/login_coreui.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_access.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/projects/project_access.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/projects/project_list.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/projects/project_list.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/register.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/register.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/breadcrumb.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/card.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/card.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/cards.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/cards.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/carousel.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/carousel.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/collapse.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/collapse.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/forms.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/forms.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/jumbotron.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/jumbotron.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/list-group.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/list-group.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navbar.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/navbar.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/navs.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/navs.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/pagination.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/pagination.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/popovers.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/popovers.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/progress.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/progress.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/scrollspy.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/scrollspy.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/switches.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/switches.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tables.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/tables.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tabs.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/tabs.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/base/tooltips.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/base/tooltips.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/brand-buttons.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/brand-buttons.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/button-group.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/button-group.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/buttons.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/buttons.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/dropdowns.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/dropdowns.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/buttons/social-buttons.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/buttons/social-buttons.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/charts.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/charts.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/colors.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/colors.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/flags.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/flags.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/font-awesome.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/font-awesome.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/icons/simple-line-icons.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/icons/simple-line-icons.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/login.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/login.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/main.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/main.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/alerts.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/alerts.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/badge.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/badge.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/notifications/modals.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/notifications/modals.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/typography.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/typography.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/templates/views/widgets.html` & `seamm_dashboard-2024.6.2/seamm_dashboard/templates/views/widgets.html`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/tests/conftest.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_admin.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api_admin.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_api_authenticated.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_api_authenticated.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/tests/test_views.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard/util.py` & `seamm_dashboard-2024.6.2/seamm_dashboard/util.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/PKG-INFO` & `seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm-dashboard
-Version: 2024.5.24
+Version: 2024.6.2
 Summary: The Web Dashboard for SEAMM (Simulation Environment for Atomistic and Molecular Simulations).
 Home-page: https://github.com/molssi-seamm/seamm_dashboard.git
 Author: Jessica Nash
 Author-email: janash@vt.edu
 License: BSD-3C
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `seamm_dashboard-2024.5.24/seamm_dashboard.egg-info/SOURCES.txt` & `seamm_dashboard-2024.6.2/seamm_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/setup.py` & `seamm_dashboard-2024.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard-2024.5.24/versioneer.py` & `seamm_dashboard-2024.6.2/versioneer.py`

 * *Files identical despite different names*

