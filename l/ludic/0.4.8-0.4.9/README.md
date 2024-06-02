# Comparing `tmp/ludic-0.4.8.tar.gz` & `tmp/ludic-0.4.9.tar.gz`

## Comparing `ludic-0.4.8.tar` & `ludic-0.4.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.8/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.8/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.8/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.8/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/catalog.md
--rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/getting-started.md
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/click_to_load.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/__init__.py
--rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/attrs.py
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/components.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/format.py
--rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/types.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/forms.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/headers.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/icons.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/items.py
--rw-r--r--   0        0        0     9261 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/messages.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/tables.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/typography.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/collect.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/themes.py
--rw-r--r--   0        0        0    27206 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/types.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/__init__.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/parsers.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/responses.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/__init__.py
--rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_components.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/styles/test_styles.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.8/LICENCE
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.8/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.9/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.9/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.9/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/catalog.md
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/getting-started.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.9/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/click_to_load.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.9/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/__init__.py
+-rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/attrs.py
+-rw-r--r--   0        0        0     9896 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/components.py
+-rw-r--r--   0        0        0     7003 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/format.py
+-rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/types.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/headers.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/icons.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/items.py
+-rw-r--r--   0        0        0     9261 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/styles/collect.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/styles/themes.py
+-rw-r--r--   0        0        0    27206 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/responses.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.9/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/__init__.py
+-rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/test_components.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.9/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.9/LICENCE
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.9/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.9/PKG-INFO
```

### Comparing `ludic-0.4.8/.pre-commit-config.yaml` & `ludic-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/CONTRIBUTING.md` & `ludic-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/mkdocs.yaml` & `ludic-0.4.9/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/.github/workflows/publish.yaml` & `ludic-0.4.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/.github/workflows/test.yaml` & `ludic-0.4.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/catalog.md` & `ludic-0.4.9/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/components.md` & `ludic-0.4.9/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/getting-started.md` & `ludic-0.4.9/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/htmx.md` & `ludic-0.4.9/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/index.md` & `ludic-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/styles.md` & `ludic-0.4.9/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/web-framework.md` & `ludic-0.4.9/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/docs/assets/ludic.png` & `ludic-0.4.9/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/README.md` & `ludic-0.4.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/__init__.py` & `ludic-0.4.9/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/bulk_update.py` & `ludic-0.4.9/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/click_to_edit.py` & `ludic-0.4.9/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/click_to_load.py` & `ludic-0.4.9/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/delete_row.py` & `ludic-0.4.9/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/edit_row.py` & `ludic-0.4.9/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/infinite_scroll.py` & `ludic-0.4.9/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/examples/lazy_loading.py` & `ludic-0.4.9/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/attrs.py` & `ludic-0.4.9/ludic/attrs.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/base.py` & `ludic-0.4.9/ludic/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta
-from collections.abc import Callable, Iterator, Mapping, MutableMapping, Sequence
+from collections.abc import Iterator, Mapping, MutableMapping, Sequence
 from typing import (
     Any,
     ClassVar,
     Generic,
     Never,
     TypeAlias,
     TypedDict,
@@ -117,52 +117,46 @@
         )
 
     def _format_attributes(
         self, classes: list[str] | None = None, is_html: bool = False
     ) -> str:
         attrs: dict[str, Any]
         if is_html:
-            attrs = format_attrs(type(self), dict(self.attrs), is_html=True)
+            attrs = format_attrs(type(self), self.attrs, is_html=True)
         else:
             attrs = self.aliased_attrs
 
         if classes:
             if "class" in attrs:
                 attrs["class"] += " " + " ".join(classes)
             else:
                 attrs["class"] = " ".join(classes)
 
         return " ".join(
             f'{key}="{value}"' if '"' not in value else f"{key}='{value}'"
             for key, value in attrs.items()
         )
 
-    def _format_children(
-        self,
-        format_fun: Callable[[Any], str] = format_element,
-    ) -> str:
-        formatted = []
+    def _format_children(self) -> str:
+        formatted = ""
         for child in self.children:
-            if isinstance(child, BaseElement):
+            if self.context and isinstance(child, BaseElement):
                 child.context.update(self.context)
-            formatted.append(format_fun(child))
-        return "".join(formatted)
+            formatted += format_element(child)
+        return formatted
 
     @property
     def aliased_attrs(self) -> dict[str, Any]:
         """Attributes as a dict with keys renamed to their aliases."""
