# Comparing `tmp/pyproject_pip-0.0.2.tar.gz` & `tmp/pyproject_pip-0.0.3.tar.gz`

## Comparing `pyproject_pip-0.0.2.tar` & `pyproject_pip-0.0.3.tar`

### file list

```diff
@@ -1,1021 +1,1021 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/requirements.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/.gitignore
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/pyvenv.cfg
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.csh
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.fish
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.nu
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.ps1
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate_this.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/normalizer
--rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/pip
--rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/pip-3.11
--rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/pip3
--rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/pip3.11
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/pypip
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/python -> /opt/homebrew/opt/python@3.11/bin/python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/wheel
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/wheel-3.11
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/wheel3
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/bin/wheel3.11
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_pyproject_pip.pth
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.virtualenv
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/__main__.py
--rw-r--r--   0        0        0    21097 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/api.py
--rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cd.py
--rw-r--r--   0        0        0    40481 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/constant.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/legacy.py
--rwxr-xr-x   0        0        0    50117 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so
--rw-r--r--   0        0        0    19624 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.py
--rwxr-xr-x   0        0        0   232636 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so
--rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/version.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cli/__main__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0        0        0    33550 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/__init__.py
--rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_compat.py
--rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_termui_impl.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_textwrap.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_winconsole.py
--rw-r--r--   0        0        0   114086 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/core.py
--rw-r--r--   0        0        0    18719 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/decorators.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/exceptions.py
--rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/formatting.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/globals.py
--rw-r--r--   0        0        0    19067 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/py.typed
--rw-r--r--   0        0        0    18460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/shell_completion.py
--rw-r--r--   0        0        0    28324 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/termui.py
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/testing.py
--rw-r--r--   0        0        0    36391 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/types.py
--rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/top_level.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/core.py
--rw-r--r--   0        0        0    78320 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/WHEEL
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0        0        0    74033 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0        0        0   108932 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   134976 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    20105 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
--rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/direct_url.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/_internal_utils.py
--rw-r--r--   0        0        0    27451 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/api.py
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/auth.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/certs.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/compat.py
--rw-r--r--   0        0        0    18590 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/cookies.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/exceptions.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/hooks.py
--rw-r--r--   0        0        0    35418 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/models.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/packages.py
--rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/sessions.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/structures.py
--rw-r--r--   0        0        0    33619 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/INSTALLER
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/LICENSE
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/METADATA
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/top_level.txt
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_core_metadata.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_normalization.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    18740 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/build_meta.py
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-32.exe
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-64.exe
--rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    21152 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    37504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-32.exe
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-64.exe
--rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/modified.py
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    38376 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/warnings.py
--rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_log.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_modified.py
--rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    48644 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17863 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    14977 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/_requirestxt.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16433 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    17724 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    15127 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    87124 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    34488 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    26516 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/py310.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/py311.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/py39.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    17383 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25630 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   274893 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/METADATA
--rw-r--r--   0        0        0    37032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_compat.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_types.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_utils.py
--rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/api.py
--rw-r--r--   0        0        0    28827 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/container.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/exceptions.py
--rw-r--r--   0        0        0    53209 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/items.py
--rw-r--r--   0        0        0    37935 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/py.typed
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/source.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_char.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_document.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_file.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/LICENSE
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/METADATA
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/REQUESTED
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/WHEEL
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/__init__.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_base_connection.py
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_collections.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_version.py
--rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connection.py
--rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/exceptions.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/filepost.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/http2.py
--rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/py.typed
--rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/socks.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/__init__.py
--rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/connection.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/fetch.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/request.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/response.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/response.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/retry.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/wait.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/METADATA
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/__main__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/_setuptools_logging.py
--rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/bdist_wheel.py
--rw-r--r--   0        0        0    16103 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/macosx_libfile.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/metadata.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/util.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/wheelfile.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/convert.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/pack.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/tags.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/unpack.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/vendor.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
--rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
--rw-r--r--   0        0        0    39778 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
--rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/METADATA
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/WHEEL
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/src/pyproject_pip/__about__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/src/pyproject_pip/__init__.py
--rwxr-xr-x   0        0        0    15614 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/src/pyproject_pip/pypip.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/tests/test_pypip.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/LICENSE
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/README.md
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyproject_pip-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/.gitignore
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/pyvenv.cfg
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.csh
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.fish
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.nu
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.ps1
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate_this.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/normalizer
+-rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/pip
+-rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/pip-3.11
+-rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/pip3
+-rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/pip3.11
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/pypip
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/python -> /opt/homebrew/opt/python@3.11/bin/python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/wheel
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/wheel3
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/bin/wheel3.11
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_pyproject_pip.pth
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.virtualenv
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/__main__.py
+-rw-r--r--   0        0        0   293951 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/cacert.pem
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/__main__.py
+-rw-r--r--   0        0        0    21097 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/api.py
+-rw-r--r--   0        0        0    12560 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cd.py
+-rw-r--r--   0        0        0    40481 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/constant.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/legacy.py
+-rwxr-xr-x   0        0        0    50117 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so
+-rw-r--r--   0        0        0    19624 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.py
+-rwxr-xr-x   0        0        0   232636 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/version.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cli/__main__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0        0        0    33550 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/METADATA
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/__init__.py
+-rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_compat.py
+-rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_termui_impl.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_textwrap.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_winconsole.py
+-rw-r--r--   0        0        0   114086 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/core.py
+-rw-r--r--   0        0        0    18719 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/decorators.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/exceptions.py
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/formatting.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/globals.py
+-rw-r--r--   0        0        0    19067 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/py.typed
+-rw-r--r--   0        0        0    18460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/shell_completion.py
+-rw-r--r--   0        0        0    28324 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/termui.py
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/testing.py
+-rw-r--r--   0        0        0    36391 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/types.py
+-rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/compat.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/core.py
+-rw-r--r--   0        0        0    78320 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/py.typed
+-rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/uts46data.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/METADATA
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/WHEEL
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0    74033 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108932 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0        0        0   134976 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    20105 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/METADATA
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/direct_url.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/_internal_utils.py
+-rw-r--r--   0        0        0    27451 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/api.py
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/auth.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/certs.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/compat.py
+-rw-r--r--   0        0        0    18590 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/cookies.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/exceptions.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/hooks.py
+-rw-r--r--   0        0        0    35418 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/models.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/packages.py
+-rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/sessions.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/structures.py
+-rw-r--r--   0        0        0    33619 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/LICENSE
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/METADATA
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_core_metadata.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_normalization.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    18740 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    21152 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    37504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/modified.py
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47476 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    38376 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/warnings.py
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_log.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_modified.py
+-rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    48644 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17863 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    14977 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/_requirestxt.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16433 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    17724 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    15127 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    87124 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    34488 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    26516 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/py310.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/py311.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/compat/py39.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    17383 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    25630 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   274893 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0    37032 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/__init__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_compat.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_types.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_utils.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/api.py
+-rw-r--r--   0        0        0    28827 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/container.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/exceptions.py
+-rw-r--r--   0        0        0    53209 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/items.py
+-rw-r--r--   0        0        0    37935 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/py.typed
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/source.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_char.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_document.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_file.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/LICENSE
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/METADATA
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/REQUESTED
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/WHEEL
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/__init__.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_collections.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_version.py
+-rw-r--r--   0        0        0    34704 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connection.py
+-rw-r--r--   0        0        0    43556 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/exceptions.py
+-rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/filepost.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/http2.py
+-rw-r--r--   0        0        0    22935 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/py.typed
+-rw-r--r--   0        0        0    43874 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19161 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/__init__.py
+-rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/connection.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/fetch.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/request.py
+-rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/response.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/response.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/retry.py
+-rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/wait.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/METADATA
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/_setuptools_logging.py
+-rw-r--r--   0        0        0    20938 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    16103 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/tags.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/vendor.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
+-rw-r--r--   0        0        0    39778 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
+-rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/src/pyproject_pip/__about__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/src/pyproject_pip/__init__.py
+-rwxr-xr-x   0        0        0    15673 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/src/pyproject_pip/pypip.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/tests/test_pypip.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/LICENSE
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/README.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pyproject_pip-0.0.3/PKG-INFO
```

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate` & `pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.csh` & `pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.fish` & `pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.nu` & `pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate.ps1` & `pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/bin/activate_this.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_virtualenv.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/cacert.pem` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/cacert.pem`

 * *Files 1% similar despite different names*

