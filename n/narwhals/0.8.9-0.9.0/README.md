# Comparing `tmp/narwhals-0.8.9.tar.gz` & `tmp/narwhals-0.9.0.tar.gz`

## Comparing `narwhals-0.8.9.tar` & `narwhals-0.9.0.tar`

### file list

```diff
@@ -1,124 +1,152 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.9/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.9/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.9/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/requirements-docs.txt
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/why.md
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/index.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/series.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.9/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/__init__.py
--rw-r--r--   0        0        0    96138 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/dependencies.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/dtypes.py
--rw-r--r--   0        0        0    39888 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/functions.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/py.typed
--rw-r--r--   0        0        0    16770 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/typing.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    16520 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    14015 2020-02-02 00:00:00.000000 narwhals-0.8.9/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/conftest.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/group_by_test.py
--rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_common.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/cum_sum_test.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/diff_test.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/fill_null_test.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/over_test.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/shift_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/str/head_test.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/frame/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/frame/drop_nulls_test.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/frame/pipe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.9/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.9/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.9/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.9/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.9/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.9/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.9/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.9/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 narwhals-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 narwhals-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 narwhals-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.9.0/requirements-dev.txt
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/ISSUE_TEMPLATE/doc_issue.yml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.9.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/generate_members.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/how_it_works.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/installation.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/quick_start.md
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/why.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/group_by.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/index.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/selectors.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/series.md
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.9.0/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/__init__.py
+-rw-r--r--   0        0        0    98383 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/dataframe.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/dtypes.py
+-rw-r--r--   0        0        0    94785 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/expression.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/functions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/py.typed
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/selectors.py
+-rw-r--r--   0        0        0    67336 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/series.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/typing.py
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/selectors.py
+-rw-r--r--   0        0        0    21404 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    16759 2020-02-02 00:00:00.000000 narwhals-0.9.0/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/group_by_test.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/selectors_test.py
+-rw-r--r--   0        0        0    24366 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_common.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_group_by.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_invalid.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_pandas.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/utils.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/utils_test.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/filter_test.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/is_between_test.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/is_duplicated_test.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/is_first_distinct_test.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/is_last_distinct_test.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/is_unique_test.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/n_unique_test.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/null_count_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/over_test.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/shift_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/drop_nulls_test.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/len_test.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/pipe_test.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/schema_test.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/slice_test.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/with_columns_sequence_test.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/frame/with_row_index_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/series/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/series/eq_ne_test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 narwhals-0.9.0/tests/series/to_frame_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.9.0/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.9.0/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.9.0/utils/bump_version.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 narwhals-0.9.0/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 narwhals-0.9.0/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 narwhals-0.9.0/PKG-INFO
```

### Comparing `narwhals-0.8.9/.pre-commit-config.yaml` & `narwhals-0.9.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 repos:
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.4.3'
+  rev: 'v0.4.5'
   hooks:
     # Run the formatter.
     - id: ruff-format
     # Run the linter.
     - id: ruff
       args: [--fix]
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v1.10.0'
   hooks:
     - id: mypy
       additional_dependencies: ['polars==0.20.10', 'pytest==8.0.1']
       exclude: utils|tpch
 - repo: https://github.com/codespell-project/codespell
-  rev: 'v2.2.6'
+  rev: 'v2.3.0'
   hooks:
     - id: codespell
       files: \.(py|rst|md)$
       args: [--ignore-words-list=ser]
 - repo: local
   hooks:
     - id: check-api-reference
       name: check-api-reference
       pass_filenames: false
       entry: python -m utils.check_api_reference
       language: python
       additional_dependencies: [polars]
-
+    - id: imports-are-banned
+      name: import are banned (use `get_pandas` instead of `import pandas`)
+      entry: (?<!>>> )import (pandas|polars|modin|cudf)
+      language: pygrep
+      files: ^narwhals/
```

### Comparing `narwhals-0.8.9/CONTRIBUTING.md` & `narwhals-0.9.0/CONTRIBUTING.md`

 * *Files 7% similar despite different names*

```diff
@@ -26,10 +26,15 @@
 
 ## Building docs
 
 To build the docs, run `mkdocs serve`, and then open the link provided in a browser.
 The docs should refresh when you make changes. If they don't, press `ctrl+C`, and then
 do `mkdocs build` and then `mkdocs serve`.
 