-        return format_attrs(type(self), dict(self.attrs))
+        return format_attrs(type(self), self.attrs)
 
     @property
     def text(self) -> str:
         """Get the text content of the element."""
-        return "".join(
-            child.text if isinstance(child, BaseElement) else str(child)
-            for child in self.children
-        )
+        return "".join(getattr(child, "text", str(child)) for child in self.children)
 
     @property
     def theme(self) -> Theme:
         """Get the theme of the element."""
         if context_theme := self.context.get("theme"):
             if isinstance(context_theme, Theme):
                 return context_theme
@@ -211,15 +205,15 @@
         return element
 
     def to_html(self) -> str:
         """Convert an element tree to an HTML string."""
         dom = self
         classes = list(dom.classes)
 
-        while dom != (rendered_dom := dom.render()):
+        while id(dom) != id(rendered_dom := dom.render()):
             rendered_dom.context.update(dom.context)
             dom = rendered_dom
             classes += dom.classes
 
         element_tag = f"{dom.html_header}\n" if dom.html_header else ""
         children_str = dom._format_children() if dom.children else ""
```

### Comparing `ludic-0.4.8/ludic/components.py` & `ludic-0.4.9/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/format.py` & `ludic-0.4.9/ludic/format.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import html
 import random
 import re
+from collections.abc import Mapping
 from contextvars import ContextVar
 from typing import Annotated, Any, Final, TypeVar, get_args, get_origin
 
 from .utils import get_element_attrs_annotations
 
 EXTRACT_NUMBER_RE: Final[re.Pattern[str]] = re.compile(r"\{(\d+:id)\}")
 
@@ -16,33 +17,45 @@
 
     Args:
         key (str): The key of the attribute.
         value (Any): The value of the attribute, can be a string or a dictionary.
     Returns:
         str: The formatted HTML attribute.
     """
+
+    def _html_escape(value: Any) -> str:
+        if (
+            is_html
+            and value
+            and isinstance(value, str)
+            and getattr(value, "escape", True)
+        ):
+            return html.escape(value, False)  # type: ignore
+        return str(value)
+
     if isinstance(value, dict):
-        value = ";".join(
-            f"{dict_key}:{html.escape(dict_value, False)}"
+        formatted_value = ";".join(
+            f"{dict_key}:{_html_escape(dict_value)}"
             for dict_key, dict_value in value.items()
         )
     elif isinstance(value, list):
-        value = " ".join(html.escape(v, False) for v in value)
+        formatted_value = " ".join(map(_html_escape, value))
     elif isinstance(value, bool):
         if is_html and not key.startswith("hx"):
-            value = html.escape(key, False) if value else ""
+            formatted_value = html.escape(key, False) if value else ""
         else:
-            value = "true" if value else "false"
-    elif isinstance(value, str) and getattr(value, "escape", True):
-        value = html.escape(value, False)
-    return str(value)
+            formatted_value = "true" if value else "false"
+    else:
+        formatted_value = _html_escape(value)
+
+    return formatted_value
 
 
 def format_attrs(
-    attrs_type: Any, attrs: dict[str, Any], is_html: bool = False
+    attrs_type: Any, attrs: Mapping[str, Any], is_html: bool = False
 ) -> dict[str, Any]:
     """Format the given attributes according to the element's attributes.
 
     Here is an example of TypedDict definition:
 
         class PersonAttrs(TypedDict):
             name: str
```

### Comparing `ludic-0.4.8/ludic/html.py` & `ludic-0.4.9/ludic/html.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/types.py` & `ludic-0.4.9/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/utils.py` & `ludic-0.4.9/ludic/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,59 @@
+from collections.abc import Hashable
 from functools import lru_cache
 from typing import (
     Annotated,
     Any,
     TypeVar,
     get_args,
     get_origin,
     get_type_hints,
 )
 
 _T = TypeVar("_T", covariant=True)
 
 
-def get_element_generic_args(cls_or_obj: Any) -> tuple[type, ...] | None:
+@lru_cache
+def get_element_generic_args(obj_or_type: Hashable) -> tuple[type, ...] | None:
     """Get the generic arguments of the element class.
 
     Args:
-        cls_or_obj (Any): The element to get the generic arguments of.
+        obj_or_type (Any): The element to get the generic arguments of.
 
     Returns:
         dict[str, Any] | None: The generic arguments or :obj:`None`.
     """
     from ludic.base import BaseElement
 