```diff
@@ -4808,7 +4808,31 @@
 xKITDmcZuI1CfmwMmm6gJC3VRRvcxAIU/oVbZZfKTpBQCHpCNfnqwmbU+AGuHrS+
 w6jv/naaoqYfRvaE7fzbzsQCzndILIyy7MMAo+wsVRjBfhnu4S/yrYObnqsZ38aK
 L4x35bcF7DvB7L6Gs4a8wPfc5+pbrrLMtTWGS9DiP7bY+A4A7l3j941Y/8+LN+lj
 X273CXE2whJdV/LItM3z7gLfEdxquVeEHVlNjM7IDiPCtyaaEBRx/pOyiriA8A4Q
 ntOoUAw3gi/q4Iqd4Sw5/7W0cwDk90imc6y/st53BIe0o82bNSQ3+pCTE4FCxpgm
 dTdmQRCsu/WU48IxK63nI1bMNSWSs1A=
 -----END CERTIFICATE-----
+
+# Issuer: CN=FIRMAPROFESIONAL CA ROOT-A WEB O=Firmaprofesional SA
+# Subject: CN=FIRMAPROFESIONAL CA ROOT-A WEB O=Firmaprofesional SA
+# Label: "FIRMAPROFESIONAL CA ROOT-A WEB"
+# Serial: 65916896770016886708751106294915943533
+# MD5 Fingerprint: 82:b2:ad:45:00:82:b0:66:63:f8:5f:c3:67:4e:ce:a3
+# SHA1 Fingerprint: a8:31:11:74:a6:14:15:0d:ca:77:dd:0e:e4:0c:5d:58:fc:a0:72:a5
+# SHA256 Fingerprint: be:f2:56:da:f2:6e:9c:69:bd:ec:16:02:35:97:98:f3:ca:f7:18:21:a0:3e:01:82:57:c5:3c:65:61:7f:3d:4a
+-----BEGIN CERTIFICATE-----
+MIICejCCAgCgAwIBAgIQMZch7a+JQn81QYehZ1ZMbTAKBggqhkjOPQQDAzBuMQsw
+CQYDVQQGEwJFUzEcMBoGA1UECgwTRmlybWFwcm9mZXNpb25hbCBTQTEYMBYGA1UE
+YQwPVkFURVMtQTYyNjM0MDY4MScwJQYDVQQDDB5GSVJNQVBST0ZFU0lPTkFMIENB
+IFJPT1QtQSBXRUIwHhcNMjIwNDA2MDkwMTM2WhcNNDcwMzMxMDkwMTM2WjBuMQsw
+CQYDVQQGEwJFUzEcMBoGA1UECgwTRmlybWFwcm9mZXNpb25hbCBTQTEYMBYGA1UE
+YQwPVkFURVMtQTYyNjM0MDY4MScwJQYDVQQDDB5GSVJNQVBST0ZFU0lPTkFMIENB
+IFJPT1QtQSBXRUIwdjAQBgcqhkjOPQIBBgUrgQQAIgNiAARHU+osEaR3xyrq89Zf
+e9MEkVz6iMYiuYMQYneEMy3pA4jU4DP37XcsSmDq5G+tbbT4TIqk5B/K6k84Si6C
+cyvHZpsKjECcfIr28jlgst7L7Ljkb+qbXbdTkBgyVcUgt5SjYzBhMA8GA1UdEwEB
+/wQFMAMBAf8wHwYDVR0jBBgwFoAUk+FDY1w8ndYn81LsF7Kpryz3dvgwHQYDVR0O
+BBYEFJPhQ2NcPJ3WJ/NS7Beyqa8s93b4MA4GA1UdDwEB/wQEAwIBBjAKBggqhkjO
+PQQDAwNoADBlAjAdfKR7w4l1M+E7qUW/Runpod3JIha3RxEL2Jq68cgLcFBTApFw
+hVmpHqTm6iMxoAACMQD94vizrxa5HnPEluPBMBnYfubDl94cT7iJLzPrSA8Z94dG
+XSaQpYXFuXqUPoeovQA=
+-----END CERTIFICATE-----
```

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/LICENSE` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certifi
-Version: 2024.2.2
+Version: 2024.6.2
 Summary: Python package for providing Mozilla's CA Bundle.
 Home-page: https://github.com/certifi/python-certifi
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/certifi/python-certifi
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Certifi: Python SSL Certificates
 ================================
 
 Certifi provides Mozilla's carefully curated collection of Root Certificates for
```

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/certifi-2024.6.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-certifi-2024.2.2.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
-certifi-2024.2.2.dist-info/LICENSE,sha256=6TcW2mucDVpKHfYP5pWzcPBpVgPSH2-D8FPkLPwQyvc,989
-certifi-2024.2.2.dist-info/METADATA,sha256=1noreLRChpOgeSj0uJT1mehiBl8ngh33Guc7KdvzYYM,2170
-certifi-2024.2.2.dist-info/RECORD,,
-certifi-2024.2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-certifi-2024.2.2.dist-info/top_level.txt,sha256=KMu4vUCfsjLrkPbSNdgdekS-pVJzBAJFO__nI8NF6-U,8
-certifi/__init__.py,sha256=ljtEx-EmmPpTe2SOd5Kzsujm_lUD0fKJVnE9gzce320,94
+certifi-2024.6.2.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
+certifi-2024.6.2.dist-info/LICENSE,sha256=6TcW2mucDVpKHfYP5pWzcPBpVgPSH2-D8FPkLPwQyvc,989
+certifi-2024.6.2.dist-info/METADATA,sha256=0JvKStGd0rn8QzECH3rN6wcw-6ZmNtR68uciKdXeVmU,2221
+certifi-2024.6.2.dist-info/RECORD,,
+certifi-2024.6.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+certifi-2024.6.2.dist-info/top_level.txt,sha256=KMu4vUCfsjLrkPbSNdgdekS-pVJzBAJFO__nI8NF6-U,8
+certifi/__init__.py,sha256=OemlOQZNxjR0BTLg7e4GIST-_QTOZsTKNgXw4v_0DwI,94
 certifi/__main__.py,sha256=xBBoj905TUWBLRGANOcf7oi6e-3dMP4cEoG9OyMs11g,243
 certifi/__pycache__/__init__.cpython-311.pyc,,
 certifi/__pycache__/__main__.cpython-311.pyc,,
 certifi/__pycache__/core.cpython-311.pyc,,