+## How it works
+
+If Narwhals looks like underwater unicorn magic to you, then please read
+[how it works](https://narwhals-dev.github.io/narwhals/roadmap/).
+
 ## Happy contributing!
 
 Please remember to abide by the code of conduct, else you'll be conducted away from this project.
```

### Comparing `narwhals-0.8.9/mkdocs.yml` & `narwhals-0.9.0/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 site_name: Narwhals
-repo_url: https://github.com/MarcoGorelli/narwhals.git
+repo_url: https://github.com/narwhals-dev/narwhals.git
 nav:
   - Home: index.md
   - Why: why.md
   - Installation: installation.md
   - Quick start: quick_start.md
   - Tutorial:
     - basics/dataframe.md
     - basics/column.md
     - basics/complete_example.md
   - Other concepts:
     - other/pandas_index.md
   - extending.md
+  - how_it_works.md
   - Roadmap: roadmap.md
   - Related projects: related.md
   - API Reference:
     - api-reference/index.md
     - api-reference/narwhals.md
     - api-reference/dataframe.md
     - api-reference/lazyframe.md
@@ -23,14 +24,16 @@
     - api-reference/series_dt.md
     - api-reference/series_str.md
     - api-reference/expressions.md
     - api-reference/expressions_dt.md
     - api-reference/expressions_str.md
     - api-reference/dtypes.md
     - api-reference/dependencies.md
+    - api-reference/selectors.md
+    - api-reference/group_by.md
 theme:
   name: material
   font: false
   features:
     - content.code.copy
     - content.code.annotate
     - navigation.footer
```

### Comparing `narwhals-0.8.9/.github/CODE_OF_CONDUCT.md` & `narwhals-0.9.0/.github/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Contributor Covenant Code of Conduct
 
 ## Our Pledge
 
 We as members, contributors, and leaders pledge to make participation in our
 community a harassment-free experience for everyone, regardless of age, body
 size, visible or invisible disability, ethnicity, sex characteristics, gender
-identity and expression, level of experience, education, socio-economic status,
+identity and expression, level of experience, education, socioeconomic status,
 nationality, personal appearance, race, religion, or sexual identity
 and orientation.
 
 We pledge to act and interact in ways that contribute to an open, welcoming,
 diverse, inclusive, and healthy community.
 
 ## Our Standards
```

### Comparing `narwhals-0.8.9/.github/workflows/extremes.yml` & `narwhals-0.9.0/.github/workflows/extremes.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             ~/.cache/pip
             $RUNNER_TOOL_CACHE/Python/*
             ~\AppData\Local\pip\Cache
           key: ${{ runner.os }}-build-${{ matrix.python-version }}
       - name: install-reqs
         run: python -m pip install --upgrade tox virtualenv setuptools pip -r requirements-dev.txt
       - name: install-modin
-        run: python -m pip install pandas==1.1.5 polars==0.20.3
+        run: python -m pip install pandas==1.1.5 polars==0.20.3 "numpy<=1.21"
       - name: Run pytest
         run: pytest tests --cov=narwhals --cov=tests --cov-fail-under=50 --runslow
       - name: Run doctests
         run: pytest narwhals --doctest-modules
 
   pandas-nightly:
     strategy:
```

### Comparing `narwhals-0.8.9/.github/workflows/mkdocs.yml` & `narwhals-0.9.0/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/.github/workflows/publish_to_pypi.yml` & `narwhals-0.9.0/.github/workflows/publish_to_pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Install pypa/build
       run: >-
         python3 -m
         pip install
         build
@@ -64,15 +64,15 @@
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `narwhals-0.8.9/.github/workflows/pytest.yml` & `narwhals-0.9.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/extending.md` & `narwhals-0.9.0/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/generate_members.py` & `narwhals-0.9.0/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/index.md` & `narwhals-0.9.0/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 - ✅ **Just use** a subset of **the Polars API**, no need to learn anything new
 - ✅ **No dependencies** (not even Polars), keep your library lightweight
 - ✅ Support both **lazy** and eager execution
 - ✅ Use **Expressions**
 - ✅ Tested against pandas and Polars nightly builds!
 - ✅ Preserve your Index (if present) without it getting in the way!
+- ✅ **Zero 3rd party imports**, Narwhals only uses what you already have!
 
 ## Who's this for?
 
 Anyone wishing to write a library/application/service which consumes dataframes, and wishing to make it
 completely dataframe-agnostic.
 
 Let's get started!
```

### Comparing `narwhals-0.8.9/docs/quick_start.md` & `narwhals-0.9.0/docs/quick_start.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Quick start
 
 ## Prerequisites
 
 Please start by following the [installation instructions](installation.md).
 
-Then, please install the following:
+To follow along with the examples which follow, please install the following (though note that
+they are not required dependencies - Narwhals only ever uses what the user passes in):
 
 - [pandas](https://pandas.pydata.org/docs/getting_started/install.html)
 - [Polars](https://pola-rs.github.io/polars/user-guide/installation/)
 
 ## Simple example
 
 Create a Python file `t.py` with the following content:
```

### Comparing `narwhals-0.8.9/docs/related.md` & `narwhals-0.9.0/docs/related.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 Standardised way of interchanging data between libraries, see
 [here](https://data-apis.org/dataframe-protocol/latest/index.html).
 
 ## DataFrame API Standard
 
 Project which aims to "provide a standard interface that encapsulates implementation details of dataframe libraries. This will allow users and third-party libraries to write code that interacts and operates with a standard dataframe, and not with specific implementations.", see [here](https://data-apis.org/dataframe-api/draft/).
 
+The Narwhals author was originally involved, but left due to irreconcilable differences in vision.
+
 Some notable difference are:
 
 - Narwhals just uses a subset of the Polars API, whereas the dataframe standard introduces a new API
-- Narwhals supports expressions and separates lazy and eager execution
+- Narwhals supports expressions, and separates lazy and eager execution
 - Narwhals is a standalone, independent project, whereas the dataframe standard aims to be upstreamed
   and implemented by major dataframe libraries.
 
-The projects are not in competition and have different goals.
-
 ## Ibis
 
 [Presents itself as a dataframe standard](https://voltrondata.com/resources/open-source-standards), and
 dispatches to 20+ backends. Some differences with Narwhals are:
 
-- Narwhals is ~1000 times lighter
+- Narwhals is aimed at library maintainers, Ibis more to end users
+- Narwhals has zero required dependencies, whereas Ibis requires pandas and PyArrow. For users starting
+  from non-pandas environments, the difference in the relative size increase is ~1000x
 - Narwhals only supports 4 backends, Ibis more than 20
-- Narwhals is limited to fundamental dataframe operations, Ibis includes more advanced and niche ones.
+- Narwhals is focused on fundamental dataframe operations, Ibis on SQL backends
 
-Again, the projects are not in competition and have different goals.
+The projects are not in competition and have different goals.
 
 ## Array API
 
 Array counterpart to the DataFrame API, see [here](https://data-apis.org/array-api/2022.12/index.html).
```

### Comparing `narwhals-0.8.9/docs/roadmap.md` & `narwhals-0.9.0/docs/roadmap.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,16 +15,10 @@
 Currently, it can execute the first 7.
 
 ## Other backends?
 
 Narwhals is extesible - can we make it as easy as possible for backends to become
 compatible with it?
 
-## Query optimisation
-
-Can we insert a light layer to do some simple query optimisation for pandas?
-
 ## Use cases
 
-We're currently investigating whether we can make scikit-lego dataframe-agnostic.
-
-Ideas for other projects we could support? If so, please post them [here](https://github.com/narwhals-dev/narwhals/issues/62).
+Ideas for other projects where Narwhals might be useful? If so, please post them [here](https://github.com/narwhals-dev/narwhals/issues/62).
```

### Comparing `narwhals-0.8.9/docs/why.md` & `narwhals-0.9.0/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/api-reference/index.md` & `narwhals-0.9.0/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/api-reference/series.md` & `narwhals-0.9.0/docs/api-reference/expressions.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-# `narwhals.Series`
+# `narwhals.Expr`
 
-::: narwhals.series.Series
+::: narwhals.Expr
     handler: python
     options:
       members:
         - alias
         - all
         - any
         - cast
         - cum_sum
         - diff
         - drop_nulls
-        - dtype
         - fill_null
         - filter
         - is_between
+        - is_duplicated
+        - is_first_distinct
         - is_in
+        - is_last_distinct
         - is_null
+        - is_unique
         - max
         - mean
         - min
-        - name
+        - null_count
         - n_unique
+        - over
+        - quantile
         - sample
-        - shape
         - shift
         - sort
         - std
         - sum
-        - to_numpy
-        - to_pandas
         - unique
       show_source: false
       show_bases: false
```

### Comparing `narwhals-0.8.9/docs/assets/image.png` & `narwhals-0.9.0/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/basics/column.md` & `narwhals-0.9.0/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/basics/complete_example.md` & `narwhals-0.9.0/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/docs/basics/dataframe.md` & `narwhals-0.9.0/docs/basics/dataframe.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,20 @@
 `DataFrame.select` or `LazyFrame.select`.
 
 Make a Python file with the following content:
 ```python exec="1" source="above" session="df_ex1"
 import narwhals as nw
 
 def func(df_any):
-    # 1. Create a Narwhals dataframe
     df = nw.from_native(df_any)
-    # 2. Use the subset of the Polars API supported by Narwhals
     df = df.select(
         a_sum=nw.col('a').sum(),
         a_mean=nw.col('a').mean(),
         a_std=nw.col('a').std(),
     )
-    # 3. Return a library from the user's original library
     return nw.to_native(df)
 ```
 Let's try it out:
 
 === "pandas"
     ```python exec="true" source="material-block" result="python" session="df_ex1"
     import pandas as pd
@@ -58,24 +55,22 @@
     df = pl.LazyFrame({'a': [1, 1, 2]})
     print(func(df).collect())
     ```
 
 
 ## Example 2: group-by and mean
 
+Just like in Polars, we can pass expressions to `GroupBy.agg`.
 Make a Python file with the following content:
 ```python exec="1" source="above" session="df_ex2"
 import narwhals as nw
 
 def func(df_any):
-    # 1. Create a Narwhals dataframe
     df = nw.from_native(df_any)
-    # 2. Use the subset of the Polars API supported by Narwhals
     df = df.group_by('a').agg(nw.col('b').mean()).sort('a')
-    # 3. Return a library from the user's original library
     return nw.to_native(df)
 ```
 Let's try it out:
 
 === "pandas"
     ```python exec="true" source="material-block" result="python" session="df_ex2"
     import pandas as pd
@@ -107,19 +102,16 @@
 sum using `nw.sum_horizontal`.
 
 Make a Python file with the following content:
 ```python exec="1" source="above" session="df_ex3"
 import narwhals as nw
 
 def func(df_any):
-    # 1. Create a Narwhals dataframe
     df = nw.from_native(df_any)
-    # 2. Use the subset of the Polars API supported by Narwhals
     df = df.with_columns(a_plus_b=nw.sum_horizontal('a', 'b'))
-    # 3. Return a library from the user's original library
     return nw.to_native(df)
 ```
 Let's try it out:
 
 === "pandas"
     ```python exec="true" source="material-block" result="python" session="df_ex3"
     import pandas as pd
```

### Comparing `narwhals-0.8.9/docs/other/pandas_index.md` & `narwhals-0.9.0/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/narwhals/dataframe.py` & `narwhals-0.9.0/narwhals/expression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,2263 +1,2584 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Literal
-from typing import Sequence
 
-from narwhals._pandas_like.dataframe import PandasDataFrame
 from narwhals.dependencies import get_polars
-from narwhals.dtypes import to_narwhals_dtype
-from narwhals.translate import get_cudf
-from narwhals.translate import get_modin
-from narwhals.translate import get_pandas
-from narwhals.utils import validate_same_library
+from narwhals.dtypes import translate_dtype
+from narwhals.utils import flatten
+from narwhals.utils import parse_version
 
 if TYPE_CHECKING:
-    import numpy as np
-    from typing_extensions import Self
+    from narwhals.typing import IntoExpr
+
 
-    from narwhals.dtypes import DType
-    from narwhals.group_by import GroupBy
-    from narwhals.group_by import LazyGroupBy
+def extract_native(expr: Expr, other: Any) -> Any:
     from narwhals.series import Series
-    from narwhals.typing import IntoExpr
 
+    if isinstance(other, Expr):
+        return other._call(expr)
+    if isinstance(other, Series):
+        return other._series
+    return other
 
-class BaseFrame:
-    _dataframe: Any
-    _is_polars: bool
-
-    def __narwhals_namespace__(self) -> Any:
-        if self._is_polars:
-            import polars as pl
-
-            return pl
-        return self._dataframe.__narwhals_namespace__()
-
-    def _from_dataframe(self, df: Any) -> Self:
-        # construct, preserving properties
-        return self.__class__(  # type: ignore[call-arg]
-            df,
-            is_polars=self._is_polars,
-        )
-
-    def _flatten_and_extract(self, *args: Any, **kwargs: Any) -> Any:
-        from narwhals.utils import flatten
-
-        args = [self._extract_native(v) for v in flatten(args)]  # type: ignore[assignment]
-        kwargs = {k: self._extract_native(v) for k, v in kwargs.items()}
-        return args, kwargs
-
-    def _extract_native(self, arg: Any) -> Any:
-        from narwhals.expression import Expr
-        from narwhals.series import Series
-
-        if isinstance(arg, BaseFrame):
-            return arg._dataframe
-        if isinstance(arg, Series):
-            return arg._series
-        if isinstance(arg, Expr):
-            return arg._call(self.__narwhals_namespace__())
-        if get_polars() is not None and "polars" in str(type(arg)):
-            msg = (
-                f"Expected Narwhals object, got: {type(arg)}.\n\n"
-                "Perhaps you:\n"
-                "- Forgot a `nw.from_native` somewhere?\n"
-                "- Used `pl.col` instead of `nw.col`?"
-            )
-            raise TypeError(msg)
-        return arg
 
-    @property
-    def schema(self) -> dict[str, DType]:
-        return {
-            k: to_narwhals_dtype(v, is_polars=self._is_polars)
-            for k, v in self._dataframe.schema.items()
-        }
-
-    def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
-        return function(self, *args, **kwargs)
-
-    def drop_nulls(self) -> Self:
-        return self._from_dataframe(
-            self._dataframe.drop_nulls(),
+class Expr:
+    def __init__(self, call: Callable[[Any], Any]) -> None:
+        # callable from namespace to expr
+        self._call = call
+
+    # --- convert ---
+    def alias(self, name: str) -> Expr:
+        """
+        Rename the expression.
+
+        Arguments:
+            name: The new name.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 2], 'b': [4, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 2], 'b': [4, 5]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select((nw.col('b')+10).alias('c'))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                c
+            0  14
+            1  15
+            >>> func(df_pl)
+            shape: (2, 1)
+            ┌─────┐
+            │ c   │
+            │ --- │
+            │ i64 │
+            ╞═════╡
+            │ 14  │
+            │ 15  │
+            └─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).alias(name))
+
+    def cast(
+        self,
+        dtype: Any,
+    ) -> Expr:
+        """
+        Redefine an object's data type.
+
+        Arguments:
+            dtype: Data type that the object will be cast into.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> from datetime import date
+            >>> df_pd = pd.DataFrame({"foo": [1, 2, 3],"bar": [6.0, 7.0, 8.0]})
+            >>> df_pl = pl.DataFrame({"foo": [1, 2, 3],"bar": [6.0, 7.0, 8.0]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('foo').cast(nw.Float32), nw.col('bar').cast(nw.UInt8))
+            ...     native_df = nw.to_native(df)
+            ...     return native_df
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               foo  bar
+            0  1.0    6
+            1  2.0    7
+            2  3.0    8
+            >>> func(df_pl)
+            shape: (3, 2)
+            ┌─────┬─────┐
+            │ foo ┆ bar │
+            │ --- ┆ --- │
+            │ f32 ┆ u8  │
+            ╞═════╪═════╡
+            │ 1.0 ┆ 6   │
+            │ 2.0 ┆ 7   │
+            │ 3.0 ┆ 8   │
+            └─────┴─────┘
+        """
+
+        return self.__class__(
+            lambda plx: self._call(plx).cast(translate_dtype(plx, dtype)),
         )
 
-    @property
-    def columns(self) -> list[str]:
-        return self._dataframe.columns  # type: ignore[no-any-return]
+    # --- binary ---
+    def __eq__(self, other: object) -> Expr:  # type: ignore[override]
+        return self.__class__(
+            lambda plx: self._call(plx).__eq__(extract_native(plx, other))
+        )
 
-    def lazy(self) -> LazyFrame:
-        return LazyFrame(
-            self._dataframe.lazy(),
+    def __ne__(self, other: object) -> Expr:  # type: ignore[override]
+        return self.__class__(
+            lambda plx: self._call(plx).__ne__(extract_native(plx, other))
         )
 
-    def with_columns(
-        self, *exprs: IntoExpr | Iterable[IntoExpr], **named_exprs: IntoExpr
-    ) -> Self:
-        exprs, named_exprs = self._flatten_and_extract(*exprs, **named_exprs)
-        return self._from_dataframe(
-            self._dataframe.with_columns(*exprs, **named_exprs),
+    def __and__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__and__(extract_native(plx, other))
         )
 
-    def select(
-        self,
-        *exprs: IntoExpr | Iterable[IntoExpr],
-        **named_exprs: IntoExpr,
-    ) -> Self:
-        exprs, named_exprs = self._flatten_and_extract(*exprs, **named_exprs)
-        return self._from_dataframe(
-            self._dataframe.select(*exprs, **named_exprs),
+    def __rand__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rand__(extract_native(plx, other))
         )
 
-    def rename(self, mapping: dict[str, str]) -> Self:
-        return self._from_dataframe(self._dataframe.rename(mapping))
+    def __or__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__or__(extract_native(plx, other))
+        )
 
-    def head(self, n: int) -> Self:
-        return self._from_dataframe(self._dataframe.head(n))
+    def __ror__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__ror__(extract_native(plx, other))
+        )
 
-    def drop(self, *columns: str | Iterable[str]) -> Self:
-        return self._from_dataframe(self._dataframe.drop(*columns))
+    def __add__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__add__(extract_native(plx, other))
+        )
 
-    def unique(self, subset: str | list[str]) -> Self:
-        return self._from_dataframe(self._dataframe.unique(subset=subset))
+    def __radd__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__radd__(extract_native(plx, other))
+        )
 
-    def filter(self, *predicates: IntoExpr | Iterable[IntoExpr]) -> Self:
-        predicates, _ = self._flatten_and_extract(*predicates)
-        return self._from_dataframe(
-            self._dataframe.filter(*predicates),
+    def __sub__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__sub__(extract_native(plx, other))
         )
 
-    def sort(
-        self,
-        by: str | Iterable[str],
-        *more_by: str,
-        descending: bool | Sequence[bool] = False,
-    ) -> Self:
-        return self._from_dataframe(
-            self._dataframe.sort(by, *more_by, descending=descending)
+    def __rsub__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rsub__(extract_native(plx, other))
         )
 
-    def join(
-        self,
-        other: Self,
-        *,
-        how: Literal["inner"] = "inner",
-        left_on: str | list[str],
-        right_on: str | list[str],
-    ) -> Self:
-        if how != "inner":
-            raise NotImplementedError("Only inner joins are supported for now")
-        validate_same_library([self, other])
-        return self._from_dataframe(
-            self._dataframe.join(
-                self._extract_native(other),
-                how=how,
-                left_on=left_on,
-                right_on=right_on,
-            )
+    def __truediv__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__truediv__(extract_native(plx, other))
         )
 
+    def __rtruediv__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rtruediv__(extract_native(plx, other))
+        )
 
-class DataFrame(BaseFrame):
-    r"""
-    Two-dimensional data structure representing data as a table with rows and columns.
+    def __mul__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__mul__(extract_native(plx, other))
+        )
 
-    Arguments:
-        df: A pandas-like dataframe (Pandas, cuDF or Modin), a Polars dataframe,
-             a narwhals DataFrame or a narwhals LazyFrame.
+    def __rmul__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rmul__(extract_native(plx, other))
+        )
 
-        is_polars: if set to `True`, assume the dataframe to be of Polars type.
+    def __le__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__le__(extract_native(plx, other))
+        )
 
-    Examples:
-        Constructing a DataFrame from a dictionary:
+    def __lt__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__lt__(extract_native(plx, other))
+        )
 
-        >>> import polars as pl
-        >>> import narwhals as nw
-        >>> data = {"a": [1, 2], "b": [3, 4]}
-        >>> df_pl = pl.DataFrame(data)
-        >>> df = nw.DataFrame(df_pl)
-        >>> df
-        ┌───────────────────────────────────────────────┐
-        | Narwhals DataFrame                            |
-        | Use `narwhals.to_native` to see native output |
-        └───────────────────────────────────────────────┘
-        >>> nw.to_native(df)
-        shape: (2, 2)
-        ┌─────┬─────┐
-        │ a   ┆ b   │
-        │ --- ┆ --- │
-        │ i64 ┆ i64 │
-        ╞═════╪═════╡
-        │ 1   ┆ 3   │
-        │ 2   ┆ 4   │
-        └─────┴─────┘
-    """
+    def __gt__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__gt__(extract_native(plx, other))
+        )
 
-    def __init__(
-        self,
-        df: Any,
-        *,
-        is_polars: bool = False,
-    ) -> None:
-        self._is_polars = is_polars
-        if hasattr(df, "__narwhals_dataframe__"):
-            self._dataframe: Any = df.__narwhals_dataframe__()
-        elif is_polars or (
-            (pl := get_polars()) is not None and isinstance(df, pl.DataFrame)
-        ):
-            self._dataframe = df
-            self._is_polars = True
-        elif (pl := get_polars()) is not None and isinstance(df, pl.LazyFrame):
-            raise TypeError(
-                "Can't instantiate DataFrame from Polars LazyFrame. Call `collect()` first, or use `narwhals.LazyFrame` if you don't specifically require eager execution."
-            )
-        elif (pd := get_pandas()) is not None and isinstance(df, pd.DataFrame):
-            self._dataframe = PandasDataFrame(df, implementation="pandas")
-        elif (mpd := get_modin()) is not None and isinstance(
-            df, mpd.DataFrame
-        ):  # pragma: no cover
-            self._dataframe = PandasDataFrame(df, implementation="modin")
-        elif (cudf := get_cudf()) is not None and isinstance(
-            df, cudf.DataFrame
-        ):  # pragma: no cover
-            self._dataframe = PandasDataFrame(df, implementation="cudf")
-        else:
-            msg = f"Expected pandas-like dataframe, Polars dataframe, or Polars lazyframe, got: {type(df)}"
-            raise TypeError(msg)
+    def __ge__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__ge__(extract_native(plx, other))
+        )
 
-    def __array__(self, *args: Any, **kwargs: Any) -> np.ndarray:
-        return self._dataframe.to_numpy(*args, **kwargs)
+    def __pow__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__pow__(extract_native(plx, other))
+        )
 
-    def __repr__(self) -> str:  # pragma: no cover
-        header = " Narwhals DataFrame                            "
-        length = len(header)
-        return (
-            "┌"
-            + "─" * length
-            + "┐\n"
-            + f"|{header}|\n"
-            + "| Use `narwhals.to_native` to see native output |\n"
-            + "└"
-            + "─" * length
-            + "┘"
+    def __rpow__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rpow__(extract_native(plx, other))
         )
 
-    def to_pandas(self) -> Any:
-        r"""
-        Convert this DataFrame to a pandas DataFrame.
+    def __floordiv__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__floordiv__(extract_native(plx, other))
+        )
 
-        Returns:
-            A pandas DataFrame.
+    def __rfloordiv__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rfloordiv__(extract_native(plx, other))
+        )
 
-        Notes:
-            This operation requires that `pandas` is installed.
+    def __mod__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__mod__(extract_native(plx, other))
+        )
+
+    def __rmod__(self, other: Any) -> Expr:
+        return self.__class__(
+            lambda plx: self._call(plx).__rmod__(extract_native(plx, other))
+        )
+
+    # --- unary ---
+    def __invert__(self) -> Expr:
+        return self.__class__(lambda plx: self._call(plx).__invert__())
+
+    def any(self) -> Expr:
+        """
+        Return whether any of the values in the column are `True`
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> df.to_pandas()
-               foo  bar ham
-            0    1  6.0   a
-            1    2  7.0   b
-            2    3  8.0   c
+            >>> df_pd = pd.DataFrame({'a': [True, False], 'b': [True, True]})
+            >>> df_pl = pl.DataFrame({'a': [True, False], 'b': [True, True]})
 
-            Null values in numeric columns are converted to `NaN`.
+            We define a dataframe-agnostic function:
 
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, None],
-            ...         "bar": [6.0, None, 8.0],
-            ...         "ham": [None, "b", "c"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> df.to_pandas()
-               foo  bar   ham
-            0  1.0  6.0  None
-            1  2.0  NaN     b
-            2  NaN  8.0     c
-        """
-        return self._dataframe.to_pandas()
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a', 'b').any())
+            ...     return nw.to_native(df)
 
-    def to_numpy(self) -> Any:
-        r"""
-        Convert this DataFrame to a NumPy ndarray.
+            We can then pass either pandas or Polars to `func`:
 
-        Returns:
-            A NumPy ndarray.
+            >>> func(df_pd)
+                  a     b
+            0  True  True
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌──────┬──────┐
+            │ a    ┆ b    │
+            │ ---  ┆ ---  │
+            │ bool ┆ bool │
+            ╞══════╪══════╡
+            │ true ┆ true │
+            └──────┴──────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).any())
+
+    def all(self) -> Expr:
+        """
+        Return whether all values in the column are `True`.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.5, 7.0, 8.5],
-            ...         "ham": ["a", "b", "c"],
-            ...     },
-            ...     schema_overrides={"foo": pl.UInt8, "bar": pl.Float32},
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-
-            Export to a standard 2D numpy array.
-
-            >>> df.to_numpy()
-            array([[1, 6.5, 'a'],
-                   [2, 7.0, 'b'],
-                   [3, 8.5, 'c']], dtype=object)
+            >>> df_pd = pd.DataFrame({'a': [True, False], 'b': [True, True]})
+            >>> df_pl = pl.DataFrame({'a': [True, False], 'b': [True, True]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a', 'b').all())
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                   a     b
+            0  False  True
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌───────┬──────┐
+            │ a     ┆ b    │
+            │ ---   ┆ ---  │
+            │ bool  ┆ bool │
+            ╞═══════╪══════╡
+            │ false ┆ true │
+            └───────┴──────┘
         """
-        return self._dataframe.to_numpy()
+        return self.__class__(lambda plx: self._call(plx).all())
 
-    @property
-    def shape(self) -> tuple[int, int]:
-        r"""
-        Get the shape of the DataFrame.
+    def mean(self) -> Expr:
+        """
+        Get mean value.
 
         Examples:
             >>> import polars as pl
+            >>> import pandas as pd
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame({"foo": [1, 2, 3, 4, 5]})
-            >>> df = nw.DataFrame(df_pl)
-            >>> df.shape
-            (5, 1)
-        """
-        return self._dataframe.shape  # type: ignore[no-any-return]
+            >>> df_pd = pd.DataFrame({'a': [-1, 0, 1], 'b': [2, 4, 6]})
+            >>> df_pl = pl.DataFrame({'a': [-1, 0, 1], 'b': [2, 4, 6]})
 
-    def __getitem__(self, col_name: str) -> Series:
-        from narwhals.series import Series
+            Let's define a dataframe-agnostic function:
 
-        return Series(self._dataframe[col_name])
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.col('a', 'b').mean())
+            ...    return nw.to_native(df)
 
-    def to_dict(self, *, as_series: bool = True) -> dict[str, Any]:
-        r"""
-        Convert DataFrame to a dictionary mapping column name to values.
+            We can then pass either pandas or Polars to `func`:
 
-        Arguments:
-            as_series: If set to true ``True`` values are Series, otherwise
-                        values are Any.
+            >>> func(df_pd)
+                 a    b
+            0  0.0  4.0
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ f64 ┆ f64 │
+            ╞═════╪═════╡
+            │ 0.0 ┆ 4.0 │
+            └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).mean())
 
-        Examples:
-            >>> import polars as pl
-            >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "A": [1, 2, 3, 4, 5],
-            ...         "fruits": ["banana", "banana", "apple", "apple", "banana"],
-            ...         "B": [5, 4, 3, 2, 1],
-            ...         "cars": ["beetle", "audi", "beetle", "beetle", "beetle"],
-            ...         "optional": [28, 300, None, 2, -30],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(df)
-            shape: (5, 5)
-            ┌─────┬────────┬─────┬────────┬──────────┐
-            │ A   ┆ fruits ┆ B   ┆ cars   ┆ optional │
-            │ --- ┆ ---    ┆ --- ┆ ---    ┆ ---      │
-            │ i64 ┆ str    ┆ i64 ┆ str    ┆ i64      │
-            ╞═════╪════════╪═════╪════════╪══════════╡
-            │ 1   ┆ banana ┆ 5   ┆ beetle ┆ 28       │
-            │ 2   ┆ banana ┆ 4   ┆ audi   ┆ 300      │
-            │ 3   ┆ apple  ┆ 3   ┆ beetle ┆ null     │
-            │ 4   ┆ apple  ┆ 2   ┆ beetle ┆ 2        │
-            │ 5   ┆ banana ┆ 1   ┆ beetle ┆ -30      │
-            └─────┴────────┴─────┴────────┴──────────┘
-            >>> df.to_dict(as_series=False)
-            {'A': [1, 2, 3, 4, 5], 'fruits': ['banana', 'banana', 'apple', 'apple', 'banana'], 'B': [5, 4, 3, 2, 1], 'cars': ['beetle', 'audi', 'beetle', 'beetle', 'beetle'], 'optional': [28, 300, None, 2, -30]}
-            >>> df.to_dict(as_series=True) # doctest: +SKIP
-            {'A': shape: (5,)
-            Series: 'A' [i64]
-            [
-                1
-                2
-                3
-                4
-                5
-            ], 'fruits': shape: (5,)
-            Series: 'fruits' [str]
-            [
-                "banana"
-                "banana"
-                "apple"
-                "apple"
-                "banana"
-            ], 'B': shape: (5,)
-            Series: 'B' [i64]
-            [
-                5
-                4
-                3
-                2
-                1
-            ], 'cars': shape: (5,)
-            Series: 'cars' [str]
-            [
-                "beetle"
-                "audi"
-                "beetle"
-                "beetle"
-                "beetle"
-            ], 'optional': shape: (5,)
-            Series: 'optional' [i64]
-            [
-                28
-                300
-                null
-                2
-                -30
-            ]}
-        """
-        return self._dataframe.to_dict(as_series=as_series)  # type: ignore[no-any-return]
-
-    # inherited
-    def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
-        """
-        Pipe function call.
+    def std(self, *, ddof: int = 1) -> Expr:
+        """
+        Get standard deviation.
+
+        Arguments:
+            ddof: “Delta Degrees of Freedom”: the divisor used in the calculation is N - ddof,
+                     where N represents the number of elements. By default ddof is 1.
 
         Examples:
             >>> import polars as pl
             >>> import pandas as pd
             >>> import narwhals as nw
-            >>> data = {'a': [1,2,3], 'ba': [4,5,6]}
-            >>> df_pd = pd.DataFrame(data)
-            >>> df_pl = pl.DataFrame(data)
+            >>> df_pd = pd.DataFrame({'a': [20, 25, 60], 'b': [1.5, 1, -1.4]})
+            >>> df_pl = pl.DataFrame({'a': [20, 25, 60], 'b': [1.5, 1, -1.4]})
 
             Let's define a dataframe-agnostic function:
 
             >>> def func(df_any):
-            ...     df = nw.from_native(df_any)
-            ...     df = df.pipe(lambda _df: _df.select([x for x in _df.columns if len(x) == 1]))
-            ...     return nw.to_native(df)
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.col('a', 'b').std(ddof=0))
+            ...    return nw.to_native(df)
 
-            We can then pass either pandas or Polars:
+            We can then pass either pandas or Polars to `func`:
 
             >>> func(df_pd)
-               a
-            0  1
-            1  2
-            2  3
+                      a         b
+            0  17.79513  1.265789
             >>> func(df_pl)
-            shape: (3, 1)
-            ┌─────┐
-            │ a   │
-            │ --- │
-            │ i64 │
-            ╞═════╡
-            │ 1   │
-            │ 2   │
-            │ 3   │
-            └─────┘
-        """
-        return super().pipe(function, *args, **kwargs)
+            shape: (1, 2)
+            ┌──────────┬──────────┐
+            │ a        ┆ b        │
+            │ ---      ┆ ---      │
+            │ f64      ┆ f64      │
+            ╞══════════╪══════════╡
+            │ 17.79513 ┆ 1.265789 │
+            └──────────┴──────────┘
 
-    def drop_nulls(self) -> Self:
         """
-        Drop null values.
+        return self.__class__(lambda plx: self._call(plx).std(ddof=ddof))
 
-        Notes:
-            pandas and Polars handle null values differently. Polars distinguishes
-            between NaN and Null, whereas pandas doesn't.
+    def sum(self) -> Expr:
+        """
+        Return the sum value.
 
         Examples:
-            >>> import polars as pl
             >>> import pandas as pd
+            >>> import polars as pl
             >>> import narwhals as nw
-            >>> data = {'a': [1., 2., None], 'ba': [1, None, 2.]}
-            >>> df_pd = pd.DataFrame(data)
-            >>> df_pl = pl.DataFrame(data)
+            >>> df_pd = pd.DataFrame({'a': [5, 10], 'b': [50, 100]})
+            >>> df_pl = pl.DataFrame({'a': [5, 10], 'b': [50, 100]})
 
             Let's define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
-            ...     df = df.drop_nulls()
+            ...     df = df.select(nw.col('a', 'b').sum())
             ...     return nw.to_native(df)
 
-            We can then pass either pandas or Polars:
+            We can then pass either pandas or Polars to `func`:
 
             >>> func(df_pd)
-                 a   ba
-            0  1.0  1.0
+                a    b
+            0  15  150
             >>> func(df_pl)
             shape: (1, 2)
             ┌─────┬─────┐
-            │ a   ┆ ba  │
+            │ a   ┆ b   │
             │ --- ┆ --- │
-            │ f64 ┆ f64 │
+            │ i64 ┆ i64 │
             ╞═════╪═════╡
-            │ 1.0 ┆ 1.0 │
+            │ 15  ┆ 150 │
             └─────┴─────┘
         """
-        return super().drop_nulls()
+        return self.__class__(lambda plx: self._call(plx).sum())
 
-    @property
-    def schema(self) -> dict[str, DType]:
-        r"""
-        Get a dict[column name, DataType].
+    def min(self) -> Expr:
+        """
+        Returns the minimum value(s) from a column(s).
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df.schema  # doctest: +SKIP
-            OrderedDict({'foo': Int64, 'bar': Float64, 'ham': String})
+            >>> df_pd = pd.DataFrame({'a': [1, 2], 'b': [4, 3]})
+            >>> df_pl = pl.DataFrame({'a': [1, 2], 'b': [4, 3]})
+
+            Let's define a dataframe-agnostic function:
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.min('a','b'))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a  b
+            0  1  3
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ i64 ┆ i64 │
+            ╞═════╪═════╡
+            │ 1   ┆ 3   │
+            └─────┴─────┘
         """
-        return super().schema
 
-    @property
-    def columns(self) -> list[str]:
-        r"""
-        Get column names.
+        return self.__class__(lambda plx: self._call(plx).min())
 
-        Examples:
-            Get column names.
+    def max(self) -> Expr:
+        """
+        Returns the maximum value(s) from a column(s).
 
+        Examples:
             >>> import polars as pl
+            >>> import pandas as pd
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df.columns
-            ['foo', 'bar', 'ham']
-        """
-        return super().columns
-
-    def with_columns(
-        self, *exprs: IntoExpr | Iterable[IntoExpr], **named_exprs: IntoExpr
-    ) -> Self:
-        r"""
-        Add columns to this DataFrame.
+            >>> df_pd = pd.DataFrame({'a': [10, 20], 'b': [50, 100]})
+            >>> df_pl = pl.DataFrame({'a': [10, 20], 'b': [50, 100]})
 
-        Added columns will replace existing columns with the same name.
+            Let's define a dataframe-agnostic function:
 
-        Arguments:
-            *exprs: Column(s) to add, specified as positional arguments.
-                     Accepts expression input. Strings are parsed as column names, other
-                     non-expression inputs are parsed as literals.
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.max('a', 'b'))
+            ...    return nw.to_native(df)
 
-            **named_exprs: Additional columns to add, specified as keyword arguments.
-                            The columns will be renamed to the keyword used.
+            We can then pass either pandas or Polars to `func`:
 
-        Returns:
-            DataFrame: A new DataFrame with the columns added.
+            >>> func(df_pd)
+                a    b
+            0  20  100
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ i64 ┆ i64 │
+            ╞═════╪═════╡
+            │ 20  ┆ 100 │
+            └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).max())
 
-        Note:
-            Creating a new DataFrame using this method does not create a new copy of
-            existing data.
+    def n_unique(self) -> Expr:
+        """
+         Returns count of unique values
 
         Examples:
-            Pass an expression to add it as a new column.
-
             >>> import polars as pl
+            >>> import pandas as pd
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "a": [1, 2, 3, 4],
-            ...         "b": [0.5, 4, 10, 13],
-            ...         "c": [True, True, False, True],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> dframe = df.with_columns((nw.col("a") * 2).alias("a*2"))
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (4, 4)
-            ┌─────┬──────┬───────┬─────┐
-            │ a   ┆ b    ┆ c     ┆ a*2 │
-            │ --- ┆ ---  ┆ ---   ┆ --- │
-            │ i64 ┆ f64  ┆ bool  ┆ i64 │
-            ╞═════╪══════╪═══════╪═════╡
-            │ 1   ┆ 0.5  ┆ true  ┆ 2   │
-            │ 2   ┆ 4.0  ┆ true  ┆ 4   │
-            │ 3   ┆ 10.0 ┆ false ┆ 6   │
-            │ 4   ┆ 13.0 ┆ true  ┆ 8   │
-            └─────┴──────┴───────┴─────┘
-        """
-        return super().with_columns(*exprs, **named_exprs)
+            >>> df_pd = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': [1, 1, 3, 3, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 2, 3, 4, 5], 'b': [1, 1, 3, 3, 5]})
 
-    def select(
-        self,
-        *exprs: IntoExpr | Iterable[IntoExpr],
-        **named_exprs: IntoExpr,
-    ) -> Self:
-        r"""
-        Select columns from this DataFrame.
+            Let's define a dataframe-agnostic function:
 
-        Arguments:
-            *exprs: Column(s) to select, specified as positional arguments.
-                     Accepts expression input. Strings are parsed as column names,
-                     other non-expression inputs are parsed as literals.
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.col('a', 'b').n_unique())
+            ...    return nw.to_native(df)
 
-            **named_exprs: Additional columns to select, specified as keyword arguments.
-                            The columns will be renamed to the keyword used.
+            We can then pass either pandas or Polars to `func`:
 
-        Examples:
-            Pass the name of a column to select that column.
+            >>> func(df_pd)
+               a  b
+            0  5  3
+            >>> func(df_pl)
+            shape: (1, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ u32 ┆ u32 │
+            ╞═════╪═════╡
+            │ 5   ┆ 3   │
+            └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).n_unique())
+
+    def unique(self) -> Expr:
+        """
+        Return unique values
 
+        Examples:
             >>> import polars as pl
+            >>> import pandas as pd
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> dframe = df.select("foo")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 1)
-            ┌─────┐
-            │ foo │
-            │ --- │
-            │ i64 │
-            ╞═════╡
-            │ 1   │
-            │ 2   │
-            │ 3   │
-            └─────┘
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
 
-            Multiple columns can be selected by passing a list of column names.
+            Let's define a dataframe-agnostic function:
 
-            >>> dframe = df.select(["foo", "bar"])
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.col('a', 'b').unique())
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a  b
+            0  1  2
+            1  3  4
+            2  5  6
+            >>> func(df_pl)
             shape: (3, 2)
             ┌─────┬─────┐
-            │ foo ┆ bar │
+            │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
-            │ 1   ┆ 6   │
-            │ 2   ┆ 7   │
-            │ 3   ┆ 8   │
+            │ 1   ┆ 2   │
+            │ 3   ┆ 4   │
+            │ 5   ┆ 6   │
             └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).unique())
 
-            Multiple columns can also be selected using positional arguments instead of a
-            list. Expressions are also accepted.
+    def cum_sum(self) -> Expr:
+        """
+        Return cumulative sum.
 
-            >>> dframe = df.select(nw.col("foo"), nw.col("bar") + 1)
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 2)
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5], 'b': [2, 4, 4, 6, 6]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(nw.col('a', 'b').cum_sum())
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                a   b
+            0   1   2
+            1   2   6
+            2   5  10
+            3  10  16
+            4  15  22
+            >>> func(df_pl)
+            shape: (5, 2)
             ┌─────┬─────┐
-            │ foo ┆ bar │
+            │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
-            │ 1   ┆ 7   │
-            │ 2   ┆ 8   │
-            │ 3   ┆ 9   │
+            │ 1   ┆ 2   │
+            │ 2   ┆ 6   │
+            │ 5   ┆ 10  │
+            │ 10  ┆ 16  │
+            │ 15  ┆ 22  │
             └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).cum_sum())
 
-            Use keyword arguments to easily name your expression inputs.
+    def diff(self) -> Expr:
+        """
+        Returns the difference between each element and the previous one.
 
-            >>> dframe = df.select(threshold=nw.col('foo')*2)
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 1)
-            ┌───────────┐
-            │ threshold │
-            │ ---       │
-            │ i64       │
-            ╞═══════════╡
-            │ 2         │
-            │ 4         │
-            │ 6         │
-            └───────────┘
+        Notes:
+            pandas may change the dtype here, for example when introducing missing
+            values in an integer column. To ensure, that the dtype doesn't change,
+            you may want to use `fill_null` and `cast`. For example, to calculate
+            the diff and fill missing values with `0` in a Int64 column, you could
+            do:
+
+            ```python
+            nw.col('a').diff().fill_null(0).cast(nw.Int64)
+            ```
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(a_diff=nw.col('a').diff())
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a_diff
+            0     NaN
+            1     0.0
+            2     2.0
+            3     2.0
+            4     0.0
+            >>> func(df_pl)
+            shape: (5, 1)
+            ┌────────┐
+            │ a_diff │
+            │ ---    │
+            │ i64    │
+            ╞════════╡
+            │ null   │
+            │ 0      │
+            │ 2      │
+            │ 2      │
+            │ 0      │
+            └────────┘
         """
-        return super().select(*exprs, **named_exprs)
+        return self.__class__(lambda plx: self._call(plx).diff())
 
-    def rename(self, mapping: dict[str, str]) -> Self:
-        r"""
-        Rename column names.
+    def shift(self, n: int) -> Expr:
+        """
+        Shift values by `n` positions.
+
+        Notes:
+            pandas may change the dtype here, for example when introducing missing
+            values in an integer column. To ensure, that the dtype doesn't change,
+            you may want to use `fill_null` and `cast`. For example, to shift
+            and fill missing values with `0` in a Int64 column, you could
+            do:
+
+            ```python
+            nw.col('a').shift(1).fill_null(0).cast(nw.Int64)
+            ```
+
+        Examples:
+            >>> import polars as pl
+            >>> import pandas as pd
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 1, 3, 5, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 1, 3, 5, 5]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.select(a_shift=nw.col('a').shift(n=1))
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a_shift
+            0      NaN
+            1      1.0
+            2      1.0
+            3      3.0
+            4      5.0
+            >>> func(df_pl)
+            shape: (5, 1)
+            ┌─────────┐
+            │ a_shift │
+            │ ---     │
+            │ i64     │
+            ╞═════════╡
+            │ null    │
+            │ 1       │
+            │ 1       │
+            │ 3       │
+            │ 5       │
+            └─────────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).shift(n))
+
+    def sort(self, *, descending: bool = False) -> Expr:
+        """
+        Sort this column. Place null values first.
 
         Arguments:
-            mapping: Key value pairs that map from old name to new name.
+            descending: Sort in descending order.
 
         Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+
+            >>> df_pd = pd.DataFrame({"a": [5, None, 1, 2]})
+            >>> df_pl = pl.DataFrame({"a": [5, None, 1, 2]})
+
+            Let's define dataframe-agnostic functions:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a').sort())
+            ...     return nw.to_native(df)
+
+            >>> def func_descend(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a').sort(descending=True))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a
+            1  NaN
+            2  1.0
+            3  2.0
+            0  5.0
+            >>> func(df_pl)
+            shape: (4, 1)
+            ┌──────┐
+            │ a    │
+            │ ---  │
+            │ i64  │
+            ╞══════╡
+            │ null │
+            │ 1    │
+            │ 2    │
+            │ 5    │
+            └──────┘
+
+            >>> func_descend(df_pd)
+                 a
+            1  NaN
+            0  5.0
+            3  2.0
+            2  1.0
+            >>> func_descend(df_pl)
+            shape: (4, 1)
+            ┌──────┐
+            │ a    │
+            │ ---  │
+            │ i64  │
+            ╞══════╡
+            │ null │
+            │ 5    │
+            │ 2    │
+            │ 1    │
+            └──────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).sort(descending=descending))
+
+    # --- transform ---
+    def is_between(
+        self, lower_bound: Any, upper_bound: Any, closed: str = "both"
+    ) -> Expr:
+        """
+        Check if this expression is between the given lower and upper bounds.
+
+        Arguments:
+            lower_bound: Lower bound value.
+
+            upper_bound: Upper bound value.
+
+            closed: Define which sides of the interval are closed (inclusive).
+
+        Examples:
+            >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {"foo": [1, 2, 3], "bar": [6, 7, 8], "ham": ["a", "b", "c"]}
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> dframe = df.rename({"foo": "apple"})
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 3)
-            ┌───────┬─────┬─────┐
-            │ apple ┆ bar ┆ ham │
-            │ ---   ┆ --- ┆ --- │
-            │ i64   ┆ i64 ┆ str │
-            ╞═══════╪═════╪═════╡
-            │ 1     ┆ 6   ┆ a   │
-            │ 2     ┆ 7   ┆ b   │
-            │ 3     ┆ 8   ┆ c   │
-            └───────┴─────┴─────┘
+            >>> df_pd = pd.DataFrame({'a': [1, 2, 3, 4, 5]})
+            >>> df_pl = pl.DataFrame({'a': [1, 2, 3, 4, 5]})
+
+            Let's define a dataframe-agnostic function:
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a').is_between(2,4,'right'))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                   a
+            0  False
+            1  False
+            2   True
+            3   True
+            4  False
+            >>> func(df_pl)
+            shape: (5, 1)
+            ┌───────┐
+            │ a     │
+            │ ---   │
+            │ bool  │
+            ╞═══════╡
+            │ false │
+            │ false │
+            │ true  │
+            │ true  │
+            │ false │
+            └───────┘
         """
-        return super().rename(mapping)
+        return self.__class__(
+            lambda plx: self._call(plx).is_between(lower_bound, upper_bound, closed)
+        )
 
-    def head(self, n: int) -> Self:
-        r"""
-        Get the first `n` rows.
+    def is_in(self, other: Any) -> Expr:
+        """
+        Check if elements of this expression are present in the other iterable.
 
         Arguments:
-            n: Number of rows to return. If a negative value is passed, return all rows
-                except the last `abs(n)`.
+            other: iterable
 
         Examples:
-            Get column names.
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [1, 2, 9, 10]})
+            >>> df_pl = pl.DataFrame({'a': [1, 2, 9, 10]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...    df = nw.from_native(df_any)
+            ...    df = df.with_columns(b = nw.col('a').is_in([1, 2]))
+            ...    return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                a      b
+            0   1   True
+            1   2   True
+            2   9  False
+            3  10  False
 
+            >>> func(df_pl)
+            shape: (4, 2)
+            ┌─────┬───────┐
+            │ a   ┆ b     │
+            │ --- ┆ ---   │
+            │ i64 ┆ bool  │
+            ╞═════╪═══════╡
+            │ 1   ┆ true  │
+            │ 2   ┆ true  │
+            │ 9   ┆ false │
+            │ 10  ┆ false │
+            └─────┴───────┘
+        """
+        if isinstance(other, Iterable) and not isinstance(other, (str, bytes)):
+            return self.__class__(lambda plx: self._call(plx).is_in(other))
+        else:
+            raise NotImplementedError(
+                "Narwhals `is_in` doesn't accept expressions as an argument, as opposed to Polars. You should provide an iterable instead."
+            )
+
+    def filter(self, *predicates: Any) -> Expr:
+        """
+        Filters elements based on a condition, returning a new expression.
+
+        Examples:
             >>> import polars as pl
+            >>> import pandas as pd
             >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': [2, 3, 4, 5, 6, 7], 'b': [10, 11, 12, 13, 14, 15]})
+            >>> df_pl = pl.DataFrame({'a': [2, 3, 4, 5, 6, 7], 'b': [10, 11, 12, 13, 14, 15]})
+
+            Let's define a dataframe-agnostic function:
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(
+            ...             nw.col("a").filter(nw.col("a") > 4),
+            ...             nw.col("b").filter(nw.col("b") < 13)
+            ...             )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a   b
+            3  5  10
+            4  6  11
+            5  7  12
+            >>> func(df_pl)
+            shape: (3, 2)
+            ┌─────┬─────┐
+            │ a   ┆ b   │
+            │ --- ┆ --- │
+            │ i64 ┆ i64 │
+            ╞═════╪═════╡
+            │ 5   ┆ 10  │
+            │ 6   ┆ 11  │
+            │ 7   ┆ 12  │
+            └─────┴─────┘
+        """
+        return self.__class__(
+            lambda plx: self._call(plx).filter(
+                *[extract_native(plx, pred) for pred in flatten(predicates)]
+            )
+        )
+
+    def is_null(self) -> Expr:
+        """
+        Returns a boolean Series indicating which values are null.
+
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame(
+            ...         {
+            ...             'a': [2, 4, None, 3, 5],
+            ...             'b': [2.0, 4.0, float("nan"), 3.0, 5.0]
+            ...         }
+            ... )
             >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3, 4, 5],
-            ...         "bar": [6, 7, 8, 9, 10],
-            ...         "ham": ["a", "b", "c", "d", "e"],
-            ...     }
+            ...         {
+            ...             'a': [2, 4, None, 3, 5],
+            ...             'b': [2.0, 4.0, float("nan"), 3.0, 5.0]
+            ...         }
             ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> dframe = df.head(3)
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            │ 2   ┆ 7   ┆ b   │
-            │ 3   ┆ 8   ┆ c   │
-            └─────┴─────┴─────┘
-
-            Pass a negative value to get all rows `except` the last `abs(n)`.
-
-            >>> dframe = df.head(-3)
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (2, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            │ 2   ┆ 7   ┆ b   │
-            └─────┴─────┴─────┘
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         a_is_null = nw.col('a').is_null(),
+            ...         b_is_null = nw.col('b').is_null()
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a    b  a_is_null  b_is_null
+            0  2.0  2.0      False      False
+            1  4.0  4.0      False      False
+            2  NaN  NaN       True       True
+            3  3.0  3.0      False      False
+            4  5.0  5.0      False      False
+
+            >>> func(df_pl)  # nan != null for polars
+            shape: (5, 4)
+            ┌──────┬─────┬───────────┬───────────┐
+            │ a    ┆ b   ┆ a_is_null ┆ b_is_null │
+            │ ---  ┆ --- ┆ ---       ┆ ---       │
+            │ i64  ┆ f64 ┆ bool      ┆ bool      │
+            ╞══════╪═════╪═══════════╪═══════════╡
+            │ 2    ┆ 2.0 ┆ false     ┆ false     │
+            │ 4    ┆ 4.0 ┆ false     ┆ false     │
+            │ null ┆ NaN ┆ true      ┆ false     │
+            │ 3    ┆ 3.0 ┆ false     ┆ false     │
+            │ 5    ┆ 5.0 ┆ false     ┆ false     │
+            └──────┴─────┴───────────┴───────────┘
         """
-        return super().head(n)
+        return self.__class__(lambda plx: self._call(plx).is_null())
 
-    def drop(self, *columns: str | Iterable[str]) -> Self:
-        r"""
-        Remove columns from the dataframe.
+    def fill_null(self, value: Any) -> Expr:
+        """
+        Fill null values with given value.
 
-        Arguments:
-            *columns: Names of the columns that should be removed from the dataframe.
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
 
         Examples:
-            Drop a single column by passing the name of that column.
-
+            >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame(
+            ...         {
+            ...             'a': [2, 4, None, 3, 5],
+            ...             'b': [2.0, 4.0, float("nan"), 3.0, 5.0]
+            ...         }
+            ... )
             >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
+            ...         {
+            ...             'a': [2, 4, None, 3, 5],
+            ...             'b': [2.0, 4.0, float("nan"), 3.0, 5.0]
+            ...         }
             ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> dframe = df.drop("ham")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 2)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(nw.col('a', 'b').fill_null(0))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a    b
+            0  2.0  2.0
+            1  4.0  4.0
+            2  0.0  0.0
+            3  3.0  3.0
+            4  5.0  5.0
+
+            >>> func(df_pl)  # nan != null for polars
+            shape: (5, 2)
             ┌─────┬─────┐
-            │ foo ┆ bar │
+            │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ f64 │
             ╞═════╪═════╡
-            │ 1   ┆ 6.0 │
-            │ 2   ┆ 7.0 │
-            │ 3   ┆ 8.0 │
+            │ 2   ┆ 2.0 │
+            │ 4   ┆ 4.0 │
+            │ 0   ┆ NaN │
+            │ 3   ┆ 3.0 │
+            │ 5   ┆ 5.0 │
             └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).fill_null(value))
 
-            Drop multiple columns by passing a list of column names.
+    # --- partial reduction ---
+    def drop_nulls(self) -> Expr:
+        """
+        Remove missing values.
 
-            >>> dframe = df.drop(["bar", "ham"])
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 1)
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
+
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+
+            >>> df_pd = pd.DataFrame({"a": [2.0, 4.0, float("nan"), 3.0, None, 5.0]})
+            >>> df_pl = pl.DataFrame({"a": [2.0, 4.0, float("nan"), 3.0, None, 5.0]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col("a").drop_nulls())
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a
+            0  2.0
+            1  4.0
+            3  3.0
+            5  5.0
+            >>> func(df_pl)  # nan != null for polars
+            shape: (5, 1)
             ┌─────┐
-            │ foo │
+            │ a   │
             │ --- │
-            │ i64 │
+            │ f64 │
             ╞═════╡
-            │ 1   │
-            │ 2   │
-            │ 3   │
+            │ 2.0 │
+            │ 4.0 │
+            │ NaN │
+            │ 3.0 │
+            │ 5.0 │
             └─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).drop_nulls())
+
+    def sample(
+        self,
+        n: int | None = None,
+        fraction: float | None = None,
+        *,
+        with_replacement: bool = False,
+    ) -> Expr:
+        """
+        Sample randomly from this expression.
+
+        Arguments:
+            n: Number of items to return. Cannot be used with fraction.
+
+            fraction: Fraction of items to return. Cannot be used with n.
+
+            with_replacement: Allow values to be sampled more than once.
+
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+
+            >>> df_pd = pd.DataFrame({"a": [1, 2, 3]})
+            >>> df_pl = pl.DataFrame({"a": [1, 2, 3]})
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a').sample(fraction=1.0, with_replacement=True))
+            ...     return nw.to_native(df)
 
-            Use positional arguments to drop multiple columns.
+            We can then pass either pandas or Polars to `func`:
 
-            >>> dframe = df.drop("foo", "ham")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
+            >>> func(df_pd)  # doctest:+SKIP
+               a
+            2  3
+            0  1
+            2  3
+            >>> func(df_pl)  # doctest:+SKIP
             shape: (3, 1)
             ┌─────┐
-            │ bar │
+            │ a   │
             │ --- │
             │ f64 │
             ╞═════╡
-            │ 6.0 │
-            │ 7.0 │
-            │ 8.0 │
+            │ 2   │
+            │ 3   │
+            │ 3   │
             └─────┘
         """
-        return super().drop(*columns)
+        return self.__class__(
+            lambda plx: self._call(plx).sample(
+                n, fraction=fraction, with_replacement=with_replacement
+            )
+        )
 
-    def unique(self, subset: str | list[str]) -> Self:
-        r"""
-        Drop duplicate rows from this dataframe.
+    def over(self, *keys: str | Iterable[str]) -> Expr:
+        """
+        Compute expressions over the given groups.
 
         Arguments:
-            subset: Column name(s) to consider when identifying duplicate rows.
-
-        Returns:
-            DataFrame: DataFrame with unique rows.
+            keys: Names of columns to compute window expression over.
+                  Must be names of columns, as opposed to expressions -
+                  so, this is a bit less flexible than Polars' `Expr.over`.
 
         Examples:
-            >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3, 1],
-            ...         "bar": ["a", "a", "a", "a"],
-            ...         "ham": ["b", "b", "b", "b"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> dframe = df.unique(["bar", "ham"])
-            >>> nw.to_native(dframe)
-            shape: (1, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ str ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ a   ┆ b   │
-            └─────┴─────┴─────┘
-            >>> dframe = df.unique("foo").sort("foo")
-            >>> nw.to_native(dframe)
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {'a': [1, 2, 3], 'b': [1, 1, 2]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         a_min_per_group = nw.col('a').min().over('b')
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars:
+
+            >>> func(df_pd)
+               a  b  a_min_per_group
+            0  1  1                1
+            1  2  1                1
+            2  3  2                3
+            >>> func(df_pl)
             shape: (3, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ str ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ a   ┆ b   │
-            │ 2   ┆ a   ┆ b   │
-            │ 3   ┆ a   ┆ b   │
-            └─────┴─────┴─────┘
+            ┌─────┬─────┬─────────────────┐
+            │ a   ┆ b   ┆ a_min_per_group │
+            │ --- ┆ --- ┆ ---             │
+            │ i64 ┆ i64 ┆ i64             │
+            ╞═════╪═════╪═════════════════╡
+            │ 1   ┆ 1   ┆ 1               │
+            │ 2   ┆ 1   ┆ 1               │
+            │ 3   ┆ 2   ┆ 3               │
+            └─────┴─────┴─────────────────┘
         """
-        return super().unique(subset)
+        return self.__class__(lambda plx: self._call(plx).over(flatten(keys)))
 
-    def filter(self, *predicates: IntoExpr | Iterable[IntoExpr]) -> Self:
+    def is_duplicated(self) -> Expr:
         r"""
-        Filter the rows in the DataFrame based on one or more predicate expressions.
+        Return a boolean mask indicating duplicated values.
+
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {"a": [1, 2, 3, 1], "b": ["a", "a", "b", "c"]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-        The original order of the remaining rows is preserved.
+            Let's define a dataframe-agnostic function:
 
-        Arguments:
-            predicates: Expression(s) that evaluates to a boolean Series.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     duplicated = df.select(nw.all().is_duplicated())
+            ...     return nw.to_native(duplicated)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)  # doctest: +NORMALIZE_WHITESPACE
+                   a      b
+            0   True   True
+            1  False   True
+            2  False  False
+            3   True  False
+            >>> func(df_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (4, 2)
+            ┌───────┬───────┐
+            │ a     ┆ b     │
+            │ ---   ┆ ---   │
+            │ bool  ┆ bool  │
+            ╞═══════╪═══════╡
+            │ true  ┆ true  │
+            │ false ┆ true  │
+            │ false ┆ false │
+            │ true  ┆ false │
+            └───────┴───────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).is_duplicated())
+
+    def is_unique(self) -> Expr:
+        r"""
+        Return a boolean mask indicating unique values.
 
         Examples:
-            >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-
-            Filter on one condition:
-
-            >>> dframe = df.filter(nw.col("foo") > 1)
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (2, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 2   ┆ 7   ┆ b   │
-            │ 3   ┆ 8   ┆ c   │
-            └─────┴─────┴─────┘
-
-            Filter on multiple conditions, combined with and/or operators:
-
-            >>> dframe = df.filter((nw.col("foo") < 3) & (nw.col("ham") == "a"))
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (1, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            └─────┴─────┴─────┘
-
-            >>> dframe = df.filter((nw.col("foo") == 1) | (nw.col("ham") == "c"))
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (2, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            │ 3   ┆ 8   ┆ c   │
-            └─────┴─────┴─────┘
-
-            Provide multiple filters using `*args` syntax:
-
-            >>> dframe = df.filter(
-            ...     nw.col("foo") <= 2,
-            ...     ~nw.col("ham").is_in(["b", "c"]),
-            ... )
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (1, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            └─────┴─────┴─────┘
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {"a": [1, 2, 3, 1], "b": ["a", "a", "b", "c"]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     unique = df.select(nw.all().is_unique())
+            ...     return nw.to_native(unique)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)  # doctest: +NORMALIZE_WHITESPACE
+                   a      b
+            0  False  False
+            1   True  False
+            2   True   True
+            3  False   True
+            >>> func(df_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (4, 2)
+            ┌───────┬───────┐
+            │ a     ┆ b     │
+            │ ---   ┆ ---   │
+            │ bool  ┆ bool  │
+            ╞═══════╪═══════╡
+            │ false ┆ false │
+            │ true  ┆ false │
+            │ true  ┆ true  │
+            │ false ┆ true  │
+            └───────┴───────┘
         """
-        return super().filter(*predicates)
 
-    def group_by(self, *keys: str | Iterable[str]) -> GroupBy:
-        r"""
-        Start a group by operation.
+        return self.__class__(lambda plx: self._call(plx).is_unique())
 
-        Arguments:
-            *keys: Column(s) to group by. Accepts multiple columns names as a list.
+    def null_count(self) -> Expr:
+        r"""
+        Count null values.
 
-        Returns:
-            GroupBy: Object which can be used to perform aggregations.
+        Notes:
+            pandas and Polars handle null values differently. Polars distinguishes
+            between NaN and Null, whereas pandas doesn't.
 
         Examples:
-            Group by one column and call `agg` to compute the grouped sum of another
-             column.
-
-            >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "a": ["a", "b", "a", "b", "c"],
-            ...         "b": [1, 2, 1, 3, 3],
-            ...         "c": [5, 4, 3, 2, 1],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> dframe = df.group_by("a").agg(nw.col("b").sum()).sort("a")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 2)
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {"a": [1, 2, None, 1], "b": ["a", None, "b", None]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     nulls = df.select(nw.all().null_count())
+            ...     return nw.to_native(nulls)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+               a  b
+            0  1  2
+            >>> func(df_pl)
+            shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
-            │ str ┆ i64 │
+            │ u32 ┆ u32 │
             ╞═════╪═════╡
-            │ a   ┆ 2   │
-            │ b   ┆ 5   │
-            │ c   ┆ 3   │
+            │ 1   ┆ 2   │
             └─────┴─────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).null_count())
 
-            Group by multiple columns by passing a list of column names.
+    def is_first_distinct(self) -> Expr:
+        r"""
+        Return a boolean mask indicating the first occurrence of each distinct value.
 
-            >>> dframe = df.group_by(["a", "b"]).agg(nw.max("c")).sort("a", "b")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe) # doctest: +SKIP
-            shape: (4, 3)
-            ┌─────┬─────┬─────┐
-            │ a   ┆ b   ┆ c   │
-            │ --- ┆ --- ┆ --- │
-            │ str ┆ i64 ┆ i64 │
-            ╞═════╪═════╪═════╡
-            │ b   ┆ 2   ┆ 4   │
-            │ b   ┆ 3   ┆ 2   │
-            │ c   ┆ 3   ┆ 1   │
-            │ a   ┆ 1   ┆ 5   │
-            └─────┴─────┴─────┘
-        """
-        from narwhals.group_by import GroupBy
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {"a": [1, 2, 3, 1], "b": ["a", "a", "b", "c"]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-        return GroupBy(self, *keys)
+            Let's define a dataframe-agnostic function:
 
-    def sort(
-        self,
-        by: str | Iterable[str],
-        *more_by: str,
-        descending: bool | Sequence[bool] = False,
-    ) -> Self:
-        r"""
-        Sort the dataframe by the given columns.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     first_distinct = df.select(nw.all().is_first_distinct())
+            ...     return nw.to_native(first_distinct)
 
-        Arguments:
-            by: Column(s) names to sort by.
+            We can then pass either pandas or Polars to `func`:
 
-            *more_by: Additional columns to sort by, specified as positional
-                       arguments.
+            >>> func(df_pd)  # doctest: +NORMALIZE_WHITESPACE
+                   a      b
+            0   True   True
+            1   True  False
+            2   True   True
+            3  False   True
+            >>> func(df_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (4, 2)
+            ┌───────┬───────┐
+            │ a     ┆ b     │
+            │ ---   ┆ ---   │
+            │ bool  ┆ bool  │
+            ╞═══════╪═══════╡
+            │ true  ┆ true  │
+            │ true  ┆ false │
+            │ true  ┆ true  │
+            │ false ┆ true  │
+            └───────┴───────┘
+        """
+        return self.__class__(lambda plx: self._call(plx).is_first_distinct())
 
-            descending: Sort in descending order. When sorting by multiple
-                         columns, can be specified per column by passing a
-                         sequence of booleans.
+    def is_last_distinct(self) -> Expr:
+        r"""Return a boolean mask indicating the last occurrence of each distinct value.
 
         Examples:
-            Pass a single column name to sort by that column.
-
-            >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "a": [1, 2, None],
-            ...         "b": [6.0, 5.0, 4.0],
-            ...         "c": ["a", "c", "b"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> dframe = df.sort("a")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 3)
-            ┌──────┬─────┬─────┐
-            │ a    ┆ b   ┆ c   │
-            │ ---  ┆ --- ┆ --- │
-            │ i64  ┆ f64 ┆ str │
-            ╞══════╪═════╪═════╡
-            │ null ┆ 4.0 ┆ b   │
-            │ 1    ┆ 6.0 ┆ a   │
-            │ 2    ┆ 5.0 ┆ c   │
-            └──────┴─────┴─────┘
-
-            Sort by multiple columns by passing a list of columns.
-
-            >>> dframe = df.sort(["c", "a"], descending=True)
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 3)
-            ┌──────┬─────┬─────┐
-            │ a    ┆ b   ┆ c   │
-            │ ---  ┆ --- ┆ --- │
-            │ i64  ┆ f64 ┆ str │
-            ╞══════╪═════╪═════╡
-            │ 2    ┆ 5.0 ┆ c   │
-            │ null ┆ 4.0 ┆ b   │
-            │ 1    ┆ 6.0 ┆ a   │
-            └──────┴─────┴─────┘
-
-            Or use positional arguments to sort by multiple columns in the same way.
-
-            >>> dframe = df.sort("c", "a", descending=[False, True])
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (3, 3)
-            ┌──────┬─────┬─────┐
-            │ a    ┆ b   ┆ c   │
-            │ ---  ┆ --- ┆ --- │
-            │ i64  ┆ f64 ┆ str │
-            ╞══════╪═════╪═════╡
-            │ 1    ┆ 6.0 ┆ a   │
-            │ null ┆ 4.0 ┆ b   │
-            │ 2    ┆ 5.0 ┆ c   │
-            └──────┴─────┴─────┘
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {"a": [1, 2, 3, 1], "b": ["a", "a", "b", "c"]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     last_distinct = df.select(nw.all().is_last_distinct())
+            ...     return nw.to_native(last_distinct)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)  # doctest: +NORMALIZE_WHITESPACE
+                   a      b
+            0  False  False
+            1   True   True
+            2   True   True
+            3   True   True
+            >>> func(df_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (4, 2)
+            ┌───────┬───────┐
+            │ a     ┆ b     │
+            │ ---   ┆ ---   │
+            │ bool  ┆ bool  │
+            ╞═══════╪═══════╡
+            │ false ┆ false │
+            │ true  ┆ true  │
+            │ true  ┆ true  │
+            │ true  ┆ true  │
+            └───────┴───────┘
         """
-        return super().sort(by, *more_by, descending=descending)
+        return self.__class__(lambda plx: self._call(plx).is_last_distinct())
 
-    def join(
+    def quantile(
         self,
-        other: Self,
-        *,
-        how: Literal["inner"] = "inner",
-        left_on: str | list[str],
-        right_on: str | list[str],
-    ) -> Self:
-        r"""
-        Join in SQL-like fashion.
+        quantile: float,
+        interpolation: Literal["nearest", "higher", "lower", "midpoint", "linear"],
+    ) -> Expr:
+        r"""Get quantile value.
+
+        Note:
+            pandas and Polars may have implementation differences for a given interpolation method.
 
         Arguments:
-            other: DataFrame to join with.
+            quantile : float
+                Quantile between 0.0 and 1.0.
+            interpolation : {'nearest', 'higher', 'lower', 'midpoint', 'linear'}
+                Interpolation method.
+
+        Examples:
+            >>> import narwhals as nw
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> data = {'a': list(range(50)), 'b': list(range(50, 100))}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     result = df.select(nw.col('a', 'b').quantile(0.5, interpolation='linear'))
+            ...     return nw.to_native(result)
 
-            how: {'inner'}
-                  Join strategy.
+            We can then pass either pandas or Polars to `func`:
 
-                  * *inner*: Returns rows that have matching values in both
-                              tables
+            >>> func(df_pd)  # doctest: +NORMALIZE_WHITESPACE
+                a   b
+            0  24.5  74.5
 
-            left_on: Name(s) of the left join column(s).
+            >>> func(df_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (1, 2)
+            ┌──────┬──────┐
+            │ a    ┆ b    │
+            │ ---  ┆ ---  │
+            │ f64  ┆ f64  │
+            ╞══════╪══════╡
+            │ 24.5 ┆ 74.5 │
+            └──────┴──────┘
+        """
+        return self.__class__(
+            lambda plx: self._call(plx).quantile(quantile, interpolation)
+        )
 
-            right_on: Name(s) of the right join column(s).
+    @property
+    def str(self) -> ExprStringNamespace:
+        return ExprStringNamespace(self)
+
+    @property
+    def dt(self) -> ExprDateTimeNamespace:
+        return ExprDateTimeNamespace(self)
 
-        Returns:
-            A new joined DataFrame
+
+class ExprStringNamespace:
+    def __init__(self, expr: Expr) -> None:
+        self._expr = expr
+
+    def ends_with(self, suffix: str) -> Expr:
+        return self._expr.__class__(
+            lambda plx: self._expr._call(plx).str.ends_with(suffix)
+        )
+
+    def head(self, n: int = 5) -> Expr:
+        """
+        Take the first n elements of each string.
+
+        Arguments:
+            n: Number of elements to take.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
-            >>> df_pl = pl.DataFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> other_df_pl = pl.DataFrame(
-            ...     {
-            ...         "apple": ["x", "y", "z"],
-            ...         "ham": ["a", "b", "d"],
-            ...     }
-            ... )
-            >>> df = nw.DataFrame(df_pl)
-            >>> other_df = nw.DataFrame(other_df_pl)
-            >>> dframe = df.join(other_df, left_on="ham", right_on="ham")
-            >>> dframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(dframe)
-            shape: (2, 4)
-            ┌─────┬─────┬─────┬───────┐
-            │ foo ┆ bar ┆ ham ┆ apple │
-            │ --- ┆ --- ┆ --- ┆ ---   │
-            │ i64 ┆ f64 ┆ str ┆ str   │
-            ╞═════╪═════╪═════╪═══════╡
-            │ 1   ┆ 6.0 ┆ a   ┆ x     │
-            │ 2   ┆ 7.0 ┆ b   ┆ y     │
-            └─────┴─────┴─────┴───────┘
-        """
-        return super().join(other, how=how, left_on=left_on, right_on=right_on)
-
-
-class LazyFrame(BaseFrame):
-    r"""
-    Representation of a Lazy computation graph/query against a DataFrame.
+            >>> data = {'lyrics': ['Atatata', 'taata', 'taatatata', 'zukkyun']}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-    This allows for whole-query optimisation in addition to parallelism, and
-    is the preferred (and highest-performance) mode of operation for narwhals.
+            We define a dataframe-agnostic function:
 
-    Arguments:
-        df: A pandas-like dataframe (Pandas, cuDF or Modin), a Polars dataframe,
-             a Polars lazyframe, a narwhals DataFrame or a narwhals LazyFrame.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(lyrics_head = nw.col('lyrics').str.head())
+            ...     return nw.to_native(df)
 
-        is_polars: if set to `True`, assume the dataframe to be of Polars type.
+            We can then pass either pandas or Polars to `func`:
 
-    Note:
-        Initialising `LazyFrame(...)` directly is equivalent to `DataFrame(...).lazy()`.
+            >>> func(df_pd)
+                  lyrics lyrics_head
+            0    Atatata       Atata
+            1      taata       taata
+            2  taatatata       taata
+            3    zukkyun       zukky
+            >>> func(df_pl)
+            shape: (4, 2)
+            ┌───────────┬─────────────┐
+            │ lyrics    ┆ lyrics_head │
+            │ ---       ┆ ---         │
+            │ str       ┆ str         │
+            ╞═══════════╪═════════════╡
+            │ Atatata   ┆ Atata       │
+            │ taata     ┆ taata       │
+            │ taatatata ┆ taata       │
+            │ zukkyun   ┆ zukky       │
+            └───────────┴─────────────┘
+        """
+
+        def func(plx: Any) -> Any:
+            if plx is get_polars():
+                return self._expr._call(plx).str.slice(0, n)
+            return self._expr._call(plx).str.head(n)
 
-    Examples:
-        Constructing a LazyFrame directly from a dictionary:
+        return self._expr.__class__(func)
 
-        >>> import polars as pl
-        >>> import narwhals as nw
-        >>> data = {"a": [1, 2], "b": [3, 4]}
-        >>> lf_pl = pl.LazyFrame(data)
-        >>> lf = nw.LazyFrame(lf_pl)
-        >>> dframe = lf.collect()
-        >>> dframe
-        ┌───────────────────────────────────────────────┐
-        | Narwhals DataFrame                            |
-        | Use `narwhals.to_native` to see native output |
-        └───────────────────────────────────────────────┘
-        >>> nw.to_native(dframe)
-        shape: (2, 2)
-        ┌─────┬─────┐
-        │ a   ┆ b   │
-        │ --- ┆ --- │
-        │ i64 ┆ i64 │
-        ╞═════╪═════╡
-        │ 1   ┆ 3   │
-        │ 2   ┆ 4   │
-        └─────┴─────┘
-    """
+    def to_datetime(self, format: str) -> Expr:  # noqa: A002
+        """
+        Convert to Datetime dtype.
 
-    def __init__(
-        self,
-        df: Any,
-        *,
-        is_polars: bool = False,
-    ) -> None:
-        self._is_polars = is_polars
-        if hasattr(df, "__narwhals_lazyframe__"):
-            self._dataframe: Any = df.__narwhals_lazyframe__()
-        elif is_polars or (
-            (pl := get_polars()) is not None
-            and isinstance(df, (pl.DataFrame, pl.LazyFrame))
-        ):
-            self._dataframe = df.lazy()
-            self._is_polars = True
-        elif (pd := get_pandas()) is not None and isinstance(df, pd.DataFrame):
-            self._dataframe = PandasDataFrame(df, implementation="pandas")
-        elif (mpd := get_modin()) is not None and isinstance(
-            df, mpd.DataFrame
-        ):  # pragma: no cover
-            self._dataframe = PandasDataFrame(df, implementation="modin")
-        elif (cudf := get_cudf()) is not None and isinstance(
-            df, cudf.DataFrame
-        ):  # pragma: no cover
-            self._dataframe = PandasDataFrame(df, implementation="cudf")
-        else:
-            msg = f"Expected pandas-like dataframe, Polars dataframe, or Polars lazyframe, got: {type(df)}"
-            raise TypeError(msg)
+        Notes:
+            pandas defaults to nanosecond time unit, Polars to microsecond.
+            Prior to pandas 2.0, nanoseconds were the only time unit supported
+            in pandas, with no ability to set any other one. The ability to
+            set the time unit in pandas, if the version permits, will arrive.
+
+        Arguments:
+            format: Format to parse strings with. Must be passed, as different
+                    dataframe libraries have different ways of auto-inferring
+                    formats.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> df_pd = pd.DataFrame({'a': ['2020-01-01', '2020-01-02']})
+            >>> df_pl = pl.DataFrame({'a': ['2020-01-01', '2020-01-02']})
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a').str.to_datetime(format='%Y-%m-%d'))
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
 
-    def __repr__(self) -> str:  # pragma: no cover
-        header = " Narwhals LazyFrame                            "
-        length = len(header)
-        return (
-            "┌"
-            + "─" * length
-            + "┐\n"
-            + f"|{header}|\n"
-            + "| Use `narwhals.to_native` to see native output |\n"
-            + "└"
-            + "─" * length
-            + "┘"
+            >>> func(df_pd)
+                       a
+            0 2020-01-01
+            1 2020-01-02
+            >>> func(df_pl)
+            shape: (2, 1)
+            ┌─────────────────────┐
+            │ a                   │
+            │ ---                 │
+            │ datetime[μs]        │
+            ╞═════════════════════╡
+            │ 2020-01-01 00:00:00 │
+            │ 2020-01-02 00:00:00 │
+            └─────────────────────┘
+        """
+        return self._expr.__class__(
+            lambda plx: self._expr._call(plx).str.to_datetime(format=format)
         )
 
-    def collect(self) -> DataFrame:
-        r"""
-        Materialize this LazyFrame into a DataFrame.
 
-        Returns:
-            DataFrame
+class ExprDateTimeNamespace:
+    def __init__(self, expr: Expr) -> None:
+        self._expr = expr
+
+    def year(self) -> Expr:
+        """
+        Extract year from underlying DateTime representation.
+
+        Returns the year number in the calendar date.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "a": ["a", "b", "a", "b", "b", "c"],
-            ...         "b": [1, 2, 3, 4, 5, 6],
-            ...         "c": [6, 5, 4, 3, 2, 1],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lf
-            ┌───────────────────────────────────────────────┐
-            | Narwhals LazyFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> df = lf.group_by("a").agg(nw.all().sum()).collect()
-            >>> df
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(df).sort("a")
-            shape: (3, 3)
-            ┌─────┬─────┬─────┐
-            │ a   ┆ b   ┆ c   │
-            │ --- ┆ --- ┆ --- │
-            │ str ┆ i64 ┆ i64 │
-            ╞═════╪═════╪═════╡
-            │ a   ┆ 4   ┆ 10  │
-            │ b   ┆ 11  ┆ 10  │
-            │ c   ┆ 6   ┆ 1   │
-            └─────┴─────┴─────┘
+            >>> data = {
+            ...        "datetime": [
+            ...         datetime(1978, 6, 1),
+            ...         datetime(2024, 12, 13),
+            ...         datetime(2065, 1, 1),
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.year().alias("year")
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                datetime  year
+            0 1978-06-01  1978
+            1 2024-12-13  2024
+            2 2065-01-01  2065
+            >>> func(df_pl)
+            shape: (3, 2)
+            ┌─────────────────────┬──────┐
+            │ datetime            ┆ year │
+            │ ---                 ┆ ---  │
+            │ datetime[μs]        ┆ i32  │
+            ╞═════════════════════╪══════╡
+            │ 1978-06-01 00:00:00 ┆ 1978 │
+            │ 2024-12-13 00:00:00 ┆ 2024 │
+            │ 2065-01-01 00:00:00 ┆ 2065 │
+            └─────────────────────┴──────┘
         """
-        return DataFrame(
-            self._dataframe.collect(),
-        )
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.year())
 
-    # inherited
-    def pipe(self, function: Callable[[Any], Self], *args: Any, **kwargs: Any) -> Self:
+    def month(self) -> Expr:
         """
-        Pipe function call.
+        Extract month from underlying DateTime representation.
+
+        Returns the month number starting from 1. The return value ranges from 1 to 12.
 
         Examples:
-            >>> import polars as pl
             >>> import pandas as pd
+            >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> data = {'a': [1,2,3], 'ba': [4,5,6]}
+            >>> data = {
+            ...        "datetime": [
+            ...         datetime(1978, 6, 1),
+            ...         datetime(2024, 12, 13),
+            ...         datetime(2065, 1, 1),
+            ...     ]
+            ... }
             >>> df_pd = pd.DataFrame(data)
-            >>> df_pl = pl.LazyFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-            Let's define a dataframe-agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
-            ...     df = df.pipe(lambda _df: _df.select([x for x in _df.columns if len(x) == 1]))
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.year().alias("year"),
+            ...         nw.col("datetime").dt.month().alias("month")
+            ...     )
             ...     return nw.to_native(df)
 
-            We can then pass either pandas or Polars:
+            We can then pass either pandas or Polars to `func`:
 
             >>> func(df_pd)
-               a
-            0  1
-            1  2
-            2  3
-            >>> func(df_pl).collect()
-            shape: (3, 1)
-            ┌─────┐
-            │ a   │
-            │ --- │
-            │ i64 │
-            ╞═════╡
-            │ 1   │
-            │ 2   │
-            │ 3   │
-            └─────┘
+                datetime  year  month
+            0 1978-06-01  1978      6
+            1 2024-12-13  2024     12
+            2 2065-01-01  2065      1
+            >>> func(df_pl)
+            shape: (3, 3)
+            ┌─────────────────────┬──────┬───────┐
+            │ datetime            ┆ year ┆ month │
+            │ ---                 ┆ ---  ┆ ---   │
+            │ datetime[μs]        ┆ i32  ┆ i8    │
+            ╞═════════════════════╪══════╪═══════╡
+            │ 1978-06-01 00:00:00 ┆ 1978 ┆ 6     │
+            │ 2024-12-13 00:00:00 ┆ 2024 ┆ 12    │
+            │ 2065-01-01 00:00:00 ┆ 2065 ┆ 1     │
+            └─────────────────────┴──────┴───────┘
         """
-        return super().pipe(function, *args, **kwargs)
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.month())
 
-    def drop_nulls(self) -> Self:
+    def day(self) -> Expr:
         """
-        Drop null values.
+        Extract day from underlying DateTime representation.
 
-        Notes:
-            pandas and Polars handle null values differently. Polars distinguishes
-            between NaN and Null, whereas pandas doesn't.
+        Returns the day of month starting from 1. The return value ranges from 1 to 31. (The last day of month differs by months.)
 
         Examples:
-            >>> import polars as pl
             >>> import pandas as pd
+            >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> data = {'a': [1., 2., None], 'ba': [1, None, 2.]}
+            >>> data = {
+            ...        "datetime": [
+            ...         datetime(1978, 6, 1),
+            ...         datetime(2024, 12, 13),
+            ...         datetime(2065, 1, 1),
+            ...     ]
+            ... }
             >>> df_pd = pd.DataFrame(data)
-            >>> df_pl = pl.LazyFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-            Let's define a dataframe-agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
-            ...     df = df.drop_nulls()
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.year().alias("year"),
+            ...         nw.col("datetime").dt.month().alias("month"),
+            ...         nw.col("datetime").dt.day().alias("day")
+            ...     )
             ...     return nw.to_native(df)
 
-            We can then pass either pandas or Polars:
+            We can then pass either pandas or Polars to `func`:
 
             >>> func(df_pd)
-                 a   ba
-            0  1.0  1.0
-            >>> func(df_pl).collect()
-            shape: (1, 2)
-            ┌─────┬─────┐
-            │ a   ┆ ba  │
-            │ --- ┆ --- │
-            │ f64 ┆ f64 │
-            ╞═════╪═════╡
-            │ 1.0 ┆ 1.0 │
-            └─────┴─────┘
+                datetime  year  month  day
+            0 1978-06-01  1978      6    1
+            1 2024-12-13  2024     12   13
+            2 2065-01-01  2065      1    1
+            >>> func(df_pl)
+            shape: (3, 4)
+            ┌─────────────────────┬──────┬───────┬─────┐
+            │ datetime            ┆ year ┆ month ┆ day │
+            │ ---                 ┆ ---  ┆ ---   ┆ --- │
+            │ datetime[μs]        ┆ i32  ┆ i8    ┆ i8  │
+            ╞═════════════════════╪══════╪═══════╪═════╡
+            │ 1978-06-01 00:00:00 ┆ 1978 ┆ 6     ┆ 1   │
+            │ 2024-12-13 00:00:00 ┆ 2024 ┆ 12    ┆ 13  │
+            │ 2065-01-01 00:00:00 ┆ 2065 ┆ 1     ┆ 1   │
+            └─────────────────────┴──────┴───────┴─────┘
         """
-        return super().drop_nulls()
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.day())
 
-    @property
-    def schema(self) -> dict[str, DType]:
-        r"""
-        Get a dict[column name, DType].
+    def hour(self) -> Expr:
+        """
+        Extract hour from underlying DateTime representation.
+
+        Returns the hour number from 0 to 23.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lf.schema # doctest: +SKIP
-            OrderedDict({'foo': Int64, 'bar': Float64, 'ham': String})
+            >>> data = {
+            ...     "datetime": [
+            ...         datetime(1978, 1, 1, 1),
+            ...         datetime(2024, 10, 13, 5),
+            ...         datetime(2065, 1, 1, 10),
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.hour().alias("hour")
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                         datetime  hour
+            0 1978-01-01 01:00:00     1
+            1 2024-10-13 05:00:00     5
+            2 2065-01-01 10:00:00    10
+            >>> func(df_pl)
+            shape: (3, 2)
+            ┌─────────────────────┬──────┐
+            │ datetime            ┆ hour │
+            │ ---                 ┆ ---  │
+            │ datetime[μs]        ┆ i8   │
+            ╞═════════════════════╪══════╡
+            │ 1978-01-01 01:00:00 ┆ 1    │
+            │ 2024-10-13 05:00:00 ┆ 5    │
+            │ 2065-01-01 10:00:00 ┆ 10   │
+            └─────────────────────┴──────┘
         """
-        return super().schema
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.hour())
 
-    @property
-    def columns(self) -> list[str]:
-        r"""
-        Get column names.
+    def minute(self) -> Expr:
+        """
+        Extract minutes from underlying DateTime representation.
 
-        Examples:
+        Returns the minute number from 0 to 59.
 
+        Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... ).select("foo", "bar")
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lf.columns
-            ['foo', 'bar']
+            >>> data = {
+            ...     "datetime": [
+            ...         datetime(1978, 1, 1, 1, 1),
+            ...         datetime(2024, 10, 13, 5, 30),
+            ...         datetime(2065, 1, 1, 10, 20),
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.hour().alias("hour"),
+            ...         nw.col("datetime").dt.minute().alias("minute"),
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                         datetime  hour  minute
+            0 1978-01-01 01:01:00     1       1
+            1 2024-10-13 05:30:00     5      30
+            2 2065-01-01 10:20:00    10      20
+            >>> func(df_pl)
+            shape: (3, 3)
+            ┌─────────────────────┬──────┬────────┐
+            │ datetime            ┆ hour ┆ minute │
+            │ ---                 ┆ ---  ┆ ---    │
+            │ datetime[μs]        ┆ i8   ┆ i8     │
+            ╞═════════════════════╪══════╪════════╡
+            │ 1978-01-01 01:01:00 ┆ 1    ┆ 1      │
+            │ 2024-10-13 05:30:00 ┆ 5    ┆ 30     │
+            │ 2065-01-01 10:20:00 ┆ 10   ┆ 20     │
+            └─────────────────────┴──────┴────────┘
         """
-        return super().columns
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.minute())
 
-    def with_columns(
-        self, *exprs: IntoExpr | Iterable[IntoExpr], **named_exprs: IntoExpr
-    ) -> Self:
-        r"""
-        Add columns to this LazyFrame.
+    def second(self) -> Expr:
+        """
+        Extract seconds from underlying DateTime representation.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> from datetime import datetime
+            >>> import narwhals as nw
+            >>> data = {
+            ...     "datetime": [
+            ...         datetime(1978, 1, 1, 1, 1, 1),
+            ...         datetime(2024, 10, 13, 5, 30, 14),
+            ...         datetime(2065, 1, 1, 10, 20, 30),
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-        Added columns will replace existing columns with the same name.
+            We define a dataframe-agnostic function:
 
-        Arguments:
-            *exprs: Column(s) to add, specified as positional arguments.
-                     Accepts expression input. Strings are parsed as column names, other
-                     non-expression inputs are parsed as literals.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.hour().alias("hour"),
+            ...         nw.col("datetime").dt.minute().alias("minute"),
+            ...         nw.col("datetime").dt.second().alias("second"),
+            ...     )
+            ...     return nw.to_native(df)
 
-            **named_exprs: Additional columns to add, specified as keyword arguments.
-                            The columns will be renamed to the keyword used.
+            We can then pass either pandas or Polars to `func`:
 
-        Returns:
-            LazyFrame: A new LazyFrame with the columns added.
+            >>> func(df_pd)
+                         datetime  hour  minute  second
+            0 1978-01-01 01:01:01     1       1       1
+            1 2024-10-13 05:30:14     5      30      14
+            2 2065-01-01 10:20:30    10      20      30
+            >>> func(df_pl)
+            shape: (3, 4)
+            ┌─────────────────────┬──────┬────────┬────────┐
+            │ datetime            ┆ hour ┆ minute ┆ second │
+            │ ---                 ┆ ---  ┆ ---    ┆ ---    │
+            │ datetime[μs]        ┆ i8   ┆ i8     ┆ i8     │
+            ╞═════════════════════╪══════╪════════╪════════╡
+            │ 1978-01-01 01:01:01 ┆ 1    ┆ 1      ┆ 1      │
+            │ 2024-10-13 05:30:14 ┆ 5    ┆ 30     ┆ 14     │
+            │ 2065-01-01 10:20:30 ┆ 10   ┆ 20     ┆ 30     │
+            └─────────────────────┴──────┴────────┴────────┘
+        """
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.second())
 
-        Note:
-            Creating a new LazyFrame using this method does not create a new copy of
-            existing data.
+    def millisecond(self) -> Expr:
+        """
+        Extract milliseconds from underlying DateTime representation.
 
         Examples:
-            Pass an expression to add it as a new column.
-
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "a": [1, 2, 3, 4],
-            ...         "b": [0.5, 4, 10, 13],
-            ...         "c": [True, True, False, True],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.with_columns((nw.col("a") * 2).alias("2a")).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (4, 4)
-            ┌─────┬──────┬───────┬─────┐
-            │ a   ┆ b    ┆ c     ┆ 2a  │
-            │ --- ┆ ---  ┆ ---   ┆ --- │
-            │ i64 ┆ f64  ┆ bool  ┆ i64 │
-            ╞═════╪══════╪═══════╪═════╡
-            │ 1   ┆ 0.5  ┆ true  ┆ 2   │
-            │ 2   ┆ 4.0  ┆ true  ┆ 4   │
-            │ 3   ┆ 10.0 ┆ false ┆ 6   │
-            │ 4   ┆ 13.0 ┆ true  ┆ 8   │
-            └─────┴──────┴───────┴─────┘
-        """
-        return super().with_columns(*exprs, **named_exprs)
+            >>> data = {
+            ...     "datetime": [
+            ...         datetime(1978, 1, 1, 1, 1, 1, 0),
+            ...         datetime(2024, 10, 13, 5, 30, 14, 505000),
+            ...         datetime(2065, 1, 1, 10, 20, 30, 67000),
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-    def select(
-        self,
-        *exprs: IntoExpr | Iterable[IntoExpr],
-        **named_exprs: IntoExpr,
-    ) -> Self:
-        r"""
-        Select columns from this LazyFrame.
+            We define a dataframe-agnostic function:
 
-        Arguments:
-            *exprs: Column(s) to select, specified as positional arguments.
-                     Accepts expression input. Strings are parsed as column names,
-                     other non-expression inputs are parsed as literals.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.hour().alias("hour"),
+            ...         nw.col("datetime").dt.minute().alias("minute"),
+            ...         nw.col("datetime").dt.second().alias("second"),
+            ...         nw.col("datetime").dt.millisecond().alias("millisecond")
+            ...     )
+            ...     return nw.to_native(df)
 
-            **named_exprs: Additional columns to select, specified as keyword arguments.
-                            The columns will be renamed to the keyword used.
+            We can then pass either pandas or Polars to `func`:
 
-        Examples:
-            Pass the name of a column to select that column.
+            >>> func(df_pd)
+                             datetime  hour  minute  second  millisecond
+            0 1978-01-01 01:01:01.000     1       1       1            0
+            1 2024-10-13 05:30:14.505     5      30      14          505
+            2 2065-01-01 10:20:30.067    10      20      30           67
+            >>> func(df_pl)
+            shape: (3, 5)
+            ┌─────────────────────────┬──────┬────────┬────────┬─────────────┐
+            │ datetime                ┆ hour ┆ minute ┆ second ┆ millisecond │
+            │ ---                     ┆ ---  ┆ ---    ┆ ---    ┆ ---         │
+            │ datetime[μs]            ┆ i8   ┆ i8     ┆ i8     ┆ i32         │
+            ╞═════════════════════════╪══════╪════════╪════════╪═════════════╡
+            │ 1978-01-01 01:01:01     ┆ 1    ┆ 1      ┆ 1      ┆ 0           │
+            │ 2024-10-13 05:30:14.505 ┆ 5    ┆ 30     ┆ 14     ┆ 505         │
+            │ 2065-01-01 10:20:30.067 ┆ 10   ┆ 20     ┆ 30     ┆ 67          │
+            └─────────────────────────┴──────┴────────┴────────┴─────────────┘
+        """
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.millisecond())
 
+    def microsecond(self) -> Expr:
+        """
+        Extract microseconds from underlying DateTime representation.
+
+        Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.select("foo").collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 1)
-            ┌─────┐
-            │ foo │
-            │ --- │
-            │ i64 │
-            ╞═════╡
-            │ 1   │
-            │ 2   │
-            │ 3   │
-            └─────┘
+            >>> data = {
+            ...     "datetime": [
+            ...         datetime(1978, 1, 1, 1, 1, 1, 0),
+            ...         datetime(2024, 10, 13, 5, 30, 14, 505000),
+            ...         datetime(2065, 1, 1, 10, 20, 30, 67000),
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-            Multiple columns can be selected by passing a list of column names.
+            We define a dataframe-agnostic function:
 
-            >>> lframe = lf.select(["foo", "bar"]).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 2)
-            ┌─────┬─────┐
-            │ foo ┆ bar │
-            │ --- ┆ --- │
-            │ i64 ┆ i64 │
-            ╞═════╪═════╡
-            │ 1   ┆ 6   │
-            │ 2   ┆ 7   │
-            │ 3   ┆ 8   │
-            └─────┴─────┘
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.hour().alias("hour"),
+            ...         nw.col("datetime").dt.minute().alias("minute"),
+            ...         nw.col("datetime").dt.second().alias("second"),
+            ...         nw.col("datetime").dt.microsecond().alias("microsecond")
+            ...     )
+            ...     return nw.to_native(df)
 
-            Multiple columns can also be selected using positional arguments instead of a
-            list. Expressions are also accepted.
+            We can then pass either pandas or Polars to `func`:
 
-            >>> lframe = lf.select(nw.col("foo"), nw.col("bar") + 1).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 2)
-            ┌─────┬─────┐
-            │ foo ┆ bar │
-            │ --- ┆ --- │
-            │ i64 ┆ i64 │
-            ╞═════╪═════╡
-            │ 1   ┆ 7   │
-            │ 2   ┆ 8   │
-            │ 3   ┆ 9   │
-            └─────┴─────┘
-
-            Use keyword arguments to easily name your expression inputs.
+            >>> func(df_pd)
+                             datetime  hour  minute  second  microsecond
+            0 1978-01-01 01:01:01.000     1       1       1            0
+            1 2024-10-13 05:30:14.505     5      30      14       505000
+            2 2065-01-01 10:20:30.067    10      20      30        67000
+            >>> func(df_pl)
+            shape: (3, 5)
+            ┌─────────────────────────┬──────┬────────┬────────┬─────────────┐
+            │ datetime                ┆ hour ┆ minute ┆ second ┆ microsecond │
+            │ ---                     ┆ ---  ┆ ---    ┆ ---    ┆ ---         │
+            │ datetime[μs]            ┆ i8   ┆ i8     ┆ i8     ┆ i32         │
+            ╞═════════════════════════╪══════╪════════╪════════╪═════════════╡
+            │ 1978-01-01 01:01:01     ┆ 1    ┆ 1      ┆ 1      ┆ 0           │
+            │ 2024-10-13 05:30:14.505 ┆ 5    ┆ 30     ┆ 14     ┆ 505000      │
+            │ 2065-01-01 10:20:30.067 ┆ 10   ┆ 20     ┆ 30     ┆ 67000       │
+            └─────────────────────────┴──────┴────────┴────────┴─────────────┘
+        """
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.microsecond())
 
-            >>> lframe = lf.select(threshold=nw.col('foo')*2).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 1)
-            ┌───────────┐
-            │ threshold │
-            │ ---       │
-            │ i64       │
-            ╞═══════════╡
-            │ 2         │
-            │ 4         │
-            │ 6         │
-            └───────────┘
+    def nanosecond(self) -> Expr:
         """
-        return super().select(*exprs, **named_exprs)
+        Extract Nanoseconds from underlying DateTime representation
 
-    def rename(self, mapping: dict[str, str]) -> Self:
-        r"""
-        Rename column names.
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> from datetime import datetime
+            >>> import narwhals as nw
+            >>> data = {
+            ...     "datetime": [
+            ...         datetime(1978, 1, 1, 1, 1, 1, 0),
+            ...         datetime(2024, 10, 13, 5, 30, 14, 500000),
+            ...         datetime(2065, 1, 1, 10, 20, 30, 60000)
+            ...     ]
+            ... }
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-        Arguments:
-            mapping: Key value pairs that map from old name to new name, or a
-                      function that takes the old name as input and returns the
-                      new name.
+            We define a dataframe-agnostic function:
 
-        Notes:
-            If existing names are swapped (e.g. 'A' points to 'B' and 'B'
-             points to 'A'), polars will block projection and predicate
-             pushdowns at this node.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...         nw.col("datetime").dt.hour().alias("hour"),
+            ...         nw.col("datetime").dt.minute().alias("minute"),
+            ...         nw.col("datetime").dt.second().alias("second"),
+            ...         nw.col("datetime").dt.nanosecond().alias("nanosecond")
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                             datetime  hour  minute  second  nanosecond
+            0 1978-01-01 01:01:01.000     1       1       1           0
+            1 2024-10-13 05:30:14.500     5      30      14   500000000
+            2 2065-01-01 10:20:30.060    10      20      30    60000000
+            >>> func(df_pl)
+            shape: (3, 5)
+            ┌─────────────────────────┬──────┬────────┬────────┬────────────┐
+            │ datetime                ┆ hour ┆ minute ┆ second ┆ nanosecond │
+            │ ---                     ┆ ---  ┆ ---    ┆ ---    ┆ ---        │
+            │ datetime[μs]            ┆ i8   ┆ i8     ┆ i8     ┆ i32        │
+            ╞═════════════════════════╪══════╪════════╪════════╪════════════╡
+            │ 1978-01-01 01:01:01     ┆ 1    ┆ 1      ┆ 1      ┆ 0          │
+            │ 2024-10-13 05:30:14.500 ┆ 5    ┆ 30     ┆ 14     ┆ 500000000  │
+            │ 2065-01-01 10:20:30.060 ┆ 10   ┆ 20     ┆ 30     ┆ 60000000   │
+            └─────────────────────────┴──────┴────────┴────────┴────────────┘
+        """
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.nanosecond())
+
+    def ordinal_day(self) -> Expr:
+        """
+        Get ordinal day.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import datetime
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.rename({"foo": "apple"}).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 3)
-            ┌───────┬─────┬─────┐
-            │ apple ┆ bar ┆ ham │
-            │ ---   ┆ --- ┆ --- │
-            │ i64   ┆ i64 ┆ str │
-            ╞═══════╪═════╪═════╡
-            │ 1     ┆ 6   ┆ a   │
-            │ 2     ┆ 7   ┆ b   │
-            │ 3     ┆ 8   ┆ c   │
-            └───────┴─────┴─────┘
+            >>> data = {'a': [datetime(2020, 1, 1), datetime(2020, 8, 3)]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(a_ordinal_day=nw.col('a').dt.ordinal_day())
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                       a  a_ordinal_day
+            0 2020-01-01              1
+            1 2020-08-03            216
+            >>> func(df_pl)
+            shape: (2, 2)
+            ┌─────────────────────┬───────────────┐
+            │ a                   ┆ a_ordinal_day │
+            │ ---                 ┆ ---           │
+            │ datetime[μs]        ┆ i16           │
+            ╞═════════════════════╪═══════════════╡
+            │ 2020-01-01 00:00:00 ┆ 1             │
+            │ 2020-08-03 00:00:00 ┆ 216           │
+            └─────────────────────┴───────────────┘
         """
-        return super().rename(mapping)
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.ordinal_day())
 
-    def head(self, n: int) -> Self:
-        r"""
-        Get the first `n` rows.
+    def total_minutes(self) -> Expr:
+        """
+        Get total minutes.
 
-        Arguments:
-            n: Number of rows to return.
+        Notes:
+            The function outputs the total minutes in the int dtype by default,
+            however, pandas may change the dtype to float when there are missing values,
+            consider using `fill_null()` and `cast` in this case.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import timedelta
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "a": [1, 2, 3, 4, 5, 6],
-            ...         "b": [7, 8, 9, 10, 11, 12],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.head(5).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (5, 2)
-            ┌─────┬─────┐
-            │ a   ┆ b   │
-            │ --- ┆ --- │
-            │ i64 ┆ i64 │
-            ╞═════╪═════╡
-            │ 1   ┆ 7   │
-            │ 2   ┆ 8   │
-            │ 3   ┆ 9   │
-            │ 4   ┆ 10  │
-            │ 5   ┆ 11  │
-            └─────┴─────┘
-            >>> lframe = lf.head(2).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
+            >>> data = {'a': [timedelta(minutes=10), timedelta(minutes=20, seconds=40)]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...       a_total_minutes = nw.col('a').dt.total_minutes()
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                            a  a_total_minutes
+            0 0 days 00:10:00               10
+            1 0 days 00:20:40               20
+            >>> func(df_pl)
             shape: (2, 2)
-            ┌─────┬─────┐
-            │ a   ┆ b   │
-            │ --- ┆ --- │
-            │ i64 ┆ i64 │
-            ╞═════╪═════╡
-            │ 1   ┆ 7   │
-            │ 2   ┆ 8   │
-            └─────┴─────┘
+            ┌──────────────┬─────────────────┐
+            │ a            ┆ a_total_minutes │
+            │ ---          ┆ ---             │
+            │ duration[μs] ┆ i64             │
+            ╞══════════════╪═════════════════╡
+            │ 10m          ┆ 10              │
+            │ 20m 40s      ┆ 20              │
+            └──────────────┴─────────────────┘
         """
-        return super().head(n)
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.total_minutes())
 
-    def drop(self, *columns: str | Iterable[str]) -> Self:
-        r"""
-        Remove columns from the LazyFrame.
+    def total_seconds(self) -> Expr:
+        """
+        Get total seconds.
 
-        Arguments:
-            *columns: Names of the columns that should be removed from the
-                      dataframe. Accepts column selector input.
+        Notes:
+            The function outputs the total seconds in the int dtype by default,
+            however, pandas may change the dtype to float when there are missing values,
+            consider using `fill_null()` and `cast` in this case.
 
         Examples:
-            Drop a single column by passing the name of that column.
-
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import timedelta
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.drop("ham").collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 2)
-            ┌─────┬─────┐
-            │ foo ┆ bar │
-            │ --- ┆ --- │
-            │ i64 ┆ f64 │
-            ╞═════╪═════╡
-            │ 1   ┆ 6.0 │
-            │ 2   ┆ 7.0 │
-            │ 3   ┆ 8.0 │
-            └─────┴─────┘
+            >>> data = {'a': [timedelta(seconds=10),
+            ...     timedelta(seconds=20, milliseconds=40)]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-            Use positional arguments to drop multiple columns.
+            We define a dataframe-agnostic function:
 
-            >>> lframe = lf.drop("foo", "ham").collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 1)
-            ┌─────┐
-            │ bar │
-            │ --- │
-            │ f64 │
-            ╞═════╡
-            │ 6.0 │
-            │ 7.0 │
-            │ 8.0 │
-            └─────┘
-        """
-        return super().drop(*columns)
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...       a_total_seconds = nw.col('a').dt.total_seconds()
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
 
-    def unique(self, subset: str | list[str]) -> Self:
+            >>> func(df_pd)
+                                   a  a_total_seconds
+            0        0 days 00:00:10               10
+            1 0 days 00:00:20.040000               20
+            >>> func(df_pl)
+            shape: (2, 2)
+            ┌──────────────┬─────────────────┐
+            │ a            ┆ a_total_seconds │
+            │ ---          ┆ ---             │
+            │ duration[μs] ┆ i64             │
+            ╞══════════════╪═════════════════╡
+            │ 10s          ┆ 10              │
+            │ 20s 40ms     ┆ 20              │
+            └──────────────┴─────────────────┘
         """
-        Drop duplicate rows from this LazyFrame.
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.total_seconds())
 
-        Arguments:
-            subset: Column name(s) to consider when identifying duplicate rows.
-                     If set to `None`, use all columns.
+    def total_milliseconds(self) -> Expr:
+        """
+        Get total milliseconds.
 
-        Returns:
-            LazyFrame: LazyFrame with unique rows.
+        Notes:
+            The function outputs the total milliseconds in the int dtype by default,
+            however, pandas may change the dtype to float when there are missing values,
+            consider using `fill_null()` and `cast` in this case.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import timedelta
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3, 1],
-            ...         "bar": ["a", "a", "a", "a"],
-            ...         "ham": ["b", "b", "b", "b"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.unique(None).collect().sort("foo")
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ str ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ a   ┆ b   │
-            │ 2   ┆ a   ┆ b   │
-            │ 3   ┆ a   ┆ b   │
-            └─────┴─────┴─────┘
-            >>> lframe = lf.unique(subset=["bar", "ham"]).collect().sort("foo")
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (1, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ str ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ a   ┆ b   │
-            └─────┴─────┴─────┘
-        """
-        return super().unique(subset)
+            >>> data = {'a': [timedelta(milliseconds=10),
+            ...     timedelta(milliseconds=20, microseconds=40)]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
 
-    def filter(self, *predicates: IntoExpr | Iterable[IntoExpr]) -> Self:
-        r"""
-        Filter the rows in the LazyFrame based on a predicate expression.
+            We define a dataframe-agnostic function:
 
-        The original order of the remaining rows is preserved.
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...       a_total_milliseconds = nw.col('a').dt.total_milliseconds()
+            ...     )
+            ...     return nw.to_native(df)
 
-        Arguments:
-            *predicates: Expression that evaluates to a boolean Series.
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                                   a  a_total_milliseconds
+            0 0 days 00:00:00.010000                    10
+            1 0 days 00:00:00.020040                    20
+            >>> func(df_pl)
+            shape: (2, 2)
+            ┌──────────────┬──────────────────────┐
+            │ a            ┆ a_total_milliseconds │
+            │ ---          ┆ ---                  │
+            │ duration[μs] ┆ i64                  │
+            ╞══════════════╪══════════════════════╡
+            │ 10ms         ┆ 10                   │
+            │ 20040µs      ┆ 20                   │
+            └──────────────┴──────────────────────┘
+        """
+        return self._expr.__class__(
+            lambda plx: self._expr._call(plx).dt.total_milliseconds()
+        )
+
+    def total_microseconds(self) -> Expr:
+        """
+        Get total microseconds.
+
+        Notes:
+            The function outputs the total microseconds in the int dtype by default,
+            however, pandas may change the dtype to float when there are missing values,
+            consider using `fill_null()` and `cast` in this case.
 
         Examples:
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import timedelta
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6, 7, 8],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
+            >>> data = {'a': [timedelta(microseconds=10),
+            ...     timedelta(milliseconds=1, microseconds=200)]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...       a_total_microseconds = nw.col('a').dt.total_microseconds()
+            ...     )
+            ...     return nw.to_native(df)
 
-            Filter on one condition:
+            We can then pass either pandas or Polars to `func`:
 
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.filter(nw.col("foo") > 1).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (2, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 2   ┆ 7   ┆ b   │
-            │ 3   ┆ 8   ┆ c   │
-            └─────┴─────┴─────┘
-
-            Filter on multiple conditions:
-
-            >>> lframe = lf.filter((nw.col("foo") < 3) & (nw.col("ham") == "a")).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (1, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            └─────┴─────┴─────┘
-
-            Provide multiple filters using `*args` syntax:
-
-            >>> lframe = lf.filter(
-            ...     nw.col("foo") == 1,
-            ...     nw.col("ham") == "a",
-            ... ).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (1, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            └─────┴─────┴─────┘
-
-            Filter on an OR condition:
-
-            >>> lframe = lf.filter((nw.col("foo") == 1) | (nw.col("ham") == "c")).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (2, 3)
-            ┌─────┬─────┬─────┐
-            │ foo ┆ bar ┆ ham │
-            │ --- ┆ --- ┆ --- │
-            │ i64 ┆ i64 ┆ str │
-            ╞═════╪═════╪═════╡
-            │ 1   ┆ 6   ┆ a   │
-            │ 3   ┆ 8   ┆ c   │
-            └─────┴─────┴─────┘
+            >>> func(df_pd)
+                                   a  a_total_microseconds
+            0 0 days 00:00:00.000010                    10
+            1 0 days 00:00:00.001200                  1200
+            >>> func(df_pl)
+            shape: (2, 2)
+            ┌──────────────┬──────────────────────┐
+            │ a            ┆ a_total_microseconds │
+            │ ---          ┆ ---                  │
+            │ duration[μs] ┆ i64                  │
+            ╞══════════════╪══════════════════════╡
+            │ 10µs         ┆ 10                   │
+            │ 1200µs       ┆ 1200                 │
+            └──────────────┴──────────────────────┘
         """
-        return super().filter(*predicates)
+        return self._expr.__class__(
+            lambda plx: self._expr._call(plx).dt.total_microseconds()
+        )
 
-    def group_by(self, *keys: str | Iterable[str]) -> LazyGroupBy:
-        r"""
-        Start a group by operation.
+    def total_nanoseconds(self) -> Expr:
+        """
+        Get total nanoseconds.
 
-        Arguments:
-            *keys:
-                Column(s) to group by. Accepts expression input. Strings are
-                parsed as column names.
+        Notes:
+            The function outputs the total nanoseconds in the int dtype by default,
+            however, pandas may change the dtype to float when there are missing values,
+            consider using `fill_null()` and `cast` in this case.
 
         Examples:
-            Group by one column and call `agg` to compute the grouped sum of
-            another column.
-
+            >>> import pandas as pd
             >>> import polars as pl
+            >>> from datetime import timedelta
             >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "a": ["a", "b", "a", "b", "c"],
-            ...         "b": [1, 2, 1, 3, 3],
-            ...         "c": [5, 4, 3, 2, 1],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.group_by("a").agg(nw.col("b").sum()).collect().sort("a")
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 2)
-            ┌─────┬─────┐
-            │ a   ┆ b   │
-            │ --- ┆ --- │
-            │ str ┆ i64 │
-            ╞═════╪═════╡
-            │ a   ┆ 2   │
-            │ b   ┆ 5   │
-            │ c   ┆ 3   │
-            └─────┴─────┘
+            >>> data = ['2024-01-01 00:00:00.000000001',
+            ...     '2024-01-01 00:00:00.000000002']
+            >>> df_pd = pd.DataFrame({'a': pd.to_datetime(data)})
+            >>> df_pl = (pl.DataFrame({'a': data}).with_columns(
+            ...     pl.col('a').str.to_datetime(time_unit='ns')))
 
-            Group by multiple columns by passing a list of column names.
+            We define a dataframe-agnostic function:
 
-            >>> lframe = lf.group_by(["a", "b"]).agg(nw.max("c")).collect().sort(["a", "b"])
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (4, 3)
-            ┌─────┬─────┬─────┐
-            │ a   ┆ b   ┆ c   │
-            │ --- ┆ --- ┆ --- │
-            │ str ┆ i64 ┆ i64 │
-            ╞═════╪═════╪═════╡
-            │ a   ┆ 1   ┆ 5   │
-            │ b   ┆ 2   ┆ 4   │
-            │ b   ┆ 3   ┆ 2   │
-            │ c   ┆ 3   ┆ 1   │
-            └─────┴─────┴─────┘
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.with_columns(
+            ...       a_diff_total_nanoseconds = nw.col('a').diff().dt.total_nanoseconds()
+            ...     )
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                                          a  a_diff_total_nanoseconds
+            0 2024-01-01 00:00:00.000000001                       NaN
+            1 2024-01-01 00:00:00.000000002                       1.0
+            >>> func(df_pl)
+            shape: (2, 2)
+            ┌───────────────────────────────┬──────────────────────────┐
+            │ a                             ┆ a_diff_total_nanoseconds │
+            │ ---                           ┆ ---                      │
+            │ datetime[ns]                  ┆ i64                      │
+            ╞═══════════════════════════════╪══════════════════════════╡
+            │ 2024-01-01 00:00:00.000000001 ┆ null                     │
+            │ 2024-01-01 00:00:00.000000002 ┆ 1                        │
+            └───────────────────────────────┴──────────────────────────┘
         """
-        from narwhals.group_by import LazyGroupBy
+        return self._expr.__class__(
+            lambda plx: self._expr._call(plx).dt.total_nanoseconds()
+        )
 
-        return LazyGroupBy(self, *keys)
 
-    def sort(
-        self,
-        by: str | Iterable[str],
-        *more_by: str,
-        descending: bool | Sequence[bool] = False,
-    ) -> Self:
-        r"""
-        Sort the LazyFrame by the given columns.
+def col(*names: str | Iterable[str]) -> Expr:
+    """
+    Instantiate an expression, similar to `polars.col`.
+    """
+    return Expr(lambda plx: plx.col(*names))
 
-        Arguments:
-            by: Column(s) to sort by. Accepts expression input. Strings are
-                 parsed as column names.
 
-            *more_by: Additional columns to sort by, specified as positional
-                       arguments.
+def all() -> Expr:
+    """
+    Instantiate an expression representing all columns, similar to `polars.all`.
+    """
+    return Expr(lambda plx: plx.all())
 
-            descending: Sort in descending order. When sorting by multiple
-                         columns, can be specified per column by passing a
-                         sequence of booleans.
 
-        Examples:
-            Pass a single column name to sort by that column.
+def len() -> Expr:
+    """
+    Return the number of rows.
 
-            >>> import polars as pl
-            >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "a": [1, 2, None],
-            ...         "b": [6.0, 5.0, 4.0],
-            ...         "c": ["a", "c", "b"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> lframe = lf.sort("a").collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 3)
-            ┌──────┬─────┬─────┐
-            │ a    ┆ b   ┆ c   │
-            │ ---  ┆ --- ┆ --- │
-            │ i64  ┆ f64 ┆ str │
-            ╞══════╪═════╪═════╡
-            │ null ┆ 4.0 ┆ b   │
-            │ 1    ┆ 6.0 ┆ a   │
-            │ 2    ┆ 5.0 ┆ c   │
-            └──────┴─────┴─────┘
-
-            Sort by multiple columns by passing a list of columns.
-
-            >>> lframe = lf.sort(["c", "a"], descending=True).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 3)
-            ┌──────┬─────┬─────┐
-            │ a    ┆ b   ┆ c   │
-            │ ---  ┆ --- ┆ --- │
-            │ i64  ┆ f64 ┆ str │
-            ╞══════╪═════╪═════╡
-            │ 2    ┆ 5.0 ┆ c   │
-            │ null ┆ 4.0 ┆ b   │
-            │ 1    ┆ 6.0 ┆ a   │
-            └──────┴─────┴─────┘
-
-            Or use positional arguments to sort by multiple columns in the same way.
-
-            >>> lframe = lf.sort("c", "a", descending=[False, True]).collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (3, 3)
-            ┌──────┬─────┬─────┐
-            │ a    ┆ b   ┆ c   │
-            │ ---  ┆ --- ┆ --- │
-            │ i64  ┆ f64 ┆ str │
-            ╞══════╪═════╪═════╡
-            │ 1    ┆ 6.0 ┆ a   │
-            │ null ┆ 4.0 ┆ b   │
-            │ 2    ┆ 5.0 ┆ c   │
-            └──────┴─────┴─────┘
-        """
-        return super().sort(by, *more_by, descending=descending)
+    Examples:
+        >>> import polars as pl
+        >>> import pandas as pd
+        >>> import narwhals as nw
+        >>> df_pd = pd.DataFrame({'a': [1, 2], 'b': [5, 10]})
+        >>> df_pl = pl.DataFrame({'a': [1, 2], 'b': [5, 10]})
 
-    def join(
-        self,
-        other: Self,
-        *,
-        how: Literal["inner"] = "inner",
-        left_on: str | list[str],
-        right_on: str | list[str],
-    ) -> Self:
-        r"""
-        Add a join operation to the Logical Plan.
+        Let's define a dataframe-agnostic function:
 
-        Arguments:
-            other: Lazy DataFrame to join with.
+        >>> def func(df_any):
+        ...    df = nw.from_native(df_any)
+        ...    df = df.select(nw.len())
+        ...    return nw.to_native(df)
+
+        We can then pass either pandas or Polars to `func`:
+
+        >>> func(df_pd)
+           len
+        0    2
+        >>> func(df_pl)
+        shape: (1, 1)
+        ┌─────┐
+        │ len │
+        │ --- │
+        │ u32 │
+        ╞═════╡
+        │ 2   │
+        └─────┘
+    """
 
-            how: {'inner'}
-                  Join strategy.
+    def func(plx: Any) -> Any:
+        if (
+            not hasattr(plx, "_implementation")
+            and (pl := get_polars()) is not None
+            and parse_version(pl.__version__) < parse_version("0.20.4")
+        ):  # pragma: no cover
+            return plx.count().alias("len")
+        return plx.len()
 
-                  * *inner*: Returns rows that have matching values in both
-                              tables
+    return Expr(func)
 
-            left_on: Join column of the left DataFrame.
 
-            right_on: Join column of the right DataFrame.
+def sum(*columns: str) -> Expr:
+    """
+    Sum all values.
 
-        Returns:
-            A new joined LazyFrame
+    Note:
+        Syntactic sugar for ``nw.col(columns).sum()``
 
-        Examples:
-            >>> import polars as pl
-            >>> import narwhals as nw
-            >>> lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "foo": [1, 2, 3],
-            ...         "bar": [6.0, 7.0, 8.0],
-            ...         "ham": ["a", "b", "c"],
-            ...     }
-            ... )
-            >>> other_lf_pl = pl.LazyFrame(
-            ...     {
-            ...         "apple": ["x", "y", "z"],
-            ...         "ham": ["a", "b", "d"],
-            ...     }
-            ... )
-            >>> lf = nw.LazyFrame(lf_pl)
-            >>> other_lf = nw.LazyFrame(other_lf_pl)
-            >>> lframe = lf.join(other_lf, left_on="ham", right_on="ham").collect()
-            >>> lframe
-            ┌───────────────────────────────────────────────┐
-            | Narwhals DataFrame                            |
-            | Use `narwhals.to_native` to see native output |
-            └───────────────────────────────────────────────┘
-            >>> nw.to_native(lframe)
-            shape: (2, 4)
-            ┌─────┬─────┬─────┬───────┐
-            │ foo ┆ bar ┆ ham ┆ apple │
-            │ --- ┆ --- ┆ --- ┆ ---   │
-            │ i64 ┆ f64 ┆ str ┆ str   │
-            ╞═════╪═════╪═════╪═══════╡
-            │ 1   ┆ 6.0 ┆ a   ┆ x     │
-            │ 2   ┆ 7.0 ┆ b   ┆ y     │
-            └─────┴─────┴─────┴───────┘
-        """
-        return super().join(other, how=how, left_on=left_on, right_on=right_on)
+    Arguments:
+        columns: Name(s) of the columns to use in the aggregation function
+
+    Examples:
+        >>> import pandas as pd
+        >>> import polars as pl
+        >>> import narwhals as nw
+        >>> df_pl = pl.DataFrame({"a": [1, 2]})
+        >>> df_pd = pd.DataFrame({"a": [1, 2]})
+
+    We define a dataframe-agnostic function:
+
+        >>> def func(df_any):
+        ...     df = nw.from_native(df_any)
+        ...     df = df.select(nw.sum('a'))
+        ...     return nw.to_native(df)
+
+    We can then pass either pandas or polars to `func`:
+
+        >>> func(df_pd)
+           a
+        0  3
+        >>> func(df_pl)
+        shape: (1, 1)
+        ┌─────┐
+        │ a   │
+        │ --- │
+        │ i64 │
+        ╞═════╡
+        │ 3   │
+        └─────┘
+    """
+
+    return Expr(lambda plx: plx.sum(*columns))
+
+
+def mean(*columns: str) -> Expr:
+    """
+    Get the mean value.
+
+    Note:
+        Syntactic sugar for ``nw.col(columns).mean()``
+
+    Arguments:
+        columns: Name(s) of the columns to use in the aggregation function
+
+    Examples:
+        >>> import pandas as pd
+        >>> import polars as pl
+        >>> import narwhals as nw
+        >>> df_pl = pl.DataFrame({"a": [1, 8, 3]})
+        >>> df_pd = pd.DataFrame({"a": [1, 8, 3]})
+
+    We define a dataframe agnostic function:
+
+        >>> def func(df_any):
+        ...     df = nw.from_native(df_any)
+        ...     df = df.select(nw.mean('a'))
+        ...     return nw.to_native(df)
+
+    We can then pass either pandas or Polars to `func`:
+
+        >>> func(df_pd)
+             a
+        0  4.0
+        >>> func(df_pl)
+        shape: (1, 1)
+        ┌─────┐
+        │ a   │
+        │ --- │
+        │ f64 │
+        ╞═════╡
+        │ 4.0 │
+        └─────┘
+    """
+
+    return Expr(lambda plx: plx.mean(*columns))
+
+
+def min(*columns: str) -> Expr:
+    """
+    Return the minimum value.
+
+    Note:
+       Syntactic sugar for ``nw.col(columns).min()``.
+
+    Arguments:
+        columns: Name(s) of the columns to use in the aggregation function.
+
+    Examples:
+        >>> import polars as pl
+        >>> import pandas as pd
+        >>> import narwhals as nw
+        >>> df_pd = pd.DataFrame({'a': [1, 2], 'b': [5, 10]})
+        >>> df_pl = pl.DataFrame({'a': [1, 2], 'b': [5, 10]})
+
+        Let's define a dataframe-agnostic function:
+
+        >>> def func(df_any):
+        ...    df = nw.from_native(df_any)
+        ...    df = df.select(nw.min('b'))
+        ...    return nw.to_native(df)
+
+        We can then pass either pandas or Polars to `func`:
+
+        >>> func(df_pd)
+           b
+        0  5
+        >>> func(df_pl)
+        shape: (1, 1)
+        ┌─────┐
+        │ b   │
+        │ --- │
+        │ i64 │
+        ╞═════╡
+        │ 5   │
+        └─────┘
+    """
+    return Expr(lambda plx: plx.min(*columns))
+
+
+def max(*columns: str) -> Expr:
+    """
+    Return the maximum value.
+
+    Note:
+       Syntactic sugar for ``nw.col(columns).max()``.
+
+    Arguments:
+        columns: Name(s) of the columns to use in the aggregation function.
+
+    Examples:
+        >>> import polars as pl
+        >>> import pandas as pd
+        >>> import narwhals as nw
+        >>> df_pd = pd.DataFrame({'a': [1, 2], 'b': [5, 10]})
+        >>> df_pl = pl.DataFrame({'a': [1, 2], 'b': [5, 10]})
+
+        Let's define a dataframe-agnostic function:
+
+        >>> def func(df_any):
+        ...    df = nw.from_native(df_any)
+        ...    df = df.select(nw.max('a'))
+        ...    return nw.to_native(df)
+
+        We can then pass either pandas or Polars to `func`:
+
+        >>> func(df_pd)
+           a
+        0  2
+        >>> func(df_pl)
+        shape: (1, 1)
+        ┌─────┐
+        │ a   │
+        │ --- │
+        │ i64 │
+        ╞═════╡
+        │ 2   │
+        └─────┘
+    """
+    return Expr(lambda plx: plx.max(*columns))
+
+
+def sum_horizontal(*exprs: IntoExpr | Iterable[IntoExpr]) -> Expr:
+    """
+    Instantiate an expression representing the horizontal sum of one or more expressions, similar to `polars.sum_horizontal`.
+    """
+    return Expr(
+        lambda plx: plx.sum_horizontal([extract_native(plx, v) for v in flatten(exprs)])
+    )
+
+
+__all__ = [
+    "Expr",
+]
```

### Comparing `narwhals-0.8.9/narwhals/dtypes.py` & `narwhals-0.9.0/narwhals/dtypes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Any
 
+from narwhals.dependencies import get_polars
 from narwhals.utils import isinstance_or_issubclass
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 class DType:
@@ -62,14 +63,17 @@
 
 class Boolean(DType): ...
 
 
 class Datetime(TemporalType): ...
 
 
+class Categorical(DType): ...
+
+
 class Date(TemporalType): ...
 
 
 def translate_dtype(plx: Any, dtype: DType) -> Any:
     if "polars" in str(type(dtype)):
         msg = (
             f"Expected Narwhals object, got: {type(dtype)}.\n\n"
@@ -98,24 +102,26 @@
         return plx.UInt16
     if dtype == UInt8:
         return plx.UInt8
     if dtype == String:
         return plx.String
     if dtype == Boolean:
         return plx.Boolean
+    if dtype == Categorical:
+        return plx.Categorical
     if dtype == Datetime:
         return plx.Datetime
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
 
 
 def to_narwhals_dtype(dtype: Any, *, is_polars: bool) -> DType:
     if not is_polars:
         return dtype  # type: ignore[no-any-return]
-    import polars as pl
+    pl = get_polars()
 
     if dtype == pl.Float64:
         return Float64()
     if dtype == pl.Float32:
         return Float32()
     if dtype == pl.Int64:
         return Int64()
@@ -133,11 +139,13 @@
         return UInt16()
     if dtype == pl.UInt8:
         return UInt8()
     if dtype == pl.String:
         return String()
     if dtype == pl.Boolean:
         return Boolean()
+    if dtype == pl.Categorical:
+        return Categorical()
     if dtype == pl.Datetime:
         return Datetime()
     msg = f"Unexpected dtype, got: {type(dtype)}"  # pragma: no cover
     raise AssertionError(msg)
```

### Comparing `narwhals-0.8.9/narwhals/functions.py` & `narwhals-0.9.0/narwhals/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Iterable
 from typing import Literal
 
+from narwhals.utils import validate_laziness
 from narwhals.utils import validate_same_library
 
 if TYPE_CHECKING:
     from narwhals.dataframe import DataFrame
     from narwhals.dataframe import LazyFrame
 
 
@@ -20,13 +21,14 @@
         raise NotImplementedError(
             "Only horizontal and vertical concatenations are supported"
         )
     if not items:
         raise ValueError("No items to concatenate")
     items = list(items)
     validate_same_library(items)
+    validate_laziness(items)
     first_item = items[0]
     plx = first_item.__narwhals_namespace__()
     return first_item.__class__(
         plx.concat([df._dataframe for df in items], how=how),
         is_polars=first_item._is_polars,
     )
```

### Comparing `narwhals-0.8.9/narwhals/translate.py` & `narwhals-0.9.0/narwhals/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,33 @@
         return Series(native_dataframe.__narwhals_series__())
     elif strict:  # pragma: no cover
         msg = f"Expected pandas-like dataframe, Polars dataframe, or Polars lazyframe, got: {type(native_dataframe)}"
         raise TypeError(msg)
     return native_dataframe  # type: ignore[no-any-return]  # pragma: no cover (todo)
 
 
+def get_native_namespace(obj: Any) -> Any:
+    """
+    Get native namespace from object.
+
+    Examples:
+        >>> import polars as pl
+        >>> import pandas as pd
+        >>> import narwhals as nw
+        >>> df = nw.from_native(pd.DataFrame({'a': [1,2,3]}))
+        >>> nw.get_native_namespace(df)
+        <module 'pandas'...>
+        >>> df = nw.from_native(pl.DataFrame({'a': [1,2,3]}))
+        >>> nw.get_native_namespace(df)
+        <module 'polars'...>
+    """
+    return obj.__native_namespace__()
+
+
 __all__ = [
     "get_pandas",
     "get_polars",
     "get_modin",
     "get_cudf",
+    "get_native_namespace",
     "to_native",
 ]
```

### Comparing `narwhals-0.8.9/narwhals/typing.py` & `narwhals-0.9.0/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/narwhals/_pandas_like/dataframe.py` & `narwhals-0.9.0/narwhals/_pandas_like/dataframe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
 
 import collections
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterable
 from typing import Literal
+from typing import overload
 
+from narwhals._pandas_like.utils import create_native_series
 from narwhals._pandas_like.utils import evaluate_into_exprs
 from narwhals._pandas_like.utils import horizontal_concat
 from narwhals._pandas_like.utils import translate_dtype
 from narwhals._pandas_like.utils import validate_dataframe_comparand
 from narwhals._pandas_like.utils import validate_indices
+from narwhals.translate import get_cudf
+from narwhals.translate import get_modin
+from narwhals.translate import get_pandas
 from narwhals.utils import flatten
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from typing_extensions import Self
 
@@ -44,14 +49,27 @@
         return self
 
     def __narwhals_namespace__(self) -> PandasNamespace:
         from narwhals._pandas_like.namespace import PandasNamespace
 
         return PandasNamespace(self._implementation)
 
+    def __native_namespace__(self) -> Any:
+        if self._implementation == "pandas":
+            return get_pandas()
+        if self._implementation == "modin":  # pragma: no cover
+            return get_modin()
+        if self._implementation == "cudf":  # pragma: no cover
+            return get_cudf()
+        msg = f"Expected pandas/modin/cudf, got: {type(self._implementation)}"  # pragma: no cover
+        raise AssertionError(msg)
+
+    def __len__(self) -> int:
+        return len(self._dataframe)
+
     def _validate_columns(self, columns: Sequence[str]) -> None:
         if len(columns) != len(set(columns)):
             counter = collections.Counter(columns)
             for col, count in counter.items():
                 if count > 1:
                     msg = f"Expected unique column names, got {col!r} {count} time(s)"
                     raise ValueError(
@@ -61,21 +79,39 @@
 
     def _from_dataframe(self, df: Any) -> Self:
         return self.__class__(
             df,
             implementation=self._implementation,
         )
 
-    def __getitem__(self, column_name: str) -> PandasSeries:
-        from narwhals._pandas_like.series import PandasSeries
+    @overload
+    def __getitem__(self, item: str) -> PandasSeries: ...
 
-        return PandasSeries(
-            self._dataframe.loc[:, column_name],
-            implementation=self._implementation,
-        )
+    @overload
+    def __getitem__(self, item: range | slice) -> PandasDataFrame: ...
+
+    def __getitem__(self, item: str | range | slice) -> PandasSeries | PandasDataFrame:
+        if isinstance(item, str):
+            from narwhals._pandas_like.series import PandasSeries
+
+            return PandasSeries(
+                self._dataframe.loc[:, item],
+                implementation=self._implementation,
+            )
+
+        elif isinstance(item, (range, slice)):
+            from narwhals._pandas_like.dataframe import PandasDataFrame
+
+            return PandasDataFrame(
+                self._dataframe.iloc[item], implementation=self._implementation
+            )
+
+        else:  # pragma: no cover
+            msg = f"Expected str, range or slice, got: {type(item)}"
+            raise TypeError(msg)
 
     # --- properties ---
     @property
     def columns(self) -> list[str]:
         return self._dataframe.columns.tolist()  # type: ignore[no-any-return]
 
     @property
@@ -87,24 +123,39 @@
     # --- reshape ---
     def select(
         self,
         *exprs: IntoPandasExpr | Iterable[IntoPandasExpr],
         **named_exprs: IntoPandasExpr,
     ) -> Self:
         new_series = evaluate_into_exprs(self, *exprs, **named_exprs)
+        if not new_series:
+            # return empty dataframe, like Polars does
+            return self._from_dataframe(self._dataframe.__class__())
         new_series = validate_indices(new_series)
         df = horizontal_concat(
             new_series,
             implementation=self._implementation,
         )
         return self._from_dataframe(df)
 
     def drop_nulls(self) -> Self:
         return self._from_dataframe(self._dataframe.dropna(axis=0))
 
+    def with_row_index(self, name: str) -> Self:
+        row_index = create_native_series(
+            range(len(self._dataframe)),
+            index=self._dataframe.index,
+            implementation=self._implementation,
+        ).alias(name)
+        return self._from_dataframe(
+            horizontal_concat(
+                [row_index._series, self._dataframe], implementation=self._implementation
+            )
+        )
+
     def filter(
         self,
         *predicates: IntoPandasExpr | Iterable[IntoPandasExpr],
     ) -> Self:
         from narwhals._pandas_like.namespace import PandasNamespace
 
         plx = PandasNamespace(self._implementation)
@@ -230,7 +281,33 @@
 
     def to_pandas(self) -> Any:
         if self._implementation == "pandas":
             return self._dataframe
         if self._implementation == "modin":  # pragma: no cover
             return self._dataframe._to_pandas()
         return self._dataframe.to_pandas()  # pragma: no cover
+
+    # --- descriptive ---
+    def is_duplicated(self: Self) -> PandasSeries:
+        from narwhals._pandas_like.series import PandasSeries
+
+        return PandasSeries(
+            self._dataframe.duplicated(keep=False),
+            implementation=self._implementation,
+        )
+
+    def is_empty(self: Self) -> bool:
+        return self._dataframe.empty  # type: ignore[no-any-return]
+
+    def is_unique(self: Self) -> PandasSeries:
+        from narwhals._pandas_like.series import PandasSeries
+
+        return PandasSeries(
+            ~self._dataframe.duplicated(keep=False),
+            implementation=self._implementation,
+        )
+
+    def null_count(self: Self) -> PandasDataFrame:
+        return PandasDataFrame(
+            self._dataframe.isnull().sum(axis=0).to_frame().transpose(),
+            implementation=self._implementation,
+        )
```

### Comparing `narwhals-0.8.9/narwhals/_pandas_like/group_by.py` & `narwhals-0.9.0/narwhals/_pandas_like/group_by.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,28 @@
 from typing import Callable
 from typing import Iterable
 from typing import Iterator
 
 from narwhals._pandas_like.utils import is_simple_aggregation
 from narwhals._pandas_like.utils import item
 from narwhals._pandas_like.utils import parse_into_exprs
+from narwhals._pandas_like.utils import series_from_iterable
+from narwhals.dependencies import get_pandas
 from narwhals.utils import parse_version
 from narwhals.utils import remove_prefix
 
 if TYPE_CHECKING:
     from narwhals._pandas_like.dataframe import PandasDataFrame
     from narwhals._pandas_like.expr import PandasExpr
     from narwhals._pandas_like.typing import IntoPandasExpr
 
+POLARS_TO_PANDAS_AGGREGATIONS = {
+    "len": "size",
+}
+
 
 class PandasGroupBy:
     def __init__(self, df: PandasDataFrame, keys: list[str]) -> None:
         self._df = df
         self._keys = list(keys)
         self._grouped = self._df._dataframe.groupby(
             list(self._keys),
@@ -84,37 +90,37 @@
 ) -> PandasDataFrame:
     """
     This should be the fastpath, but cuDF is too far behind to use it.
 
     - https://github.com/rapidsai/cudf/issues/15118
     - https://github.com/rapidsai/cudf/issues/15084
     """
-    import pandas as pd
-
-    from narwhals._pandas_like.namespace import PandasNamespace
+    pd = get_pandas()
 
     all_simple_aggs = True
     for expr in exprs:
         if not is_simple_aggregation(expr):
             all_simple_aggs = False
             break
 
     if all_simple_aggs:
         simple_aggregations: dict[str, tuple[str, str]] = {}
         for expr in exprs:
             if expr._depth == 0:
-                # e.g. agg(pl.len())
+                # e.g. agg(nw.len())
                 assert expr._output_names is not None
+                function_name = POLARS_TO_PANDAS_AGGREGATIONS.get(
+                    expr._function_name, expr._function_name
+                )
                 for output_name in expr._output_names:
-                    simple_aggregations[output_name] = (
-                        keys[0],
-                        expr._function_name.replace("len", "size"),
-                    )
+                    simple_aggregations[output_name] = (keys[0], function_name)
                 continue
 
+            # e.g. agg(nw.mean('a'))
+            assert expr._depth == 1
             assert expr._root_names is not None
             assert expr._output_names is not None
             for root_name, output_name in zip(expr._root_names, expr._output_names):
                 name = remove_prefix(expr._function_name, "col->")
                 simple_aggregations[output_name] = (root_name, name)
 
         aggs = collections.defaultdict(list)
@@ -136,31 +142,31 @@
         "Found complex group-by expression, which can't be expressed efficiently with the "
         "pandas API. If you can, please rewrite your query such that group-by aggregations "
         "are simple (e.g. mean, std, min, max, ...).",
         UserWarning,
         stacklevel=2,
     )
 
-    plx = PandasNamespace(implementation=implementation)
-
     def func(df: Any) -> Any:
         out_group = []
         out_names = []
         for expr in exprs:
             results_keys = expr._call(from_dataframe(df))
             for result_keys in results_keys:
                 out_group.append(item(result_keys._series))
                 out_names.append(result_keys.name)
-        return plx.make_native_series(name="", data=out_group, index=out_names)
+        return series_from_iterable(
+            out_group, index=out_names, name="", implementation=implementation
+        )
 
     if implementation == "pandas":
-        import pandas as pd
+        pd = get_pandas()
 
         if parse_version(pd.__version__) < parse_version("2.2.0"):  # pragma: no cover
             result_complex = grouped.apply(func)
-        else:  # pragma: no cover
+        else:
             result_complex = grouped.apply(func, include_groups=False)
     else:  # pragma: no cover
         result_complex = grouped.apply(func)
 
     result = result_complex.reset_index()
     return from_dataframe(result.loc[:, output_names])
```

### Comparing `narwhals-0.8.9/narwhals/_pandas_like/namespace.py` & `narwhals-0.9.0/narwhals/_pandas_like/namespace.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any
 from typing import Callable
 from typing import Iterable
 
 from narwhals import dtypes
 from narwhals._pandas_like.dataframe import PandasDataFrame
 from narwhals._pandas_like.expr import PandasExpr
+from narwhals._pandas_like.selectors import PandasSelectorNamespace
 from narwhals._pandas_like.series import PandasSeries
 from narwhals._pandas_like.utils import horizontal_concat
 from narwhals._pandas_like.utils import parse_into_exprs
 from narwhals._pandas_like.utils import series_from_iterable
 from narwhals._pandas_like.utils import vertical_concat
 from narwhals.utils import flatten
 
@@ -28,31 +29,21 @@
     UInt64 = dtypes.UInt64
     UInt32 = dtypes.UInt32
     UInt16 = dtypes.UInt16
     UInt8 = dtypes.UInt8
     Float64 = dtypes.Float64
     Float32 = dtypes.Float32
     Boolean = dtypes.Boolean
+    Categorical = dtypes.Categorical
     String = dtypes.String
     Datetime = dtypes.Datetime
 
-    def make_native_series(self, name: str, data: list[Any], index: Any) -> Any:
-        if self._implementation == "pandas":
-            import pandas as pd
-
-            return pd.Series(name=name, data=data, index=index)
-        if self._implementation == "modin":  # pragma: no cover
-            import modin.pandas as mpd
-
-            return mpd.Series(name=name, data=data, index=index)
-        if self._implementation == "cudf":  # pragma: no cover
-            import cudf
-
-            return cudf.Series(name=name, data=data, index=index)
-        raise NotImplementedError  # pragma: no cover
+    @property
+    def selectors(self) -> PandasSelectorNamespace:
+        return PandasSelectorNamespace(self._implementation)
 
     # --- not in spec ---
     def __init__(self, implementation: str) -> None:
         self._implementation = implementation
 
     def _create_expr_from_callable(  # noqa: PLR0913
         self,
```

### Comparing `narwhals-0.8.9/narwhals/_pandas_like/series.py` & `narwhals-0.9.0/narwhals/_pandas_like/series.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING
 from typing import Any
+from typing import Literal
 from typing import Sequence
 
 from narwhals._pandas_like.utils import item
 from narwhals._pandas_like.utils import reverse_translate_dtype
 from narwhals._pandas_like.utils import to_datetime
 from narwhals._pandas_like.utils import translate_dtype
 from narwhals._pandas_like.utils import validate_column_comparand
+from narwhals.dependencies import get_pandas
 from narwhals.utils import parse_version
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from narwhals._pandas_like.namespace import PandasNamespace
     from narwhals.dtypes import DType
@@ -73,20 +74,20 @@
     ) -> None:
         """Parameters
         ----------
         df
             DataFrame this column originates from.
         """
 
-        self._name = str(series.name) if series.name is not None else ""
+        self._name = series.name
         self._series = series
         self._implementation = implementation
         self._use_copy_false = False
         if self._implementation == "pandas":
-            import pandas as pd
+            pd = get_pandas()
 
             if parse_version(pd.__version__) < parse_version("3.0.0"):
                 self._use_copy_false = True
             else:  # pragma: no cover
                 pass
         else:  # pragma: no cover
             pass
@@ -114,15 +115,15 @@
         )
 
     def __len__(self) -> int:
         return self.shape[0]
 
     @property
     def name(self) -> str:
-        return self._name
+        return self._name  # type: ignore[no-any-return]
 
     @property
     def shape(self) -> tuple[int]:
         return self._series.shape  # type: ignore[no-any-return]
 
     @property
     def dtype(self) -> DType:
@@ -135,33 +136,40 @@
         ser = self._series
         dtype = reverse_translate_dtype(dtype)
         return self._from_series(ser.astype(dtype))
 
     def item(self) -> Any:
         return item(self._series)
 
+    def to_frame(self) -> Any:
+        from narwhals._pandas_like.dataframe import PandasDataFrame
+
+        return PandasDataFrame(
+            self._series.to_frame(), implementation=self._implementation
+        )
+
     def is_between(
         self, lower_bound: Any, upper_bound: Any, closed: str = "both"
     ) -> PandasSeries:
         ser = self._series
-        return self._from_series(ser.between(lower_bound, upper_bound, inclusive=closed))
+        if closed == "left":
+            res = ser.ge(lower_bound) & ser.lt(upper_bound)
+        elif closed == "right":
+            res = ser.gt(lower_bound) & ser.le(upper_bound)
+        elif closed == "none":
+            res = ser.gt(lower_bound) & ser.lt(upper_bound)
+        elif closed == "both":
+            res = ser.ge(lower_bound) & ser.le(upper_bound)
+        else:  # pragma: no cover
+            raise AssertionError
+        return self._from_series(res)
 
     def is_in(self, other: Any) -> PandasSeries:
-        import pandas as pd
-
         ser = self._series
-        with warnings.catch_warnings():
-            # np.find_common_type is deprecated.  Please use `np.result_type` or `np.promote_types`
-            warnings.filterwarnings(
-                "ignore",
-                message="np.find_common_type is deprecated.*",
-                category=DeprecationWarning,
-            )
-            res = ser.isin(other).convert_dtypes()
-        res[ser.isna()] = pd.NA
+        res = ser.isin(other)
         return self._from_series(res)
 
     # Binary comparisons
 
     def filter(self, other: Any) -> PandasSeries:
         ser = self._series
         other = validate_column_comparand(self._series.index, other)
@@ -342,15 +350,15 @@
 
     def drop_nulls(self) -> PandasSeries:
         ser = self._series
         return self._from_series(ser.dropna())
 
     def n_unique(self) -> int:
         ser = self._series
-        return ser.nunique()  # type: ignore[no-any-return]
+        return ser.nunique(dropna=False)  # type: ignore[no-any-return]
 
     def sample(
         self,
         n: int | None = None,
         fraction: float | None = None,
         *,
         with_replacement: bool = False,
@@ -383,15 +391,17 @@
     def sort(
         self,
         *,
         descending: bool | Sequence[bool] = False,
     ) -> PandasSeries:
         ser = self._series
         return self._from_series(
-            ser.sort_values(ascending=not descending).rename(self.name)
+            ser.sort_values(ascending=not descending, na_position="first").rename(
+                self.name
+            )
         )
 
     def alias(self, name: str) -> Self:
         ser = self._series
         return self._from_series(self._rename(ser, name))
 
     def to_numpy(self) -> Any:
@@ -416,14 +426,70 @@
         elif self._implementation == "cudf":  # pragma: no cover
             return self._series.to_pandas()
         elif self._implementation == "modin":  # pragma: no cover
             return self._series._to_pandas()
         msg = f"Unknown implementation: {self._implementation}"  # pragma: no cover
         raise AssertionError(msg)
 
+    # --- descriptive ---
+    def is_duplicated(self: Self) -> Self:
+        return self._from_series(self._series.duplicated(keep=False))
+
+    def is_empty(self: Self) -> bool:
+        return self._series.empty  # type: ignore[no-any-return]
+
+    def is_unique(self: Self) -> Self:
+        return self._from_series(~self._series.duplicated(keep=False))
+
+    def null_count(self: Self) -> int:
+        return self._series.isnull().sum()  # type: ignore[no-any-return]
+
+    def is_first_distinct(self: Self) -> Self:
+        return self._from_series(~self._series.duplicated(keep="first"))
+
+    def is_last_distinct(self: Self) -> Self:
+        return self._from_series(~self._series.duplicated(keep="last"))
+
+    def is_sorted(self: Self, *, descending: bool = False) -> bool:
+        if not isinstance(descending, bool):
+            msg = f"argument 'descending' should be boolean, found {type(descending)}"
+            raise TypeError(msg)
+
+        if descending:
+            return self._series.is_monotonic_decreasing  # type: ignore[no-any-return]
+        else:
+            return self._series.is_monotonic_increasing  # type: ignore[no-any-return]
+
+    def value_counts(self: Self, *, sort: bool = False, parallel: bool = False) -> Any:
+        """Parallel is unused, exists for compatibility"""
+        from narwhals._pandas_like.dataframe import PandasDataFrame
+
+        name_ = "index" if self._series.name is None else self._series.name
+        val_count = self._series.value_counts(dropna=False, sort=False).reset_index()
+        val_count.columns = [name_, "count"]
+        if sort:
+            val_count = val_count.sort_values(name_)
+
+        return PandasDataFrame(
+            val_count,
+            implementation=self._implementation,
+        )
+
+    def quantile(
+        self: Self,
+        quantile: float,
+        interpolation: Literal["nearest", "higher", "lower", "midpoint", "linear"],
+    ) -> Any:
+        return self._series.quantile(q=quantile, interpolation=interpolation)
+
+    def zip_with(self: Self, mask: Any, other: Any) -> PandasSeries:
+        ser = self._series
+        res = ser.where(mask._series, other._series)
+        return self._from_series(res)
+
     @property
     def str(self) -> PandasSeriesStringNamespace:
         return PandasSeriesStringNamespace(self)
 
     @property
     def dt(self) -> PandasSeriesDateTimeNamespace:
         return PandasSeriesDateTimeNamespace(self)
@@ -479,18 +545,84 @@
         )
 
     def second(self) -> PandasSeries:
         return self._series._from_series(
             self._series._series.dt.second,
         )
 
+    def millisecond(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.microsecond // 1000,
+        )
+
+    def microsecond(self) -> PandasSeries:
+        return self._series._from_series(self._series._series.dt.microsecond)
+
+    def nanosecond(self) -> PandasSeries:
+        return self._series._from_series(
+            (
+                (self._series._series.dt.microsecond * 1_000)
+                + self._series._series.dt.nanosecond
+            ),
+        )
+
     def ordinal_day(self) -> PandasSeries:
         ser = self._series._series
         year_start = ser.dt.year
         result = (
             ser.to_numpy().astype("datetime64[D]")
             - (year_start.to_numpy() - 1970).astype("datetime64[Y]")
         ).astype("int32") + 1
         dtype = "Int64[pyarrow]" if "pyarrow" in str(ser.dtype) else "int32"
         return self._series._from_series(
             self._series._series.__class__(result, dtype=dtype, name=year_start.name)
         )
+
+    def total_minutes(self) -> PandasSeries:
+        s = self._series._series.dt.total_seconds()
+        s_sign = (
+            2 * (s > 0).astype(int) - 1
+        )  # this calculates the sign of each series element
+        s_abs = s.abs() // 60
+        if ~s.isna().any():
+            s_abs = s_abs.astype(int)
+        return self._series._from_series(s_abs * s_sign)
+
+    def total_seconds(self) -> PandasSeries:
+        s = self._series._series.dt.total_seconds()
+        s_sign = (
+            2 * (s > 0).astype(int) - 1
+        )  # this calculates the sign of each series element
+        s_abs = s.abs() // 1
+        if ~s.isna().any():
+            s_abs = s_abs.astype(int)
+        return self._series._from_series(s_abs * s_sign)
+
+    def total_milliseconds(self) -> PandasSeries:
+        s = self._series._series.dt.total_seconds() * 1e3
+        s_sign = (
+            2 * (s > 0).astype(int) - 1
+        )  # this calculates the sign of each series element
+        s_abs = s.abs() // 1
+        if ~s.isna().any():
+            s_abs = s_abs.astype(int)
+        return self._series._from_series(s_abs * s_sign)
+
+    def total_microseconds(self) -> PandasSeries:
+        s = self._series._series.dt.total_seconds() * 1e6
+        s_sign = (
+            2 * (s > 0).astype(int) - 1
+        )  # this calculates the sign of each series element
+        s_abs = s.abs() // 1
+        if ~s.isna().any():
+            s_abs = s_abs.astype(int)
+        return self._series._from_series(s_abs * s_sign)
+
+    def total_nanoseconds(self) -> PandasSeries:
+        s = self._series._series.dt.total_seconds() * 1e9
+        s_sign = (
+            2 * (s > 0).astype(int) - 1
+        )  # this calculates the sign of each series element
+        s_abs = s.abs() // 1
+        if ~s.isna().any():
+            s_abs = s_abs.astype(int)
+        return self._series._from_series(s_abs * s_sign)
```

### Comparing `narwhals-0.8.9/narwhals/_pandas_like/typing.py` & `narwhals-0.9.0/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/narwhals/_pandas_like/utils.py` & `narwhals-0.9.0/narwhals/_pandas_like/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterable
 from typing import TypeVar
 
 from narwhals.dependencies import get_cudf
 from narwhals.dependencies import get_modin
+from narwhals.dependencies import get_numpy
 from narwhals.dependencies import get_pandas
 from narwhals.dependencies import get_pyarrow
 from narwhals.utils import flatten
 from narwhals.utils import isinstance_or_issubclass
 from narwhals.utils import parse_version
 
 T = TypeVar("T")
@@ -74,51 +75,86 @@
             return item(other._series)
         if other._series.index is not index and not (other._series.index == index).all():
             return other._series.set_axis(index, axis=0)
         return other._series
     raise AssertionError("Please report a bug")
 
 
-def maybe_evaluate_expr(df: PandasDataFrame, arg: Any) -> Any:
-    """Evaluate expression if it's an expression, otherwise return it as is."""
+def maybe_evaluate_expr(df: PandasDataFrame, expr: Any) -> Any:
+    """Evaluate `expr` if it's an expression, otherwise return it as is."""
     from narwhals._pandas_like.expr import PandasExpr
 
-    if isinstance(arg, PandasExpr):
-        return arg._call(df)
-    return arg
+    if isinstance(expr, PandasExpr):
+        return expr._call(df)
+    return expr
 
 
 def parse_into_exprs(
     implementation: str,
     *exprs: IntoPandasExpr | Iterable[IntoPandasExpr],
     **named_exprs: IntoPandasExpr,
 ) -> list[PandasExpr]:
+    """Parse each input as an expression (if it's not already one). See `parse_into_expr` for
+    more details."""
     out = [parse_into_expr(implementation, into_expr) for into_expr in flatten(exprs)]
     for name, expr in named_exprs.items():
         out.append(parse_into_expr(implementation, expr).alias(name))
     return out
 
 
 def parse_into_expr(implementation: str, into_expr: IntoPandasExpr) -> PandasExpr:
+    """Parse `into_expr` as an expression.
+
+    For example, in Polars, we can do both `df.select('a')` and `df.select(pl.col('a'))`.
+    We do the same in Narwhals:
+
+    - if `into_expr` is already an expression, just return it
+    - if it's a Series, then convert it to an expression
+    - if it's a numpy array, then convert it to a Series and then to an expression
+    - if it's a string, then convert it to an expression
+    - else, raise
+    """
     from narwhals._pandas_like.expr import PandasExpr
     from narwhals._pandas_like.namespace import PandasNamespace
     from narwhals._pandas_like.series import PandasSeries
 
     plx = PandasNamespace(implementation=implementation)
 
     if isinstance(into_expr, PandasExpr):
         return into_expr
     if isinstance(into_expr, PandasSeries):
         return plx._create_expr_from_series(into_expr)
     if isinstance(into_expr, str):
         return plx.col(into_expr)
+    if (np := get_numpy()) is not None and isinstance(into_expr, np.ndarray):
+        series = create_native_series(into_expr, implementation=implementation)
+        return plx._create_expr_from_series(series)
     msg = f"Expected IntoExpr, got {type(into_expr)}"  # pragma: no cover
     raise AssertionError(msg)
 
 
+def create_native_series(
+    iterable: Any,
+    implementation: str,
+    index: Any = None,
+) -> PandasSeries:
+    from narwhals._pandas_like.series import PandasSeries
+
+    if implementation == "pandas":
+        pd = get_pandas()
+        series = pd.Series(iterable, index=index, name="")
+    elif implementation == "modin":
+        mpd = get_modin()
+        series = mpd.Series(iterable, index=index, name="")
+    elif implementation == "cudf":
+        cudf = get_cudf()
+        series = cudf.Series(iterable, index=index, name="")
+    return PandasSeries(series, implementation=implementation)
+
+
 def evaluate_into_expr(
     df: PandasDataFrame, into_expr: IntoPandasExpr
 ) -> list[PandasSeries]:
     """
     Return list of raw columns.
     """
     expr = parse_into_expr(df._implementation, into_expr)
@@ -141,62 +177,89 @@
         if len(evaluated_expr) > 1:
             msg = "Named expressions must return a single column"  # pragma: no cover
             raise AssertionError(msg)
         series.append(evaluated_expr[0].alias(name))
     return series
 
 
-def register_expression_call(expr: ExprT, attr: str, *args: Any, **kwargs: Any) -> ExprT:
+def reuse_series_implementation(
+    expr: ExprT, attr: str, *args: Any, returns_scalar: bool = False, **kwargs: Any
+) -> ExprT:
+    """Reuse Series implementation for expression.
+
+    If Series.foo is already defined, and we'd like Expr.foo to be the same, we can
+    leverage this method to do that for us.
+
+    Arguments
+        expr: expression object.
+        attr: name of method.
+        returns_scalar: whether the Series version returns a scalar. In this case,
+            the expression version should return a 1-row Series.
+        args, kwargs: arguments and keyword arguments to pass to function.
+    """
     from narwhals._pandas_like.expr import PandasExpr
     from narwhals._pandas_like.namespace import PandasNamespace
-    from narwhals._pandas_like.series import PandasSeries
 
     plx = PandasNamespace(implementation=expr._implementation)
 
     def func(df: PandasDataFrame) -> list[PandasSeries]:
         out: list[PandasSeries] = []
         for column in expr._call(df):
             _out = getattr(column, attr)(
                 *[maybe_evaluate_expr(df, arg) for arg in args],
                 **{
                     arg_name: maybe_evaluate_expr(df, arg_value)
                     for arg_name, arg_value in kwargs.items()
                 },
             )
-            if isinstance(_out, PandasSeries):
-                out.append(_out)
-            else:
+            if returns_scalar:
                 out.append(plx._create_series_from_scalar(_out, column))
-        if expr._output_names is not None:
+            else:
+                out.append(_out)
+        if expr._output_names is not None:  # safety check
             assert [s._series.name for s in out] == expr._output_names
         return out
 
+    # Try tracking root and output names by combining them from all
+    # expressions appearing in args and kwargs. If any anonymous
+    # expression appears (e.g. nw.all()), then give up on tracking root names
+    # and just set it to None.
     root_names = copy(expr._root_names)
+    output_names = expr._output_names
     for arg in list(args) + list(kwargs.values()):
         if root_names is not None and isinstance(arg, PandasExpr):
             if arg._root_names is not None:
                 root_names.extend(arg._root_names)
             else:
                 root_names = None
+                output_names = None
                 break
         elif root_names is None:
+            output_names = None
             break
 
+    assert (output_names is None and root_names is None) or (
+        output_names is not None and root_names is not None
+    )  # safety check
+
     return plx._create_expr_from_callable(  # type: ignore[return-value]
         func,
         depth=expr._depth + 1,
         function_name=f"{expr._function_name}->{attr}",
         root_names=root_names,
-        output_names=expr._output_names,
+        output_names=output_names,
     )
 
 
-def register_namespace_expression_call(
+def reuse_series_namespace_implementation(
     expr: ExprT, namespace: str, attr: str, *args: Any, **kwargs: Any
 ) -> PandasExpr:
+    """Just like `reuse_series_implementation`, but for e.g. `Expr.dt.foo` instead
+    of `Expr.foo`.
+    """
     from narwhals._pandas_like.expr import PandasExpr
 
     return PandasExpr(
         lambda df: [
             getattr(getattr(series, namespace), attr)(*args, **kwargs)
             for series in expr._call(df)
         ],
@@ -213,41 +276,48 @@
     if len(s) != 1:
         msg = "Can only convert a Series of length 1 to a scalar"  # pragma: no cover
         raise AssertionError(msg)
     return s.iloc[0]
 
 
 def is_simple_aggregation(expr: PandasExpr) -> bool:
-    return (
-        expr._function_name is not None
-        and expr._depth is not None
-        and expr._depth < 2
-        # todo: avoid this one?
-        and (expr._root_names is not None or (expr._depth == 0))
-    )
+    """
+    Check if expr is a very simple one, such as:
+
+    - nw.col('a').mean()  # depth 1
+    - nw.mean('a')  # depth 1
+    - nw.len()  # depth 0
+
+    as opposed to, say
+
+    - nw.col('a').filter(nw.col('b')>nw.col('c')).max()
+
+    because then, we can use a fastpath in pandas.
+    """
+    return expr._depth < 2
 
 
 def horizontal_concat(dfs: list[Any], implementation: str) -> Any:
     """
     Concatenate (native) DataFrames horizontally.
 
     Should be in namespace.
     """
     if implementation == "pandas":
-        import pandas as pd
+        pd = get_pandas()
 
         if parse_version(pd.__version__) < parse_version("3.0.0"):
             return pd.concat(dfs, axis=1, copy=False)
         return pd.concat(dfs, axis=1)  # pragma: no cover
     if implementation == "cudf":  # pragma: no cover
-        import cudf
+        cudf = get_cudf()
 
         return cudf.concat(dfs, axis=1)
     if implementation == "modin":  # pragma: no cover
-        import modin.pandas as mpd
+        mpd = get_modin()
 
         return mpd.concat(dfs, axis=1)
     msg = f"Unknown implementation: {implementation}"  # pragma: no cover
     raise TypeError(msg)  # pragma: no cover
 
 
 def vertical_concat(dfs: list[Any], implementation: str) -> Any:
@@ -262,45 +332,45 @@
     cols = set(dfs[0].columns)
     for df in dfs:
         cols_current = set(df.columns)
         if cols_current != cols:
             msg = "unable to vstack, column names don't match"
             raise TypeError(msg)
     if implementation == "pandas":
-        import pandas as pd
+        pd = get_pandas()
 
         if parse_version(pd.__version__) < parse_version("3.0.0"):
             return pd.concat(dfs, axis=0, copy=False)
         return pd.concat(dfs, axis=0)  # pragma: no cover
     if implementation == "cudf":  # pragma: no cover
-        import cudf
+        cudf = get_cudf()
 
         return cudf.concat(dfs, axis=0)
     if implementation == "modin":  # pragma: no cover
-        import modin.pandas as mpd
+        mpd = get_modin()
 
         return mpd.concat(dfs, axis=0)
     msg = f"Unknown implementation: {implementation}"  # pragma: no cover
     raise TypeError(msg)  # pragma: no cover
 
 
 def series_from_iterable(
     data: Iterable[Any], name: str, index: Any, implementation: str
 ) -> Any:
     """Return native series."""
     if implementation == "pandas":
-        import pandas as pd
+        pd = get_pandas()
 
         return pd.Series(data, name=name, index=index, copy=False)
     if implementation == "cudf":  # pragma: no cover
-        import cudf
+        cudf = get_cudf()
 
         return cudf.Series(data, name=name, index=index)
     if implementation == "modin":  # pragma: no cover
-        import modin.pandas as mpd
+        mpd = get_modin()
 
         return mpd.Series(data, name=name, index=index)
     msg = f"Unknown implementation: {implementation}"  # pragma: no cover
     raise TypeError(msg)  # pragma: no cover
 
 
 def translate_dtype(dtype: Any) -> DType:
@@ -326,14 +396,16 @@
         return dtypes.Float64()
     if dtype in ("float32", "Float32", "Float32[pyarrow]"):
         return dtypes.Float32()
     if dtype in ("string", "string[python]", "string[pyarrow]"):
         return dtypes.String()
     if dtype in ("bool", "boolean", "boolean[pyarrow]"):
         return dtypes.Boolean()
+    if dtype in ("category",):
+        return dtypes.Categorical()
     if str(dtype).startswith("datetime64"):
         # todo: different time units and time zones
         return dtypes.Datetime()
     if dtype == "object":
         return dtypes.String()
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
@@ -361,23 +433,25 @@
     if isinstance_or_issubclass(dtype, dtypes.UInt32):
         return "uint32"
     if isinstance_or_issubclass(dtype, dtypes.UInt16):
         return "uint16"
     if isinstance_or_issubclass(dtype, dtypes.UInt8):
         return "uint8"
     if isinstance_or_issubclass(dtype, dtypes.String):
-        import pandas as pd
+        pd = get_pandas()
 
-        if parse_version(pd.__version__) >= parse_version("2.0.0"):
+        if pd is not None and parse_version(pd.__version__) >= parse_version("2.0.0"):
             if get_pyarrow() is not None:
                 return "string[pyarrow]"
             return "string[python]"  # pragma: no cover
         return "object"  # pragma: no cover
     if isinstance_or_issubclass(dtype, dtypes.Boolean):
         return "bool"
+    if isinstance_or_issubclass(dtype, dtypes.Categorical):
+        return "category"
     if isinstance_or_issubclass(dtype, dtypes.Datetime):
         # todo: different time units and time zones
         return "datetime64[us]"
     msg = f"Unknown dtype: {dtype}"  # pragma: no cover
     raise AssertionError(msg)
```

### Comparing `narwhals-0.8.9/tests/conftest.py` & `narwhals-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/group_by_test.py` & `narwhals-0.9.0/tests/group_by_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/test_common.py` & `narwhals-0.9.0/tests/test_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os
 import warnings
 from typing import Any
+from typing import Literal
 
 import numpy as np
 import pandas as pd
 import polars as pl
 import pytest
 from pandas.testing import assert_series_equal as pd_assert_series_equal
 from polars.testing import assert_series_equal as pl_assert_series_equal
@@ -568,25 +569,25 @@
     result = df.to_dict(as_series=True)
     expected = {
         "a": pd.Series([1, 3, 2], name="a"),
         "b": pd.Series([4, 4, 6], name="b"),
         "z": pd.Series([7.0, 8, 9], name="z"),
     }
     for key in expected:
-        pd_assert_series_equal(result[key], expected[key])
+        pd_assert_series_equal(nw.to_native(result[key]), expected[key])
 
     df = nw.DataFrame(df_polars)
     result = df.to_dict(as_series=True)
     expected = {
         "a": pl.Series("a", [1, 3, 2]),
         "b": pl.Series("b", [4, 4, 6]),
         "z": pl.Series("z", [7.0, 8, 9]),
     }
     for key in expected:
-        pl_assert_series_equal(result[key], expected[key])
+        pl_assert_series_equal(nw.to_native(result[key]), expected[key])
 
 
 @pytest.mark.parametrize(
     "df_raw", [df_pandas, df_lazy, df_pandas_nullable, df_pandas_pyarrow]
 )
 def test_any_all(df_raw: Any) -> None:
     df = nw.LazyFrame(df_raw)
@@ -644,7 +645,64 @@
         NotImplementedError, match="Cross-library comparisons aren't supported"
     ):
         nw.concat([df_left, df_right], how="vertical")
     with pytest.raises(
         NotImplementedError, match="Cross-library comparisons aren't supported"
     ):
         df_left.join(df_right, left_on=["a"], right_on=["a"], how="inner")
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
+def test_is_duplicated(df_raw: Any) -> None:
+    df = nw.DataFrame(df_raw)
+    result = nw.concat([df, df.head(1)]).is_duplicated()  # type: ignore [union-attr]
+    expected = np.array([True, False, False, True])
+    assert (result.to_numpy() == expected).all()
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
+@pytest.mark.parametrize(("threshold", "expected"), [(0, False), (10, True)])
+def test_is_empty(df_raw: Any, threshold: Any, expected: Any) -> None:
+    df = nw.DataFrame(df_raw)
+    result = df.filter(nw.col("a") > threshold).is_empty()
+    assert result == expected
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
+def test_is_unique(df_raw: Any) -> None:
+    df = nw.DataFrame(df_raw)
+    result = nw.concat([df, df.head(1)]).is_unique()  # type: ignore [union-attr]
+    expected = np.array([False, True, True, False])
+    assert (result.to_numpy() == expected).all()
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas_na, df_lazy_na.collect()])
+def test_null_count(df_raw: Any) -> None:
+    df = nw.DataFrame(df_raw)
+    result = nw.to_native(df.null_count())
+    expected = {"a": [1], "b": [0], "z": [1]}
+    compare_dicts(result, expected)
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas, df_polars])
+@pytest.mark.parametrize(
+    ("interpolation", "expected"),
+    [
+        ("lower", {"a": [1.0], "b": [4.0], "z": [7.0]}),
+        ("higher", {"a": [2.0], "b": [4.0], "z": [8.0]}),
+        ("midpoint", {"a": [1.5], "b": [4.0], "z": [7.5]}),
+        ("linear", {"a": [1.6], "b": [4.0], "z": [7.6]}),
+        ("nearest", {"a": [2.0], "b": [4.0], "z": [8.0]}),
+    ],
+)
+def test_quantile(
+    df_raw: Any,
+    interpolation: Literal["nearest", "higher", "lower", "midpoint", "linear"],
+    expected: dict[str, list[float]],
+) -> None:
+    q = 0.3
+
+    df = nw.from_native(df_raw)
+    result = nw.to_native(
+        df.select(nw.all().quantile(quantile=q, interpolation=interpolation))
+    )
+    compare_dicts(result, expected)
```

### Comparing `narwhals-0.8.9/tests/test_group_by.py` & `narwhals-0.9.0/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/test_str.py` & `narwhals-0.9.0/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/tpch_q1_test.py` & `narwhals-0.9.0/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/utils.py` & `narwhals-0.9.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/customer.parquet` & `narwhals-0.9.0/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/lineitem.parquet` & `narwhals-0.9.0/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/nation.parquet` & `narwhals-0.9.0/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/orders.parquet` & `narwhals-0.9.0/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/part.parquet` & `narwhals-0.9.0/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/partsupp.parquet` & `narwhals-0.9.0/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/region.parquet` & `narwhals-0.9.0/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/data/supplier.parquet` & `narwhals-0.9.0/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/cum_sum_test.py` & `narwhals-0.9.0/tests/expr/cum_sum_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/diff_test.py` & `narwhals-0.9.0/tests/expr/diff_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/fill_null_test.py` & `narwhals-0.9.0/tests/expr/fill_null_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/over_test.py` & `narwhals-0.9.0/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/shift_test.py` & `narwhals-0.9.0/tests/expr/shift_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/str/head_test.py` & `narwhals-0.9.0/tests/expr/str/head_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/expr/str/to_datetime_test.py` & `narwhals-0.9.0/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/frame/drop_nulls_test.py` & `narwhals-0.9.0/tests/frame/drop_nulls_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/frame/pipe_test.py` & `narwhals-0.9.0/tests/frame/pipe_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.9.0/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/hypothesis/test_concat.py` & `narwhals-0.9.0/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tests/hypothesis/test_join.py` & `narwhals-0.9.0/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/q1.py` & `narwhals-0.9.0/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/q2.py` & `narwhals-0.9.0/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/q3.py` & `narwhals-0.9.0/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/q4.py` & `narwhals-0.9.0/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/q5.py` & `narwhals-0.9.0/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.9.0/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/utils/bump_version.py` & `narwhals-0.9.0/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/utils/check_api_reference.py` & `narwhals-0.9.0/utils/check_api_reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,21 +122,35 @@
 # str
 
 # Check Expr vs Series
 expr = [i for i in nw.Expr(lambda: 0).__dir__() if not i[0].isupper() and i[0] != "_"]
 series = [
     i for i in nw.Series(pl.Series()).__dir__() if not i[0].isupper() and i[0] != "_"
 ]
+
 if missing := set(expr).difference(series).difference({"over"}):
     print("In expr but not in series")  # noqa: T201
     print(missing)  # noqa: T201
     ret = 1
 if (
     extra := set(series)
     .difference(expr)
-    .difference({"to_pandas", "to_numpy", "dtype", "name", "shape"})
+    .difference(
+        {
+            "to_pandas",
+            "to_numpy",
+            "dtype",
+            "name",
+            "shape",
+            "to_frame",
+            "is_empty",
+            "is_sorted",
+            "value_counts",
+            "zip_with",
+        }
+    )
 ):
     print("in series but not in expr")  # noqa: T201
     print(extra)  # noqa: T201
     ret = 1
 
 sys.exit(ret)
```

### Comparing `narwhals-0.8.9/LICENSE.md` & `narwhals-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.9/README.md` & `narwhals-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Narwhals
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="narwhals_small"
-		src="https://github.com/MarcoGorelli/narwhals/assets/33491632/26be901e-5383-49f2-9fbd-5c97b7696f27">
+		src="https://github.com/narwhals-dev/narwhals/assets/33491632/26be901e-5383-49f2-9fbd-5c97b7696f27">
 </h1>
 
 [![PyPI version](https://badge.fury.io/py/narwhals.svg)](https://badge.fury.io/py/narwhals)
 
 Extremely lightweight and extensible compatibility layer between Polars, pandas, Modin, and cuDF (and more!).
 
 - [Read the documentation](https://narwhals-dev.github.io/narwhals/)
@@ -16,50 +16,53 @@
 
 Seamlessly support all, without depending on any!
 
 - ✅ **Just use** a subset of **the Polars API**, no need to learn anything new
 - ✅ **No dependencies** (not even Polars), keep your library lightweight
 - ✅ Separate **lazy** and eager APIs
 - ✅ Use **Expressions**
-- ✅ 100% branch coverage, tested against pandas and Polars nightly builds!
-- ✅ Preserve your Index (if present) without it getting in the way!
+- ✅ 100% branch coverage, tested against pandas and Polars nightly builds
+- ✅ Preserve your Index (if present) without it getting in the way
+- ✅ **Zero 3rd party imports**, Narwhals only uses what you already have
 
 ## Used by
 
 Join the party!
 
-- https://github.com/FBruzzesi/timebasedcv
+- [scikit-lego](https://github.com/koaning/scikit-lego)
+- [scikit-playtime](https://github.com/koaning/scikit-playtime)
+- [timebasedcv](https://github.com/FBruzzesi/timebasedcv)
 
 ## Installation
 
 ```
 pip install narwhals
 ```
 Or just vendor it, it's only a bunch of pure-Python files.
 
 ## Usage
 
 There are three steps to writing dataframe-agnostic code using Narwhals:
 
 1. use `narwhals.from_native` to wrap a pandas/Polars/Modin/cuDF
    DataFrame/LazyFrame in a Narwhals class
-2. use the [subset of the Polars API supported by Narwhals](https://marcogorelli.github.io/narwhals/api-reference/narwhals/)
+2. use the [subset of the Polars API supported by Narwhals](https://narwhals-dev.github.io/narwhals/api-reference/)
 3. use `narwhals.to_native` to return an object to the user in its original
    dataframe flavour. For example:
 
    - if you started with pandas, you'll get pandas back
    - if you started with Polars, you'll get Polars back
    - if you started with Modin, you'll get Modin back (and compute will be distributed)
    - if you started with cuDF, you'll get cuDF back (and compute will happen on GPU)
 
 ## What about Ibis?
 
 Like Ibis, Narwhals aims to enable dataframe-agnostic code. However, Narwhals comes with **zero** dependencies,
 is about as lightweight as it gets, and is aimed at library developers rather than at end users. It also does
-not aim to support as many backends, preferring to instead focus on dataframes. So, which should you use?
+not aim to support as many backends, instead preferring to focus on dataframes. So, which should you use?
 
 - If you need to run complicated analyses and aren't too bothered about package size: Ibis!
 - If you're a library maintainer and want the thinnest-possible layer to get cross-dataframe library support: Narwhals!
 
 Here is the package size increase which would result from installing each tool in a non-pandas
 environment:
 
@@ -68,17 +71,17 @@
 ## Example
 
 See the [tutorial](https://narwhals-dev.github.io/narwhals/basics/dataframe/) for several examples!
 
 ## Scope
 
 - Do you maintain a dataframe-consuming library?
-- Is there a Polars function which you'd like Narwhals to have, which would make your work easier?
+- Do you have a specific Polars function in mind that you would like Narwhals to have in order to make your work easier?
 
-If, I'd love to hear from you!
+If you said yes to both, we'd love to hear from you!
 
 **Note**: You might suspect that this is a secret ploy to infiltrate the Polars API everywhere.
 Indeed, you may suspect that.
 
 ## Why "Narwhals"?
 
 [Coz they are so awesome](https://youtu.be/ykwqXuMPsoc?si=A-i8LdR38teYsos4).
```

### Comparing `narwhals-0.8.9/pyproject.toml` & `narwhals-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.9"
+version = "0.9.0"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,16 +18,16 @@
 ]
 
 [project.optional-dependencies]
 pandas = ["pandas>=1.1.5"]
 polars = ["polars>=0.20.3"]
 
 [project.urls]
-"Homepage" = "https://github.com/MarcoGorelli/narwhals"
-"Bug Tracker" = "https://github.com/MarcoGorelli/narwhals"
+"Homepage" = "https://github.com/narwhals-dev/narwhals"
+"Bug Tracker" = "https://github.com/narwhals-dev/narwhals"
 
 [tool.ruff]
 line-length = 90
 fix = true
 target-version = "py38"
 
 lint.select = [
```

### Comparing `narwhals-0.8.9/PKG-INFO` & `narwhals-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.9
+Version: 0.9.0
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
-Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
-Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
+Project-URL: Homepage, https://github.com/narwhals-dev/narwhals
+Project-URL: Bug Tracker, https://github.com/narwhals-dev/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Provides-Extra: pandas
@@ -18,15 +18,15 @@
 
 # Narwhals
 
 <h1 align="center">
 	<img
 		width="400"
 		alt="narwhals_small"
-		src="https://github.com/MarcoGorelli/narwhals/assets/33491632/26be901e-5383-49f2-9fbd-5c97b7696f27">
+		src="https://github.com/narwhals-dev/narwhals/assets/33491632/26be901e-5383-49f2-9fbd-5c97b7696f27">
 </h1>
 
 [![PyPI version](https://badge.fury.io/py/narwhals.svg)](https://badge.fury.io/py/narwhals)
 
 Extremely lightweight and extensible compatibility layer between Polars, pandas, Modin, and cuDF (and more!).
 
 - [Read the documentation](https://narwhals-dev.github.io/narwhals/)
@@ -34,50 +34,53 @@
 
 Seamlessly support all, without depending on any!
 
 - ✅ **Just use** a subset of **the Polars API**, no need to learn anything new
 - ✅ **No dependencies** (not even Polars), keep your library lightweight
 - ✅ Separate **lazy** and eager APIs
 - ✅ Use **Expressions**
-- ✅ 100% branch coverage, tested against pandas and Polars nightly builds!
-- ✅ Preserve your Index (if present) without it getting in the way!
+- ✅ 100% branch coverage, tested against pandas and Polars nightly builds
+- ✅ Preserve your Index (if present) without it getting in the way
+- ✅ **Zero 3rd party imports**, Narwhals only uses what you already have
 
 ## Used by
 
 Join the party!
 
-- https://github.com/FBruzzesi/timebasedcv
+- [scikit-lego](https://github.com/koaning/scikit-lego)
+- [scikit-playtime](https://github.com/koaning/scikit-playtime)
+- [timebasedcv](https://github.com/FBruzzesi/timebasedcv)
 
 ## Installation
 
 ```
 pip install narwhals
 ```
 Or just vendor it, it's only a bunch of pure-Python files.
 
 ## Usage
 
 There are three steps to writing dataframe-agnostic code using Narwhals:
 
 1. use `narwhals.from_native` to wrap a pandas/Polars/Modin/cuDF
    DataFrame/LazyFrame in a Narwhals class
-2. use the [subset of the Polars API supported by Narwhals](https://marcogorelli.github.io/narwhals/api-reference/narwhals/)
+2. use the [subset of the Polars API supported by Narwhals](https://narwhals-dev.github.io/narwhals/api-reference/)
 3. use `narwhals.to_native` to return an object to the user in its original
    dataframe flavour. For example:
 
    - if you started with pandas, you'll get pandas back
    - if you started with Polars, you'll get Polars back
    - if you started with Modin, you'll get Modin back (and compute will be distributed)
    - if you started with cuDF, you'll get cuDF back (and compute will happen on GPU)
 
 ## What about Ibis?
 
 Like Ibis, Narwhals aims to enable dataframe-agnostic code. However, Narwhals comes with **zero** dependencies,
 is about as lightweight as it gets, and is aimed at library developers rather than at end users. It also does
-not aim to support as many backends, preferring to instead focus on dataframes. So, which should you use?
+not aim to support as many backends, instead preferring to focus on dataframes. So, which should you use?
 
 - If you need to run complicated analyses and aren't too bothered about package size: Ibis!
 - If you're a library maintainer and want the thinnest-possible layer to get cross-dataframe library support: Narwhals!
 
 Here is the package size increase which would result from installing each tool in a non-pandas
 environment:
 
@@ -86,17 +89,17 @@
 ## Example
 
 See the [tutorial](https://narwhals-dev.github.io/narwhals/basics/dataframe/) for several examples!
 
 ## Scope
 
 - Do you maintain a dataframe-consuming library?
-- Is there a Polars function which you'd like Narwhals to have, which would make your work easier?
+- Do you have a specific Polars function in mind that you would like Narwhals to have in order to make your work easier?
 
-If, I'd love to hear from you!
+If you said yes to both, we'd love to hear from you!
 
 **Note**: You might suspect that this is a secret ploy to infiltrate the Polars API everywhere.
 Indeed, you may suspect that.
 
 ## Why "Narwhals"?
 
 [Coz they are so awesome](https://youtu.be/ykwqXuMPsoc?si=A-i8LdR38teYsos4).
```