-    if hints := getattr(cls_or_obj, "__annotations__", None):
+    if hints := getattr(obj_or_type, "__annotations__", None):
         children = hints.get("children")
         attrs = hints.get("attrs")
         if attrs and children:
             return (children, attrs)
 
-    for base in getattr(cls_or_obj, "__orig_bases__", []):
+    for base in getattr(obj_or_type, "__orig_bases__", []):
         if issubclass(get_origin(base), BaseElement):
             return get_args(base)
     return None
 
 
 @lru_cache
 def get_element_attrs_annotations(
-    cls_or_obj: Any, include_extras: bool = False
+    obj_or_type: Hashable, include_extras: bool = False
 ) -> dict[str, Any]:
     """Get the annotations of the element.
 
     Args:
-        cls_or_obj (type[Any]): The element to get the annotations of.
+        obj_or_type (Hashable): The element to get the annotations of.
         include_extras (bool): Whether to include extra annotation info.
 
     Returns:
         dict[str, Any]: The attributes' annotations of the element.
     """
-    if (args := get_element_generic_args(cls_or_obj)) is not None:
+    if (args := get_element_generic_args(obj_or_type)) is not None:
         return get_type_hints(args[-1], include_extras=include_extras)
     return {}
 
 
 def get_annotations_metadata_of_type(
     annotations: dict[str, Any],
     expected_type: type[_T],
```

### Comparing `ludic-0.4.8/ludic/catalog/buttons.py` & `ludic-0.4.9/ludic/catalog/buttons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/forms.py` & `ludic-0.4.9/ludic/catalog/forms.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/headers.py` & `ludic-0.4.9/ludic/catalog/headers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/icons.py` & `ludic-0.4.9/ludic/catalog/icons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/items.py` & `ludic-0.4.9/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/layouts.py` & `ludic-0.4.9/ludic/catalog/layouts.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/lists.py` & `ludic-0.4.9/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/loaders.py` & `ludic-0.4.9/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/messages.py` & `ludic-0.4.9/ludic/catalog/messages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/navigation.py` & `ludic-0.4.9/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/pages.py` & `ludic-0.4.9/ludic/catalog/pages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/quotes.py` & `ludic-0.4.9/ludic/catalog/quotes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/tables.py` & `ludic-0.4.9/ludic/catalog/tables.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/typography.py` & `ludic-0.4.9/ludic/catalog/typography.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/catalog/utils.py` & `ludic-0.4.9/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/styles/collect.py` & `ludic-0.4.9/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/styles/themes.py` & `ludic-0.4.9/ludic/styles/themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/styles/types.py` & `ludic-0.4.9/ludic/styles/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/styles/utils.py` & `ludic-0.4.9/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/app.py` & `ludic-0.4.9/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/datastructures.py` & `ludic-0.4.9/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/endpoints.py` & `ludic-0.4.9/ludic/web/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             raise RuntimeError(
                 f"{type(self).__name__} is not bound to a request, you can only use "
                 f"the {type(self).__name__}.url_for method in the context of a request."
             )
 
         if inspect.isclass(endpoint) and issubclass(endpoint, Endpoint):
             endpoint_generic_args = get_element_generic_args(endpoint)
-            self_generic_args = get_element_generic_args(self)
+            self_generic_args = get_element_generic_args(type(self))
 
             if (
                 endpoint_generic_args
                 and self_generic_args
                 and endpoint_generic_args[-1] is self_generic_args[-1]
             ):
                 path_params = {
```

### Comparing `ludic-0.4.8/ludic/web/exceptions.py` & `ludic-0.4.9/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/parsers.py` & `ludic-0.4.9/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/requests.py` & `ludic-0.4.9/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/responses.py` & `ludic-0.4.9/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/ludic/web/routing.py` & `ludic-0.4.9/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/test_components.py` & `ludic-0.4.9/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/test_elements.py` & `ludic-0.4.9/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/test_examples.py` & `ludic-0.4.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/test_exceptions.py` & `ludic-0.4.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/test_formatting.py` & `ludic-0.4.9/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/test_types.py` & `ludic-0.4.9/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/styles/__init__.py` & `ludic-0.4.9/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/styles/test_styles.py` & `ludic-0.4.9/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/tests/styles/test_themes.py` & `ludic-0.4.9/tests/styles/test_themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/.gitignore` & `ludic-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/LICENCE` & `ludic-0.4.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/README.md` & `ludic-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/pyproject.toml` & `ludic-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.8/PKG-INFO` & `ludic-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.8
+Version: 0.4.9
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