-certifi/cacert.pem,sha256=ejR8qP724p-CtuR4U1WmY1wX-nVeCUD2XxWqj8e9f5I,292541
+certifi/cacert.pem,sha256=FgXQ05xeJdZ-eDjaahfc8ujGz6eQMOj7AxjjX1SVSTw,293951
 certifi/core.py,sha256=qRDDFyXVJwTB_EmoGppaXU_R9qCZvhl-EzxPMuV3nTA,4426
 certifi/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
```

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cd.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/constant.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/legacy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/md__mypyc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/models.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cli/__main__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_termui_impl.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_textwrap.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/_winconsole.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/decorators.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/decorators.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/formatting.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/formatting.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/globals.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/globals.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/shell_completion.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/shell_completion.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/termui.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/termui.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/testing.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/testing.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/types.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/types.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/codec.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/idnadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/intranges.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna/uts46data.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/LICENSE.md` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/idna-3.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__main__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__pip-runner__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/build_env.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cache.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/configuration.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/index.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/link.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/download.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/session.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/six.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_macos.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_openssl.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_ssl_constants.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_windows.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/AUTHORS.txt` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/LICENSE.txt` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pip-24.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-pip
-Version: 0.0.1
+Version: 0.0.2
 Summary: Install and manage pyproject.toml with pip commands.
 Project-URL: Documentation, https://github.com/Sebastian Peralta/pypip#readme
 Project-URL: Issues, https://github.com/Sebastian Peralta/pypip/issues
 Project-URL: Source, https://github.com/Sebastian Peralta/pypip
 Author-email: Sebastian Peralta <sebastian@mbodi.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -15,14 +15,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Provides-Extra: all
