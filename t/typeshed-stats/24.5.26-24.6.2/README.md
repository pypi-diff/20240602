# Comparing `tmp/typeshed_stats-24.5.26.tar.gz` & `tmp/typeshed_stats-24.6.2.tar.gz`

## Comparing `typeshed_stats-24.5.26.tar` & `typeshed_stats-24.6.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.editorconfig
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.gitattributes
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.markdownlint.yaml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/mkdocs.yml
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/website_macros.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/renovate.json5
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/check-requirements.yml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/regen-examples-and-docs.yml
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/test-website.yml
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/test.yml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/typecheck.yml
--rw-r--r--   0        0        0    31422 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/examples/example.csv
--rw-r--r--   0        0        0   170862 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/examples/example.json
--rw-r--r--   0        0        0   286082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/examples/example.md
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/scripts/regenerate.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/scripts/runtests.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/__init__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/__main__.py
--rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/_cli.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/_markdown_template.md.jinja
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/_version.py
--rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/gather.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/py.typed
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/serialize.py
--rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/big_logo.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/cli.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/gather.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/index.md
--rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/logo.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/serialize.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/stats-csv.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/stats.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/.snippets/links.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/.snippets/refs.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/javascripts/filtertable.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/javascripts/tablesort.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/__init__.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/conftest.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test___all__.py
--rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test__cli.py
--rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test_gather.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test_running_from_command_line.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test_serialize.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/LICENSE
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/README.md
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/pyproject.toml
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.editorconfig
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.gitattributes
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.markdownlint.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/mkdocs.yml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/website_macros.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/renovate.json5
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/workflows/check-requirements.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/workflows/regen-examples-and-docs.yml
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/workflows/test-website.yml
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.github/workflows/typecheck.yml
+-rw-r--r--   0        0        0    31754 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/examples/example.csv
+-rw-r--r--   0        0        0   172898 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/examples/example.json
+-rw-r--r--   0        0        0   289512 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/examples/example.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/scripts/regenerate.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/scripts/runtests.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/__main__.py
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/_cli.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/_markdown_template.md.jinja
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/_version.py
+-rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/gather.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/py.typed
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/src/typeshed_stats/serialize.py
+-rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/big_logo.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/cli.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/gather.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/index.md
+-rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/logo.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/serialize.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/stats-csv.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/stats.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/.snippets/links.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/.snippets/refs.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/javascripts/filtertable.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/stats_website/javascripts/tablesort.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/conftest.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/test___all__.py
+-rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/test__cli.py
+-rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/test_gather.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/test_running_from_command_line.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/tests/test_serialize.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/LICENSE
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/README.md
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/pyproject.toml
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 typeshed_stats-24.6.2/PKG-INFO
```

### Comparing `typeshed_stats-24.5.26/.pre-commit-config.yaml` & `typeshed_stats-24.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/mkdocs.yml` & `typeshed_stats-24.6.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/website_macros.py` & `typeshed_stats-24.6.2/website_macros.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/renovate.json5` & `typeshed_stats-24.6.2/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/workflows/check-requirements.yml` & `typeshed_stats-24.6.2/.github/workflows/check-requirements.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/workflows/publish.yml` & `typeshed_stats-24.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/workflows/regen-examples-and-docs.yml` & `typeshed_stats-24.6.2/.github/workflows/regen-examples-and-docs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/workflows/test-website.yml` & `typeshed_stats-24.6.2/.github/workflows/test-website.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/workflows/test.yml` & `typeshed_stats-24.6.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.github/workflows/typecheck.yml` & `typeshed_stats-24.6.2/.github/workflows/typecheck.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/examples/example.csv` & `typeshed_stats-24.6.2/examples/example.csv`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 colorama,types-colorama,https://github.com/tartley/colorama,COMPLETE,-,201,UP_TO_DATE,UPLOADED,STRICT,89,0,60,0,0,0,3,1,85,0,0,11,0,0,ERROR_ON_MISSING_STUB,linux;win32,44
 commonmark,types-commonmark,https://github.com/rtfd/commonmark.py,PARTIAL,-,370,UP_TO_DATE,UPLOADED,NOT_STRICT,63,158,84,76,55,0,0,0,133,86,0,18,0,0,MISSING_STUBS_IGNORED,linux,0
 console-menu,types-console-menu,https://github.com/aegirhall/console-menu,COMPLETE,-,711,UP_TO_DATE,UPLOADED,STRICT,217,0,278,0,0,0,7,1,58,3,1,39,0,0,ERROR_ON_MISSING_STUB,linux,0
 croniter,types-croniter,https://github.com/kiorky/croniter,COMPLETE,-,151,UP_TO_DATE,UPLOADED,STRICT,69,0,24,0,0,0,0,8,29,0,0,8,1,0,ERROR_ON_MISSING_STUB,linux,0
 dateparser,types-dateparser,https://github.com/scrapinghub/dateparser,COMPLETE,-,473,UP_TO_DATE,UPLOADED,NOT_STRICT,126,130,74,69,21,0,4,6,135,76,0,34,0,0,ERROR_ON_MISSING_STUB,linux,6
 decorator,types-decorator,https://github.com/micheles/decorator,COMPLETE,-,66,UP_TO_DATE,UPLOADED,STRICT,36,0,13,0,0,0,19,6,15,3,0,2,0,0,ERROR_ON_MISSING_STUB,linux,10
 defusedxml,types-defusedxml,https://github.com/tiran/defusedxml,PARTIAL,-,234,UP_TO_DATE,UPLOADED,NOT_STRICT,81,97,38,13,13,0,0,1,37,0,19,12,0,0,MISSING_STUBS_IGNORED,linux,0
-docker,types-docker,https://github.com/docker/docker-py,COMPLETE,-,1899,OUT_OF_DATE,UPLOADED,NOT_STRICT,782,376,292,270,315,7,19,25,206,2,83,128,2,24,ERROR_ON_MISSING_STUB,linux,7
+docker,types-docker,https://github.com/docker/docker-py,COMPLETE,-,1936,UP_TO_DATE,UPLOADED,NOT_STRICT,801,373,294,269,315,7,19,25,210,2,83,131,2,24,ERROR_ON_MISSING_STUB,linux,7
 dockerfile-parse,types-dockerfile-parse,https://github.com/containerbuildsystem/dockerfile-parse,COMPLETE,-,113,UP_TO_DATE,UPLOADED,STRICT,46,0,24,0,0,0,0,0,39,0,0,8,0,0,ERROR_ON_MISSING_STUB,linux,0
 docopt,types-docopt,https://github.com/docopt/docopt,COMPLETE,-,14,UP_TO_DATE,UPLOADED,STRICT,7,0,3,0,1,0,0,1,2,0,0,2,0,0,ERROR_ON_MISSING_STUB,linux,0
 docutils,types-docutils,https://sourceforge.net/p/docutils/code,PARTIAL,-,1493,UP_TO_DATE,UPLOADED,NOT_STRICT,762,51,448,7,51,33,39,19,250,20,1,222,1,0,MISSING_STUBS_IGNORED,linux,18
 editdistance,types-editdistance,https://github.com/roy-ht/editdistance,COMPLETE,-,5,UP_TO_DATE,UPLOADED,STRICT,10,0,4,0,0,0,0,0,0,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,1
 entrypoints,types-entrypoints,https://github.com/takluyver/entrypoints,COMPLETE,-,41,UP_TO_DATE,UPLOADED,STRICT,23,0,12,0,0,0,0,1,12,0,0,5,0,0,ERROR_ON_MISSING_STUB,linux,1
 fanstatic,types-fanstatic,https://github.com/zopefoundation/fanstatic,COMPLETE,-,530,UP_TO_DATE,UPLOADED,STRICT,167,0,133,0,0,0,8,3,128,0,0,49,0,0,ERROR_ON_MISSING_STUB,linux,40
 first,types-first,https://github.com/hynek/first,COMPLETE,-,14,UP_TO_DATE,UPLOADED,STRICT,8,0,4,0,0,0,2,0,2,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,0
@@ -74,19 +74,20 @@
 keyboard,types-keyboard,https://github.com/boppreh/keyboard,COMPLETE,-,246,UP_TO_DATE,UPLOADED,STRICT,130,0,76,0,0,0,0,0,38,0,0,7,0,0,ERROR_ON_MISSING_STUB,linux,7
 ldap3,types-ldap3,https://github.com/cannatag/ldap3,PARTIAL,-,2659,UP_TO_DATE,UPLOADED,NOT_STRICT,558,654,219,421,282,0,0,0,931,322,57,316,0,0,MISSING_STUBS_IGNORED,linux,0
 libsass,types-libsass,https://github.com/sass/libsass-python,COMPLETE,-,230,UP_TO_DATE,UPLOADED,STRICT,109,0,41,0,0,0,2,0,36,0,0,17,0,0,ERROR_ON_MISSING_STUB,linux,2
 lzstring,types-lzstring,https://github.com/gkovacs/lz-string-python,COMPLETE,-,17,UP_TO_DATE,UPLOADED,STRICT,8,0,8,0,0,0,0,0,0,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,5
 mock,types-mock,https://github.com/testing-cabal/mock,COMPLETE,-,390,UP_TO_DATE,UPLOADED,STRICT,217,0,90,0,45,0,86,15,58,34,0,24,2,0,ERROR_ON_MISSING_STUB,linux,4
 mypy-extensions,types-mypy-extensions,https://github.com/python/mypy_extensions,COMPLETE,-,79,UP_TO_DATE,UPLOADED,STRICT,31,0,28,0,0,0,3,7,1,0,0,3,0,0,ERROR_ON_MISSING_STUB,linux,6
 mysqlclient,types-mysqlclient,https://github.com/PyMySQL/mysqlclient,COMPLETE,-,1228,UP_TO_DATE,UPLOADED,NOT_STRICT,35,124,37,79,3,0,0,0,971,0,28,35,0,1,ERROR_ON_MISSING_STUB,linux,1
-netaddr,types-netaddr,https://github.com/drkjam/netaddr,COMPLETE,-,696,UP_TO_DATE,UPLOADED,STRICT_ON_SOME_FILES,286,4,308,0,1,0,1,1,101,1,2,43,0,0,ERROR_ON_MISSING_STUB,linux,2
-networkx,types-networkx,https://github.com/networkx/networkx,PARTIAL,-,4781,OUT_OF_DATE,UPLOADED,NOT_STRICT,1959,1511,503,808,763,102,4,3,320,2,249,126,1,2,MISSING_STUBS_IGNORED,linux,13
+nanoid,types-nanoid,https://github.com/puyuan/py-nanoid,COMPLETE,-,16,UP_TO_DATE,UPLOADED,STRICT,8,0,4,0,0,0,0,0,2,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,0
+netaddr,types-netaddr,https://github.com/drkjam/netaddr,COMPLETE,-,698,UP_TO_DATE,UPLOADED,STRICT_ON_SOME_FILES,288,4,308,0,1,0,1,1,101,1,2,43,0,0,ERROR_ON_MISSING_STUB,linux,2
+networkx,types-networkx,https://github.com/networkx/networkx,PARTIAL,-,4784,OUT_OF_DATE,UPLOADED,NOT_STRICT,1961,1511,504,808,763,102,4,3,320,2,249,126,1,2,MISSING_STUBS_IGNORED,linux,13
 oauthlib,types-oauthlib,https://github.com/oauthlib/oauthlib,PARTIAL,-,1444,UP_TO_DATE,UPLOADED,NOT_STRICT,406,414,161,191,182,0,0,0,329,207,2,109,2,0,MISSING_STUBS_IGNORED,linux,1
 olefile,types-olefile,https://github.com/decalage2/olefile,COMPLETE,-,214,UP_TO_DATE,UPLOADED,STRICT,103,0,66,0,0,0,0,0,73,0,0,7,0,0,ERROR_ON_MISSING_STUB,linux,1
-openpyxl,types-openpyxl,https://foss.heptapod.net/openpyxl/openpyxl,COMPLETE,-,13238,UP_TO_DATE,UPLOADED,NOT_STRICT,3902,341,1315,91,211,8,12,13,4048,3,352,609,1,21,ERROR_ON_MISSING_STUB,linux,183
+openpyxl,types-openpyxl,https://foss.heptapod.net/openpyxl/openpyxl,COMPLETE,-,13238,OUT_OF_DATE,UPLOADED,NOT_STRICT,3902,341,1315,91,211,8,12,13,4048,3,352,609,1,21,ERROR_ON_MISSING_STUB,linux,183
 opentracing,types-opentracing,https://github.com/opentracing/opentracing-python,PARTIAL,-,331,UP_TO_DATE,UPLOADED,STRICT,105,0,113,0,1,0,21,0,56,4,0,26,0,0,MISSING_STUBS_IGNORED,linux,4
 paho-mqtt,types-paho-mqtt,https://github.com/eclipse/paho.mqtt.python,COMPLETE,-,513,OBSOLETE,UPLOADED,STRICT,217,0,147,0,0,0,5,4,145,0,1,19,0,0,ERROR_ON_MISSING_STUB,linux,0
 paramiko,types-paramiko,https://github.com/paramiko/paramiko,PARTIAL,-,1840,UP_TO_DATE,UPLOADED,STRICT,770,0,642,0,3,0,20,9,545,14,3,124,2,0,MISSING_STUBS_IGNORED,linux;win32,6
 parsimonious,types-parsimonious,https://github.com/erikrose/parsimonious,COMPLETE,-,187,UP_TO_DATE,UPLOADED,STRICT_ON_SOME_FILES,114,0,59,1,0,0,22,2,34,3,2,27,0,0,ERROR_ON_MISSING_STUB,linux,4
 passlib,types-passlib,https://foss.heptapod.net/python-libs/passlib,COMPLETE,-,1798,UP_TO_DATE,UPLOADED,NOT_STRICT,410,442,187,297,132,0,27,13,576,92,3,143,2,0,ERROR_ON_MISSING_STUB,linux,31
 passpy,types-passpy,https://github.com/bfrascher/passpy,COMPLETE,-,47,UP_TO_DATE,UPLOADED,STRICT,43,0,20,0,0,0,0,0,1,0,0,3,0,0,ERROR_ON_MISSING_STUB,linux,3
 peewee,types-peewee,https://github.com/coleifer/peewee,PARTIAL,-,1693,OUT_OF_DATE,UPLOADED,NOT_STRICT,425,669,346,438,216,5,0,0,420,0,348,168,0,0,ERROR_ON_MISSING_STUB,linux,11
@@ -106,15 +107,15 @@
 pycocotools,types-pycocotools,https://github.com/ppwwyyxx/cocoapi,COMPLETE,-,183,UP_TO_DATE,UPLOADED,STRICT,51,0,35,0,0,0,0,1,70,0,1,12,0,0,ERROR_ON_MISSING_STUB,linux,0
 pycurl,types-pycurl,https://github.com/pycurl/pycurl,COMPLETE,-,706,UP_TO_DATE,UPLOADED,NOT_STRICT,15,7,26,6,0,4,0,0,659,0,0,4,0,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,0
 pyfarmhash,types-pyfarmhash,https://github.com/veelion/python-farmhash,COMPLETE,-,9,UP_TO_DATE,UPLOADED,STRICT,13,0,9,0,0,0,0,0,0,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,0
 pyflakes,types-pyflakes,https://github.com/PyCQA/pyflakes,PARTIAL,-,434,UP_TO_DATE,UPLOADED,NOT_STRICT,265,69,206,2,0,0,4,3,75,33,0,74,0,0,MISSING_STUBS_IGNORED,linux,24
 pygit2,types-pygit2,https://github.com/libgit2/pygit2,COMPLETE,-,1928,UP_TO_DATE,UPLOADED,STRICT,674,0,503,0,0,0,3,0,474,0,1,119,0,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,11
 pyinstaller,types-pyinstaller,https://github.com/pyinstaller/pyinstaller,COMPLETE,-,703,OUT_OF_DATE,UPLOADED,STRICT,274,0,149,0,6,0,1,2,195,0,15,26,0,0,ERROR_ON_MISSING_STUB,linux,49
 pyjks,types-pyjks,https://github.com/kurtbrose/pyjks,COMPLETE,-,377,UP_TO_DATE,UPLOADED,STRICT,132,0,59,0,0,0,0,0,73,0,0,31,0,0,ERROR_ON_MISSING_STUB,linux,38
-pynput,types-pynput,https://github.com/moses-palmer/pynput,COMPLETE,-,324,OUT_OF_DATE,UPLOADED,STRICT,81,0,71,0,0,0,11,0,58,1,0,24,2,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,12
+pynput,types-pynput,https://github.com/moses-palmer/pynput,COMPLETE,-,324,UP_TO_DATE,UPLOADED,STRICT,82,0,71,0,0,0,11,0,122,1,0,24,2,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,12
 pyserial,types-pyserial,https://github.com/pyserial/pyserial,COMPLETE,-,1079,UP_TO_DATE,UPLOADED,STRICT,223,0,270,0,0,0,2,4,466,7,65,66,0,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,64
 pysftp,types-pysftp,https://bitbucket.org/dundeemt/pysftp,COMPLETE,-,166,UP_TO_DATE,UPLOADED,STRICT,109,0,70,0,0,0,0,0,6,0,0,6,0,0,ERROR_ON_MISSING_STUB,linux,0
 pytest-lazy-fixture,types-pytest-lazy-fixture,https://github.com/tvorog/pytest-lazy-fixture,COMPLETE,-,12,UP_TO_DATE,UPLOADED,STRICT,5,0,5,0,0,0,0,1,1,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,8
 python-crontab,types-python-crontab,https://gitlab.com/doctormo/python-crontab,COMPLETE,-,329,UP_TO_DATE,UPLOADED,NOT_STRICT,176,2,147,4,1,0,17,0,72,1,1,18,0,1,ERROR_ON_MISSING_STUB,linux,2
 python-datemath,types-python-datemath,https://github.com/nickmaccarthy/python-datemath,PARTIAL,-,16,UP_TO_DATE,UPLOADED,STRICT,16,0,4,0,0,1,0,0,0,0,0,1,0,0,MISSING_STUBS_IGNORED,linux,0
 python-dateutil,types-python-dateutil,https://github.com/dateutil/dateutil,PARTIAL,-,439,UP_TO_DATE,UPLOADED,NOT_STRICT,172,65,112,42,5,0,0,0,89,0,4,29,0,0,MISSING_STUBS_IGNORED,linux,11
 python-gflags,types-python-gflags,https://github.com/google/python-gflags,COMPLETE,-,251,UP_TO_DATE,UPLOADED,STRICT,186,0,98,0,0,0,39,9,19,2,0,27,0,0,ERROR_ON_MISSING_STUB,linux,1
@@ -125,26 +126,27 @@
 pytz,types-pytz,https://github.com/stub42/pytz,COMPLETE,-,133,UP_TO_DATE,UPLOADED,STRICT,69,0,51,0,2,0,2,0,29,0,0,16,0,0,ERROR_ON_MISSING_STUB,linux,4
 pywin32,types-pywin32,https://github.com/mhammond/pywin32,COMPLETE,-,34801,UP_TO_DATE,UPLOADED,NOT_STRICT,3800,3558,3865,1987,419,288,1,1,25095,0,2824,724,0,0,ERROR_ON_MISSING_STUB,win32,46
 pyxdg,types-pyxdg,https://github.com/takluyver/pyxdg,COMPLETE,-,860,UP_TO_DATE,UPLOADED,NOT_STRICT,511,1,297,0,2,0,0,0,165,0,1,31,0,0,ERROR_ON_MISSING_STUB,linux,2
 qrbill,types-qrbill,https://github.com/claudep/swiss-qr-bill,COMPLETE,-,172,UP_TO_DATE,UPLOADED,STRICT,96,0,31,0,0,0,0,4,33,0,0,4,0,0,ERROR_ON_MISSING_STUB,linux,2
 qrcode,types-qrcode,https://github.com/lincolnloop/python-qrcode,COMPLETE,-,524,UP_TO_DATE,UPLOADED,NOT_STRICT,109,174,109,60,14,2,2,1,166,0,91,40,0,0,ERROR_ON_MISSING_STUB,linux,8
 redis,types-redis,https://github.com/redis/redis-py,PARTIAL,"Note: Redis-py 5.0.0 added a py.typed file, but the inline annotations are incomplete. Continuing to use `types-redis` for the time being may lead to superior results.",6165,OUT_OF_DATE,UPLOADED,NOT_STRICT,3945,1223,1379,607,352,5,92,330,618,158,34,215,0,2,MISSING_STUBS_IGNORED,linux,67
 regex,types-regex,https://github.com/mrabarnett/mrab-regex,COMPLETE,-,750,UP_TO_DATE,UPLOADED,STRICT,431,0,114,0,0,0,25,16,4,0,0,7,0,0,ERROR_ON_MISSING_STUB,linux,13
-reportlab,types-reportlab,-,COMPLETE,-,7731,UP_TO_DATE,UPLOADED,NOT_STRICT,1790,2469,1470,1057,344,3,25,11,2699,6,1269,567,0,2,ERROR_ON_MISSING_STUB,linux,65
-requests,types-requests,https://github.com/psf/requests,COMPLETE,"Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.",1015,UP_TO_DATE,UPLOADED,NOT_STRICT,379,132,133,66,19,1,8,4,116,34,5,51,0,0,ERROR_ON_MISSING_STUB,linux,4
+reportlab,types-reportlab,-,COMPLETE,-,7851,UP_TO_DATE,UPLOADED,NOT_STRICT,1911,2344,1513,1017,325,3,26,12,2742,6,1218,576,0,2,ERROR_ON_MISSING_STUB,linux,66
+requests,types-requests,https://github.com/psf/requests,COMPLETE,"Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.",1033,UP_TO_DATE,UPLOADED,NOT_STRICT,384,130,135,65,19,4,8,1,125,17,22,53,0,0,ERROR_ON_MISSING_STUB,linux,4
 requests-oauthlib,types-requests-oauthlib,https://github.com/requests/requests-oauthlib,COMPLETE,-,268,UP_TO_DATE,UPLOADED,NOT_STRICT,115,20,45,4,50,3,1,0,25,1,7,13,0,0,ERROR_ON_MISSING_STUB,linux,0
 retry,types-retry,https://github.com/invl/retry,COMPLETE,-,28,UP_TO_DATE,UPLOADED,STRICT,17,0,2,0,0,0,2,0,1,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,3
 s2clientprotocol,types-s2clientprotocol,https://github.com/Blizzard/s2client-proto,COMPLETE,Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 3.6.1 on [s2client-proto 5.0.12.91115.0](https://github.com/Blizzard/s2client-proto/tree/c04df4adbe274858a4eb8417175ee32ad02fd609),5029,UP_TO_DATE,UPLOADED,STRICT,856,0,676,0,0,0,0,0,1864,0,0,239,0,0,ERROR_ON_MISSING_STUB,linux,1
 seaborn,types-seaborn,https://github.com/mwaskom/seaborn,COMPLETE,-,2587,UP_TO_DATE,UPLOADED,NOT_STRICT,1445,25,357,2,34,7,155,17,282,13,24,100,1,0,ERROR_ON_MISSING_STUB,linux,5
 setuptools,types-setuptools,https://github.com/pypa/setuptools,COMPLETE,-,3140,UP_TO_DATE,UPLOADED,STRICT_ON_SOME_FILES,1001,434,845,262,45,13,21,1,660,87,285,187,0,0,ERROR_ON_MISSING_STUB,linux;win32,109
+shapely,types-shapely,https://github.com/shapely/shapely,COMPLETE,-,2595,UP_TO_DATE,UPLOADED,NOT_STRICT,1423,390,710,0,0,0,14,15,169,0,1,42,0,0,ERROR_ON_MISSING_STUB,linux,3
 simplejson,types-simplejson,https://github.com/simplejson/simplejson,COMPLETE,-,277,UP_TO_DATE,UPLOADED,STRICT,180,0,24,0,0,0,46,6,49,7,0,6,0,0,ERROR_ON_MISSING_STUB,linux,11
 singledispatch,types-singledispatch,https://github.com/jaraco/singledispatch,COMPLETE,-,27,UP_TO_DATE,UPLOADED,STRICT,16,0,12,0,0,0,7,0,3,1,0,2,0,0,ERROR_ON_MISSING_STUB,linux,0
 six,types-six,https://github.com/benjaminp/six,COMPLETE,-,335,UP_TO_DATE,UPLOADED,STRICT,69,0,38,0,0,0,8,6,13,0,0,3,0,0,ERROR_ON_MISSING_STUB,linux,25
 slumber,types-slumber,https://github.com/samgiles/slumber,COMPLETE,-,74,UP_TO_DATE,UPLOADED,STRICT,43,0,25,0,0,0,11,5,9,0,0,15,0,0,ERROR_ON_MISSING_STUB,linux,2
-stdlib,-,https://github.com/python/cpython,STDLIB,-,56071,STDLIB,NOT_CURRENTLY_UPLOADED,STRICT_ON_SOME_FILES,26172,823,14406,368,74,11,1959,837,8258,535,152,2412,26,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,1423
+stdlib,-,https://github.com/python/cpython,STDLIB,-,56261,STDLIB,NOT_CURRENTLY_UPLOADED,STRICT_ON_SOME_FILES,26271,823,14434,368,74,11,1959,837,8272,535,152,2415,26,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,1381
 tabulate,types-tabulate,https://github.com/astanin/python-tabulate,COMPLETE,-,60,UP_TO_DATE,UPLOADED,STRICT,15,0,3,0,0,0,2,0,26,0,0,4,0,0,ERROR_ON_MISSING_STUB,linux,0
 tensorflow,types-tensorflow,https://github.com/tensorflow/tensorflow,PARTIAL,Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .,25535,UP_TO_DATE,UPLOADED,NOT_STRICT,5324,8,3033,4,23,58,60,34,5294,5,7,928,1,0,MISSING_STUBS_IGNORED,linux,51
 toml,types-toml,https://github.com/uiri/toml,COMPLETE,-,136,UP_TO_DATE,UPLOADED,STRICT,71,0,41,0,0,0,21,5,14,2,0,14,2,0,ERROR_ON_MISSING_STUB,linux,4
 toposort,types-toposort,https://gitlab.com/ericvsmith/toposort,COMPLETE,-,13,UP_TO_DATE,UPLOADED,STRICT,4,0,4,0,0,0,1,0,1,1,0,2,0,0,ERROR_ON_MISSING_STUB,linux,0
 tqdm,types-tqdm,https://github.com/tqdm/tqdm,COMPLETE,-,1379,UP_TO_DATE,UPLOADED,NOT_STRICT,811,146,164,27,38,8,1,1,100,0,74,36,0,0,ERROR_ON_MISSING_STUB,linux,2
 translationstring,types-translationstring,https://github.com/Pylons/translationstring,COMPLETE,-,73,UP_TO_DATE,UPLOADED,STRICT,62,0,18,0,0,0,6,1,4,1,0,7,0,0,ERROR_ON_MISSING_STUB,linux,4
 tree-sitter,types-tree-sitter,https://github.com/tree-sitter/py-tree-sitter,COMPLETE,-,123,OBSOLETE,UPLOADED,STRICT,25,0,52,0,0,0,0,2,4,0,0,7,0,0,ERROR_ON_MISSING_STUB,linux,36
```