+Requires-Dist: click; extra == 'all'
+Requires-Dist: requests; extra == 'all'
+Requires-Dist: tomlkit; extra == 'all'
 Description-Content-Type: text/markdown
 
 # pypip
 
 [![PyPI - Version](https://img.shields.io/pypi/v/pypip.svg)](https://pypi.org/project/pypip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pypip.svg)](https://pypi.org/project/pypip)
```

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ../../../bin/pypip,sha256=qouNMb0bjM1gH6LKDO1OnaF0pRpAOL4GABv-gDQf42Y,291
 _pyproject_pip.pth,sha256=WVn-mRLjfpkA9rrwSYbD6Gc0muvySRKAWza184vPU_U,66
-pyproject_pip-0.0.1.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
-pyproject_pip-0.0.1.dist-info/METADATA,sha256=a8QtJPccadx9egZQcnrP7iMVCvQcpyNxCQi4v-_t6L4,1478
-pyproject_pip-0.0.1.dist-info/RECORD,,
-pyproject_pip-0.0.1.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyproject_pip-0.0.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-pyproject_pip-0.0.1.dist-info/direct_url.json,sha256=-NzL-xIBajyP6Eiy4X_va8BJbVgD7k01uE_cIlwoZOM,112
-pyproject_pip-0.0.1.dist-info/entry_points.txt,sha256=XIDrwIELm3de396V0JI34ALH3ZvY7I-vzLPGCBMxJ-8,50
-pyproject_pip-0.0.1.dist-info/licenses/LICENSE,sha256=ufv7fH68SJM3IBc79lq9_jbu9jq8YtkuzYWO9P3AuU8,1062
-pyproject_pip-0.0.1.dist-info/licenses/LICENSE.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyproject_pip-0.0.2.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
+pyproject_pip-0.0.2.dist-info/METADATA,sha256=FZybtr0NGFp_47y68xnp2Vuf1BqldGqkoS7tGKkW11Y,1614
+pyproject_pip-0.0.2.dist-info/RECORD,,
+pyproject_pip-0.0.2.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pyproject_pip-0.0.2.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+pyproject_pip-0.0.2.dist-info/direct_url.json,sha256=-NzL-xIBajyP6Eiy4X_va8BJbVgD7k01uE_cIlwoZOM,112
+pyproject_pip-0.0.2.dist-info/entry_points.txt,sha256=XIDrwIELm3de396V0JI34ALH3ZvY7I-vzLPGCBMxJ-8,50
+pyproject_pip-0.0.2.dist-info/licenses/LICENSE,sha256=ufv7fH68SJM3IBc79lq9_jbu9jq8YtkuzYWO9P3AuU8,1062
+pyproject_pip-0.0.2.dist-info/licenses/LICENSE.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
```

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.1.dist-info/licenses/LICENSE` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/pyproject_pip-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/_internal_utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/adapters.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/auth.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/cookies.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/help.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/hooks.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/models.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/packages.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/sessions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/status_codes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/structures.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/LICENSE` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/requests-2.32.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_core_metadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_entry_points.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_imp.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_importlib.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_itertools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_normalization.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_normalization.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_path.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_reqs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/archive_util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/build_meta.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-32.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-64.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-arm64.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dep_util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/depends.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/discovery.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/errors.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extension.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/glob.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-32.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-64.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-arm64.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui.exe` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/installer.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/launch.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/logging.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/monkey.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/msvc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/namespaces.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/package_index.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/sandbox.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/warnings.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/warnings.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/windows_support.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_functools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_functools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_modified.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_modified.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/_requirestxt.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/_requirestxt.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/alias.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_py.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/develop.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/rotate.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/sdist.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/setopt.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/test.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/expand.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/LICENSE` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/entry_points.txt` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/setuptools-69.2.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_compat.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_compat.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_types.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_types.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/_utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/api.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/api.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/container.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/container.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/items.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/items.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/source.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/source.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_char.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_char.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_file.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit/toml_file.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/LICENSE` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/tomlkit-0.12.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_base_connection.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_collections.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_request_methods.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connection.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connectionpool.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/exceptions.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/fields.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/filepost.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/http2.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/http2.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/poolmanager.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/response.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/socks.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/connection.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/connection.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/emscripten_fetch_worker.js`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/fetch.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/fetch.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/request.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/request.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/response.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/contrib/emscripten/response.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/connection.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/proxy.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/request.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/response.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/retry.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssltransport.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/timeout.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/url.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/wait.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/urllib3-2.2.1.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/_setuptools_logging.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/bdist_wheel.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/macosx_libfile.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/metadata.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/util.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/wheelfile.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/__init__.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/convert.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/pack.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/tags.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/unpack.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/version.py` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel/vendored/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/LICENSE.txt` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/METADATA` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/RECORD` & `pyproject_pip-0.0.3/.pypip/envs/pypip/lib/python3.11/site-packages/wheel-0.43.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/src/pyproject_pip/pypip.py` & `pyproject_pip-0.0.3/src/pyproject_pip/pypip.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,21 +169,20 @@
         dependency_group (str, optional): The group of dependencies to modify. Defaults to "dependencies".
     """
     is_optional = dependency_group != "dependencies"
     pyproject = read_pyproject_toml()
 
     # Prepare the package string with version if provided
     package_version_str = f"{package_name}{('==' + package_version) if package_version else ''}"
-    
+    is_hatch_env =  hatch_env and  "tool" in pyproject and "hatch" in pyproject["tool"]
     if not is_optional:
         # Modify standard dependencies based on action
         dependencies = (
             pyproject["tool"]["hatch"]["envs"][hatch_env].get("dependencies", [])
-            if "tool" in pyproject and "hatch" in pyproject["tool"]
-            else pyproject.get("project", {}).get(dependency_group, [])
+            if is_hatch_env else pyproject.setdefault("project", {}).get("dependencies", [])
         )
         dependencies = modify_dependencies(dependencies, package_version_str, action)
         optional_dependencies = pyproject.get("project", {}).get("optional-dependencies", {})
         optional_dependencies = modify_optional_dependencies(optional_dependencies, package_version_str, action, "all")
     else:
         dependencies = []
         # Modify optional dependencies based on action
@@ -192,17 +191,19 @@
             optional_dependencies,
             package_version_str,
             action,
             dependency_group,
         )
 
     # Update the pyproject.toml with modified dependencies
-    if "tool" in pyproject and "hatch" in pyproject["tool"]:
+    if is_hatch_env:
+        print('updating hatch')
         pyproject["tool"]["hatch"]["envs"][hatch_env]["dependencies"] = dependencies
     else:
+        print('Updating deps')
         pyproject.setdefault("project", {})["dependencies"] = dependencies
     pyproject.setdefault("project", {})["optional-dependencies"] = optional_dependencies
 
     write_pyproject_toml(pyproject)
 
 
 @click.group(invoke_without_command=True)
```

### Comparing `pyproject_pip-0.0.2/tests/test_pypip.py` & `pyproject_pip-0.0.3/tests/test_pypip.py`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/LICENSE` & `pyproject_pip-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pip-0.0.2/pyproject.toml` & `pyproject_pip-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,19 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [
+    "tomlkit",
+    "click",
+    "requests"
+]
 
 [project.urls]
 Documentation = "https://github.com/Sebastian Peralta/pypip#readme"
 Issues = "https://github.com/Sebastian Peralta/pypip/issues"
 Source = "https://github.com/Sebastian Peralta/pypip"
 
 [project.scripts]
```

### Comparing `pyproject_pip-0.0.2/PKG-INFO` & `pyproject_pip-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-pip
-Version: 0.0.2
+Version: 0.0.3
 Summary: Install and manage pyproject.toml with pip commands.
 Project-URL: Documentation, https://github.com/Sebastian Peralta/pypip#readme
 Project-URL: Issues, https://github.com/Sebastian Peralta/pypip/issues
 Project-URL: Source, https://github.com/Sebastian Peralta/pypip
 Author-email: Sebastian Peralta <sebastian@mbodi.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -15,14 +15,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: click
+Requires-Dist: requests
+Requires-Dist: tomlkit
 Provides-Extra: all
 Requires-Dist: click; extra == 'all'
 Requires-Dist: requests; extra == 'all'
 Requires-Dist: tomlkit; extra == 'all'
 Description-Content-Type: text/markdown
 
 # pypip
```