### Comparing `typeshed_stats-24.5.26/examples/example.json` & `typeshed_stats-24.6.2/examples/example.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9850538517707194%*

 * *Differences: {'112': "{'package_status': 'UP_TO_DATE', 'annotation_stats': {'annotated_parameters': 82, "*

 * *        "'annotated_variables': 122}}",*

 * * '131': "{'number_of_lines': 7851, 'stubtest_settings': {'allowlist_length': 66}, "*

 * *        "'annotation_stats': {'annotated_parameters': 1911, 'unannotated_parameters': 2344, "*

 * *        "'annotated_returns': 1513, 'unannotated_returns': 1017, 'explicit_Incomplete_parameters': "*

 * *        "325, 'explicit_Any_parameters': 26, 'explicit_Any_returns': 12, 'annotated_variables': "*

 * *   […]*

```diff
@@ -1361,34 +1361,34 @@
             "strictness": "MISSING_STUBS_IGNORED"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/tiran/defusedxml"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 782,
-            "annotated_returns": 292,
-            "annotated_variables": 206,
-            "classdefs": 128,
+            "annotated_parameters": 801,
+            "annotated_returns": 294,
+            "annotated_variables": 210,
+            "classdefs": 131,
             "classdefs_with_Any": 2,
             "classdefs_with_Incomplete": 24,
             "explicit_Any_parameters": 19,
             "explicit_Any_returns": 25,
             "explicit_Any_variables": 2,
             "explicit_Incomplete_parameters": 315,
             "explicit_Incomplete_returns": 7,
             "explicit_Incomplete_variables": 83,
-            "unannotated_parameters": 376,
-            "unannotated_returns": 270
+            "unannotated_parameters": 373,
+            "unannotated_returns": 269
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
-        "number_of_lines": 1899,
+        "number_of_lines": 1936,
         "package_name": "docker",
-        "package_status": "OUT_OF_DATE",
+        "package_status": "UP_TO_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-docker",
         "stubtest_settings": {
             "allowlist_length": 7,
             "platforms": [
                 "linux"
             ],
@@ -2689,15 +2689,49 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/PyMySQL/mysqlclient"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 286,
+            "annotated_parameters": 8,
+            "annotated_returns": 4,
+            "annotated_variables": 2,
+            "classdefs": 0,
+            "classdefs_with_Any": 0,
+            "classdefs_with_Incomplete": 0,
+            "explicit_Any_parameters": 0,
+            "explicit_Any_returns": 0,
+            "explicit_Any_variables": 0,
+            "explicit_Incomplete_parameters": 0,
+            "explicit_Incomplete_returns": 0,
+            "explicit_Incomplete_variables": 0,
+            "unannotated_parameters": 0,
+            "unannotated_returns": 0
+        },
+        "completeness_level": "COMPLETE",
+        "extra_description": null,
+        "number_of_lines": 16,
+        "package_name": "nanoid",
+        "package_status": "UP_TO_DATE",
+        "pyright_setting": "STRICT",
+        "stub_distribution_name": "types-nanoid",
+        "stubtest_settings": {
+            "allowlist_length": 0,
+            "platforms": [
+                "linux"
+            ],
+            "strictness": "ERROR_ON_MISSING_STUB"
+        },
+        "upload_status": "UPLOADED",
+        "upstream_url": "https://github.com/puyuan/py-nanoid"
+    },
+    {
+        "annotation_stats": {
+            "annotated_parameters": 288,
             "annotated_returns": 308,
             "annotated_variables": 101,
             "classdefs": 43,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 1,
             "explicit_Any_returns": 1,
@@ -2706,15 +2740,15 @@
             "explicit_Incomplete_returns": 0,
             "explicit_Incomplete_variables": 2,
             "unannotated_parameters": 4,
             "unannotated_returns": 0
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
-        "number_of_lines": 696,
+        "number_of_lines": 698,
         "package_name": "netaddr",
         "package_status": "UP_TO_DATE",
         "pyright_setting": "STRICT_ON_SOME_FILES",
         "stub_distribution_name": "types-netaddr",
         "stubtest_settings": {
             "allowlist_length": 2,
             "platforms": [
@@ -2723,16 +2757,16 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/drkjam/netaddr"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 1959,
-            "annotated_returns": 503,
+            "annotated_parameters": 1961,
+            "annotated_returns": 504,
             "annotated_variables": 320,
             "classdefs": 126,
             "classdefs_with_Any": 1,
             "classdefs_with_Incomplete": 2,
             "explicit_Any_parameters": 4,
             "explicit_Any_returns": 3,
             "explicit_Any_variables": 2,
@@ -2740,15 +2774,15 @@
             "explicit_Incomplete_returns": 102,
             "explicit_Incomplete_variables": 249,
             "unannotated_parameters": 1511,
             "unannotated_returns": 808
         },
         "completeness_level": "PARTIAL",
         "extra_description": null,
-        "number_of_lines": 4781,
+        "number_of_lines": 4784,
         "package_name": "networkx",
         "package_status": "OUT_OF_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-networkx",
         "stubtest_settings": {
             "allowlist_length": 13,
             "platforms": [
@@ -2844,15 +2878,15 @@
             "unannotated_parameters": 341,
             "unannotated_returns": 91
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
         "number_of_lines": 13238,
         "package_name": "openpyxl",
-        "package_status": "UP_TO_DATE",
+        "package_status": "OUT_OF_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-openpyxl",
         "stubtest_settings": {
             "allowlist_length": 183,
             "platforms": [
                 "linux"
             ],
@@ -3785,17 +3819,17 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/kurtbrose/pyjks"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 81,
+            "annotated_parameters": 82,
             "annotated_returns": 71,
-            "annotated_variables": 58,
+            "annotated_variables": 122,
             "classdefs": 24,
             "classdefs_with_Any": 2,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 11,
             "explicit_Any_returns": 0,
             "explicit_Any_variables": 1,
             "explicit_Incomplete_parameters": 0,
@@ -3804,15 +3838,15 @@
             "unannotated_parameters": 0,
             "unannotated_returns": 0
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
         "number_of_lines": 324,
         "package_name": "pynput",
-        "package_status": "OUT_OF_DATE",
+        "package_status": "UP_TO_DATE",
         "pyright_setting": "STRICT",
         "stub_distribution_name": "types-pynput",
         "stubtest_settings": {
             "allowlist_length": 12,
             "platforms": [
                 "darwin",
                 "linux",
@@ -4435,66 +4469,66 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/mrabarnett/mrab-regex"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 1790,
-            "annotated_returns": 1470,
-            "annotated_variables": 2699,
-            "classdefs": 567,
+            "annotated_parameters": 1911,
+            "annotated_returns": 1513,
+            "annotated_variables": 2742,
+            "classdefs": 576,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 2,
-            "explicit_Any_parameters": 25,
-            "explicit_Any_returns": 11,
+            "explicit_Any_parameters": 26,
+            "explicit_Any_returns": 12,
             "explicit_Any_variables": 6,
-            "explicit_Incomplete_parameters": 344,
+            "explicit_Incomplete_parameters": 325,
             "explicit_Incomplete_returns": 3,
-            "explicit_Incomplete_variables": 1269,
-            "unannotated_parameters": 2469,
-            "unannotated_returns": 1057
+            "explicit_Incomplete_variables": 1218,
+            "unannotated_parameters": 2344,
+            "unannotated_returns": 1017
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
-        "number_of_lines": 7731,
+        "number_of_lines": 7851,
         "package_name": "reportlab",
         "package_status": "UP_TO_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-reportlab",
         "stubtest_settings": {
-            "allowlist_length": 65,
+            "allowlist_length": 66,
             "platforms": [
                 "linux"
             ],
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": null
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 379,
-            "annotated_returns": 133,
-            "annotated_variables": 116,
-            "classdefs": 51,
+            "annotated_parameters": 384,
+            "annotated_returns": 135,
+            "annotated_variables": 125,
+            "classdefs": 53,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 8,
-            "explicit_Any_returns": 4,
-            "explicit_Any_variables": 34,
+            "explicit_Any_returns": 1,
+            "explicit_Any_variables": 17,
             "explicit_Incomplete_parameters": 19,
-            "explicit_Incomplete_returns": 1,
-            "explicit_Incomplete_variables": 5,
-            "unannotated_parameters": 132,
-            "unannotated_returns": 66
+            "explicit_Incomplete_returns": 4,
+            "explicit_Incomplete_variables": 22,
+            "unannotated_parameters": 130,
+            "unannotated_returns": 65
         },
         "completeness_level": "COMPLETE",
         "extra_description": "Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.",
-        "number_of_lines": 1015,
+        "number_of_lines": 1033,
         "package_name": "requests",
         "package_status": "UP_TO_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-requests",
         "stubtest_settings": {
             "allowlist_length": 4,
             "platforms": [
@@ -4674,14 +4708,48 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/pypa/setuptools"
     },
     {
         "annotation_stats": {
+            "annotated_parameters": 1423,
+            "annotated_returns": 710,
+            "annotated_variables": 169,
+            "classdefs": 42,
+            "classdefs_with_Any": 0,
+            "classdefs_with_Incomplete": 0,
+            "explicit_Any_parameters": 14,
+            "explicit_Any_returns": 15,
+            "explicit_Any_variables": 0,
+            "explicit_Incomplete_parameters": 0,
+            "explicit_Incomplete_returns": 0,
+            "explicit_Incomplete_variables": 1,
+            "unannotated_parameters": 390,
+            "unannotated_returns": 0
+        },
+        "completeness_level": "COMPLETE",
+        "extra_description": null,
+        "number_of_lines": 2595,
+        "package_name": "shapely",
+        "package_status": "UP_TO_DATE",
+        "pyright_setting": "NOT_STRICT",
+        "stub_distribution_name": "types-shapely",
+        "stubtest_settings": {
+            "allowlist_length": 3,
+            "platforms": [
+                "linux"
+            ],
+            "strictness": "ERROR_ON_MISSING_STUB"
+        },
+        "upload_status": "UPLOADED",
+        "upstream_url": "https://github.com/shapely/shapely"
+    },
+    {
+        "annotation_stats": {
             "annotated_parameters": 180,
             "annotated_returns": 24,
             "annotated_variables": 49,
             "classdefs": 6,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 46,
@@ -4810,38 +4878,38 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/samgiles/slumber"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 26172,
-            "annotated_returns": 14406,
-            "annotated_variables": 8258,
-            "classdefs": 2412,
+            "annotated_parameters": 26271,
+            "annotated_returns": 14434,
+            "annotated_variables": 8272,
+            "classdefs": 2415,
             "classdefs_with_Any": 26,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 1959,
             "explicit_Any_returns": 837,
             "explicit_Any_variables": 535,
             "explicit_Incomplete_parameters": 74,
             "explicit_Incomplete_returns": 11,
             "explicit_Incomplete_variables": 152,
             "unannotated_parameters": 823,
             "unannotated_returns": 368
         },
         "completeness_level": "STDLIB",
         "extra_description": null,
-        "number_of_lines": 56071,
+        "number_of_lines": 56261,
         "package_name": "stdlib",
         "package_status": "STDLIB",
         "pyright_setting": "STRICT_ON_SOME_FILES",
         "stub_distribution_name": "-",
         "stubtest_settings": {
-            "allowlist_length": 1423,
+            "allowlist_length": 1381,
             "platforms": [
                 "darwin",
                 "linux",
                 "win32"
             ],
             "strictness": "ERROR_ON_MISSING_STUB"
         },
```

### Comparing `typeshed_stats-24.5.26/examples/example.md` & `typeshed_stats-24.6.2/examples/example.md`

 * *Files 1% similar despite different names*

```diff
@@ -2284,19 +2284,19 @@
 
 ### Stub distribution name
 
 `types-docker`
 
 ### Number of lines
 
-1,899 (excluding blank lines)
+1,936 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
@@ -2309,29 +2309,29 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `docker`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 782
-    - Unannotated parameters: 376
+    - Annotated parameters: 801
+    - Unannotated parameters: 373
     - Explicit `Any` parameters: 19
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 315
 - Returns:
-    - Annotated returns: 292
-    - Unannotated returns: 270
+    - Annotated returns: 294
+    - Unannotated returns: 269
     - Explicit `Any` returns: 25
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
 - Variables:
-    - Annotated variables: 206
+    - Annotated variables: 210
     - Explicit `Any` variables: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 83
 - Class definitions:
-    - Total class definitions: 128
+    - Total class definitions: 131
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 24
 
 ---
 
 ## Info on typeshed's stubs for `dockerfile-parse`
 
@@ -4499,27 +4499,84 @@
 - Class definitions:
     - Total class definitions: 35
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 1
 
 ---
 
+## Info on typeshed's stubs for `nanoid`
+
+### Upstream repo URL
+
+[https://github.com/puyuan/py-nanoid](https://github.com/puyuan/py-nanoid)
+
+### Stub distribution name
+
+`types-nanoid`
+
+### Number of lines
+
+16 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 0 allowlist entries for `nanoid` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `nanoid`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 8
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 4
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 2
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 0
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `netaddr`
 
 ### Upstream repo URL
 
 [https://github.com/drkjam/netaddr](https://github.com/drkjam/netaddr)
 
 ### Stub distribution name
 
 `types-netaddr`
 
 ### Number of lines
 
-696 (excluding blank lines)
+698 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4536,15 +4593,15 @@
 ### Pyright settings in CI: *strict on some files*
 
 Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for `netaddr`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 286
+    - Annotated parameters: 288
     - Unannotated parameters: 4
     - Explicit `Any` parameters: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
 - Returns:
     - Annotated returns: 308
     - Unannotated returns: 0
     - Explicit `Any` returns: 1
@@ -4568,15 +4625,15 @@
 
 ### Stub distribution name
 
 `types-networkx`
 
 ### Number of lines
 
-4,781 (excluding blank lines)
+4,784 (excluding blank lines)
 
 ### Package status: *out of date*
 
 These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
@@ -4593,20 +4650,20 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `networkx`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 1,959
+    - Annotated parameters: 1,961
     - Unannotated parameters: 1,511
     - Explicit `Any` parameters: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 763
 - Returns:
-    - Annotated returns: 503
+    - Annotated returns: 504
     - Unannotated returns: 808
     - Explicit `Any` returns: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 102
 - Variables:
     - Annotated variables: 320
     - Explicit `Any` variables: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 249
@@ -4741,17 +4798,17 @@
 
 `types-openpyxl`
 
 ### Number of lines
 
 13,238 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *out of date*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
@@ -6341,17 +6398,17 @@
 
 `types-pynput`
 
 ### Number of lines
 
 324 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
@@ -6364,25 +6421,25 @@
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pynput`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 81
+    - Annotated parameters: 82
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 11
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 71
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 58
+    - Annotated variables: 122
     - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 24
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
@@ -7422,15 +7479,15 @@
 
 ### Stub distribution name
 
 `types-reportlab`
 
 ### Number of lines
 
-7,731 (excluding blank lines)
+7,851 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7438,38 +7495,38 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 65 unique allowlist entries for `reportlab` when running stubtest in CI.
+Typeshed currently has 66 unique allowlist entries for `reportlab` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `reportlab`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 1,790
-    - Unannotated parameters: 2,469
-    - Explicit `Any` parameters: 25
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 344
+    - Annotated parameters: 1,911
+    - Unannotated parameters: 2,344
+    - Explicit `Any` parameters: 26
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 325
 - Returns:
-    - Annotated returns: 1,470
-    - Unannotated returns: 1,057
-    - Explicit `Any` returns: 11
+    - Annotated returns: 1,513
+    - Unannotated returns: 1,017
+    - Explicit `Any` returns: 12
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 3
 - Variables:
-    - Annotated variables: 2,699
+    - Annotated variables: 2,742
     - Explicit `Any` variables: 6
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1,269
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1,218
 - Class definitions:
-    - Total class definitions: 567
+    - Total class definitions: 576
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 2
 
 ---
 
 ## Info on typeshed's stubs for `requests`
 
@@ -7483,15 +7540,15 @@
 
 ### Stub distribution name
 
 `types-requests`
 
 ### Number of lines
 
-1,015 (excluding blank lines)
+1,033 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7508,29 +7565,29 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `requests`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 379
-    - Unannotated parameters: 132
+    - Annotated parameters: 384
+    - Unannotated parameters: 130
     - Explicit `Any` parameters: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 19
 - Returns:
-    - Annotated returns: 133
-    - Unannotated returns: 66
-    - Explicit `Any` returns: 4
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Annotated returns: 135
+    - Unannotated returns: 65
+    - Explicit `Any` returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
 - Variables:
-    - Annotated variables: 116
-    - Explicit `Any` variables: 34
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 5
+    - Annotated variables: 125
+    - Explicit `Any` variables: 17
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 22
 - Class definitions:
-    - Total class definitions: 51
+    - Total class definitions: 53
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `requests-oauthlib`
 
@@ -7817,14 +7874,71 @@
 - Class definitions:
     - Total class definitions: 187
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `shapely`
+
+### Upstream repo URL
+
+[https://github.com/shapely/shapely](https://github.com/shapely/shapely)
+
+### Stub distribution name
+
+`types-shapely`
+
+### Number of lines
+
+2,595 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 3 unique allowlist entries for `shapely` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `shapely`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 1,423
+    - Unannotated parameters: 390
+    - Explicit `Any` parameters: 14
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 710
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 15
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 169
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+- Class definitions:
+    - Total class definitions: 42
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `simplejson`
 
 ### Upstream repo URL
 
 [https://github.com/simplejson/simplejson](https://github.com/simplejson/simplejson)
 
 ### Stub distribution name
@@ -8053,15 +8167,15 @@
 
 ### Upstream repo URL
 
 [https://github.com/python/cpython](https://github.com/python/cpython)
 
 ### Number of lines
 
-56,071 (excluding blank lines)
+56,261 (excluding blank lines)
 
 ### Package status: *stdlib*
 
 These are typeshed's stubs for the standard library. Typeshed's stdlib stubs are generally fairly up to date, and are tested against all currently supported Python versions in typeshed's CI.
 
 ### Upload status: *not currently uploaded*
 
@@ -8069,38 +8183,38 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
-Typeshed currently has 1,423 unique allowlist entries for the stdlib when running stubtest in CI.
+Typeshed currently has 1,381 unique allowlist entries for the stdlib when running stubtest in CI.
 
 ### Pyright settings in CI: *strict on some files*
 
 Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for the stdlib
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 26,172
+    - Annotated parameters: 26,271
     - Unannotated parameters: 823
     - Explicit `Any` parameters: 1,959
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 74
 - Returns:
-    - Annotated returns: 14,406
+    - Annotated returns: 14,434
     - Unannotated returns: 368
     - Explicit `Any` returns: 837
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 11
 - Variables:
-    - Annotated variables: 8,258
+    - Annotated variables: 8,272
     - Explicit `Any` variables: 535
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 152
 - Class definitions:
-    - Total class definitions: 2,412
+    - Total class definitions: 2,415
     - Class definitions with `Any`: 26
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `tabulate`
```

### Comparing `typeshed_stats-24.5.26/scripts/regenerate.py` & `typeshed_stats-24.6.2/scripts/regenerate.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/scripts/runtests.py` & `typeshed_stats-24.6.2/scripts/runtests.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/src/typeshed_stats/_cli.py` & `typeshed_stats-24.6.2/src/typeshed_stats/_cli.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/src/typeshed_stats/_markdown_template.md.jinja` & `typeshed_stats-24.6.2/src/typeshed_stats/_markdown_template.md.jinja`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/src/typeshed_stats/gather.py` & `typeshed_stats-24.6.2/src/typeshed_stats/gather.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/src/typeshed_stats/serialize.py` & `typeshed_stats-24.6.2/src/typeshed_stats/serialize.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/stats_website/big_logo.png` & `typeshed_stats-24.6.2/stats_website/big_logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/stats_website/gather.md` & `typeshed_stats-24.6.2/stats_website/gather.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/stats_website/logo.png` & `typeshed_stats-24.6.2/stats_website/logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/stats_website/stats-csv.md` & `typeshed_stats-24.6.2/stats_website/stats-csv.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/stats_website/.snippets/links.md` & `typeshed_stats-24.6.2/stats_website/.snippets/links.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/stats_website/javascripts/filtertable.js` & `typeshed_stats-24.6.2/stats_website/javascripts/filtertable.js`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/tests/conftest.py` & `typeshed_stats-24.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/tests/test___all__.py` & `typeshed_stats-24.6.2/tests/test___all__.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/tests/test__cli.py` & `typeshed_stats-24.6.2/tests/test__cli.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/tests/test_gather.py` & `typeshed_stats-24.6.2/tests/test_gather.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/tests/test_running_from_command_line.py` & `typeshed_stats-24.6.2/tests/test_running_from_command_line.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/tests/test_serialize.py` & `typeshed_stats-24.6.2/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/.gitignore` & `typeshed_stats-24.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/LICENSE` & `typeshed_stats-24.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/README.md` & `typeshed_stats-24.6.2/README.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/pyproject.toml` & `typeshed_stats-24.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.26/PKG-INFO` & `typeshed_stats-24.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typeshed_stats
-Version: 24.5.26
+Version: 24.6.2
 Summary: Library and command-line tool to gather stats on typeshed packages
 Project-URL: Homepage, https://github.com/AlexWaygood/typeshed-stats
 Project-URL: Bug Tracker, https://github.com/AlexWaygood/typeshed-stats/issues
 Author-email: Alex Waygood <alex.waygood@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: stubs,typeshed,typing
```

