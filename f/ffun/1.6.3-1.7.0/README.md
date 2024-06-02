# Comparing `tmp/ffun-1.6.3.tar.gz` & `tmp/ffun-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-1.6.3.tar", max compression
+gzip compressed data, was "ffun-1.7.0.tar", max compression
```

## Comparing `ffun-1.6.3.tar` & `ffun-1.7.0.tar`

### file list

```diff
@@ -1,235 +1,235 @@
--rw-r--r--   0        0        0      344 2024-05-29 16:39:30.173809 ffun-1.6.3/README.md
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/api/__init__.py
--rw-r--r--   0        0        0    10256 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/api/entities.py
--rw-r--r--   0        0        0    13637 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/api/http_handlers.py
--rw-r--r--   0        0        0      245 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/api/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/__init__.py
--rw-r--r--   0        0        0     4314 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/application.py
--rw-r--r--   0        0        0      115 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/errors.py
--rw-r--r--   0        0        0       68 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/resources.py
--rw-r--r--   0        0        0     1635 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/tests/__init__.py
--rw-r--r--   0        0        0      422 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/tests/test_settings.py
--rw-r--r--   0        0        0     3724 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/user_settings.py
--rw-r--r--   0        0        0      281 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/utils.py
--rw-r--r--   0        0        0     1252 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/auth/__init__.py
--rw-r--r--   0        0        0      984 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      828 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/auth/settings.py
--rw-r--r--   0        0        0     2800 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/__init__.py
--rw-r--r--   0        0        0      174 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/application.py
--rw-r--r--   0        0        0      439 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      732 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0     1050 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/entries.py
--rw-r--r--   0        0        0     1393 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/failed_entries.py
--rw-r--r--   0        0        0      538 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/meta.py
--rw-r--r--   0        0        0     1001 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      884 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      209 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0     1333 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/conftest.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/__init__.py
--rw-r--r--   0        0        0      631 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/api.py
--rw-r--r--   0        0        0     3139 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      493 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/entities.py
--rw-r--r--   0        0        0      552 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/errors.py
--rw-r--r--   0        0        0     2773 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/json.py
--rw-r--r--   0        0        0     5440 2024-05-29 16:39:30.173809 ffun-1.6.3/ffun/core/logging.py
--rw-r--r--   0        0        0     1516 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/middlewares.py
--rw-r--r--   0        0        0      882 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/migrations.py
--rw-r--r--   0        0        0     4019 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/postgresql.py
--rw-r--r--   0        0        0      695 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/register.py
--rw-r--r--   0        0        0     1442 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/sentry.py
--rw-r--r--   0        0        0      347 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/tests/__init__.py
--rw-r--r--   0        0        0     5031 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/tests/helpers.py
--rw-r--r--   0        0        0       82 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/tests/make.py
--rw-r--r--   0        0        0      486 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/text.py
--rw-r--r--   0        0        0     1088 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/domain/tests/__init__.py
--rw-r--r--   0        0        0     6690 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/domain/tests/test_urls.py
--rw-r--r--   0        0        0     4096 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/domain/urls.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      826 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1937 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/entities.py
--rw-r--r--   0        0        0      131 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/errors.py
--rw-r--r--   0        0        0     1027 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      641 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0      561 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
--rw-r--r--   0        0        0      531 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
--rw-r--r--   0        0        0      725 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
--rw-r--r--   0        0        0     4062 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/tests/fixtures.py
--rw-r--r--   0        0        0     1178 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/tests/make.py
--rw-r--r--   0        0        0      445 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/tests/test_domain.py
--rw-r--r--   0        0        0     7782 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      777 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      128 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      573 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/tests/__init__.py
--rw-r--r--   0        0        0      684 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_collections/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3974 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      553 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      810 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     2326 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/tests/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/feeds_links/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     3759 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/domain.py
--rw-r--r--   0        0        0      205 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/entities.py
--rw-r--r--   0        0        0      217 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/errors.py
--rw-r--r--   0        0        0     2101 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
--rw-r--r--   0        0        0     3035 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
--rw-r--r--   0        0        0     5112 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0     1255 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1548 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      468 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3295 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4421 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/tests/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/tests/test_upper_case_title.py
--rw-r--r--   0        0        0      434 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/processors/upper_case_title.py
--rw-r--r--   0        0        0     1089 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/__init__.py
--rw-r--r--   0        0        0      845 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/fixtures.py
--rw-r--r--   0        0        0      487 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/helpers.py
--rw-r--r--   0        0        0      553 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/make.py
--rw-r--r--   0        0        0     4104 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/test_background_processors.py
--rw-r--r--   0        0        0    13605 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/test_domain.py
--rw-r--r--   0        0        0    14031 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/librarian/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/__init__.py
--rw-r--r--   0        0        0     1509 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/domain.py
--rw-r--r--   0        0        0     1168 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/entities.py
--rw-r--r--   0        0        0      149 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/errors.py
--rw-r--r--   0        0        0     1498 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1288 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      710 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     1125 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
--rw-r--r--   0        0        0     1003 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
--rw-r--r--   0        0        0     1194 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
--rw-r--r--   0        0        0      784 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
--rw-r--r--   0        0        0     5926 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/tests/__init__.py
--rw-r--r--   0        0        0      799 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/tests/fixtures.py
--rw-r--r--   0        0        0     1663 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/tests/make.py
--rw-r--r--   0        0        0     1414 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/tests/test_domain.py
--rw-r--r--   0        0        0    15331 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/library/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/loader/__init__.py
--rw-r--r--   0        0        0     1218 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/loader/background_loader.py
--rw-r--r--   0        0        0     5498 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/loader/domain.py
--rw-r--r--   0        0        0       82 2024-05-29 16:39:30.177809 ffun-1.6.3/ffun/loader/entities.py
--rw-r--r--   0        0        0      226 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/errors.py
--rw-r--r--   0        0        0      738 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py
--rw-r--r--   0        0        0     9639 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/operations.py
--rw-r--r--   0        0        0      647 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/tests/__init__.py
--rw-r--r--   0        0        0     9569 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/tests/test_domain.py
--rw-r--r--   0        0        0     6941 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/loader/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/__init__.py
--rw-r--r--   0        0        0      504 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/entities.py
--rw-r--r--   0        0        0      855 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     2447 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/tests/__init__.py
--rw-r--r--   0        0        0     4835 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/markers/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/meta/__init__.py
--rw-r--r--   0        0        0     3557 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/meta/domain.py
--rw-r--r--   0        0        0      345 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
--rw-r--r--   0        0        0      246 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/meta/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/meta/tests/__init__.py
--rw-r--r--   0        0        0    15939 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/meta/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1092 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      520 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      799 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1008 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     6307 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/tests/__init__.py
--rw-r--r--   0        0        0      834 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/tests/fixtures.py
--rw-r--r--   0        0        0      408 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/tests/helpers.py
--rw-r--r--   0        0        0     9964 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/ontology/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/__init__.py
--rw-r--r--   0        0        0     5962 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/client.py
--rw-r--r--   0        0        0      612 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/entities.py
--rw-r--r--   0        0        0      150 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/errors.py
--rw-r--r--   0        0        0     7597 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0     1919 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/keys_statuses.py
--rw-r--r--   0        0        0      372 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/settings.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/tests/__init__.py
--rw-r--r--   0        0        0      130 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/tests/conftest.py
--rw-r--r--   0        0        0     2518 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/tests/fixtures.py
--rw-r--r--   0        0        0    19734 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/tests/test_keys_rotator.py
--rw-r--r--   0        0        0     2833 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/openai/tests/test_keys_statuses.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      228 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/domain.py
--rw-r--r--   0        0        0      567 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/entities.py
--rw-r--r--   0        0        0     2362 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
--rw-r--r--   0        0        0      639 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
--rw-r--r--   0        0        0     4745 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
--rw-r--r--   0        0        0     1072 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
--rw-r--r--   0        0        0      966 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/make.py
--rw-r--r--   0        0        0     1205 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/parsers/tests/test_feed.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/__init__.py
--rw-r--r--   0        0        0      769 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/domain.py
--rw-r--r--   0        0        0      280 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/entities.py
--rw-r--r--   0        0        0      120 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/errors.py
--rw-r--r--   0        0        0      865 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3984 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/tests/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/tests/test_domain.py
--rw-r--r--   0        0        0     9480 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/resources/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/__init__.py
--rw-r--r--   0        0        0      884 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/domain.py
--rw-r--r--   0        0        0      250 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/entities.py
--rw-r--r--   0        0        0      104 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/errors.py
--rw-r--r--   0        0        0      851 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0      603 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
--rw-r--r--   0        0        0     2603 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/tests/__init__.py
--rw-r--r--   0        0        0     1239 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/tests/test_domain.py
--rw-r--r--   0        0        0     6810 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/scores/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/tags/tests/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/tags/tests/test_converters.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       54 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      137 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/errors.py
--rw-r--r--   0        0        0      732 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0      534 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
--rw-r--r--   0        0        0     1748 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      581 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/settings.py
--rw-r--r--   0        0        0      508 2024-05-29 16:39:30.181810 ffun-1.6.3/ffun/user_settings/tests/asserts.py
--rw-r--r--   0        0        0     6956 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/user_settings/tests/test_domain.py
--rw-r--r--   0        0        0     5492 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/user_settings/tests/test_operations.py
--rw-r--r--   0        0        0     2297 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/user_settings/types.py
--rw-r--r--   0        0        0      489 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/__init__.py
--rw-r--r--   0        0        0      586 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/entities.py
--rw-r--r--   0        0        0      111 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/errors.py
--rw-r--r--   0        0        0      718 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1232 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/operations.py
--rw-r--r--   0        0        0        0 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/tests/fixtures.py
--rw-r--r--   0        0        0      348 2024-05-29 16:39:30.185809 ffun-1.6.3/ffun/users/tests/make.py
--rw-r--r--   0        0        0     4326 2024-05-29 16:39:37.965896 ffun-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 ffun-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0      344 2024-06-02 16:12:24.900883 ffun-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/api/__init__.py
+-rw-r--r--   0        0        0    10256 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/api/entities.py
+-rw-r--r--   0        0        0    13637 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0      245 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/api/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4314 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/errors.py
+-rw-r--r--   0        0        0       68 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/resources.py
+-rw-r--r--   0        0        0     1635 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/tests/__init__.py
+-rw-r--r--   0        0        0      422 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/tests/test_settings.py
+-rw-r--r--   0        0        0     3724 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      281 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/utils.py
+-rw-r--r--   0        0        0     1252 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/auth/__init__.py
+-rw-r--r--   0        0        0      984 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      828 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2800 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      174 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/application.py
+-rw-r--r--   0        0        0      439 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      732 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0     1050 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/entries.py
+-rw-r--r--   0        0        0     1393 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/failed_entries.py
+-rw-r--r--   0        0        0      538 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/meta.py
+-rw-r--r--   0        0        0     1001 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      884 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      209 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0     1018 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/conftest.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.900883 ffun-1.7.0/ffun/core/__init__.py
+-rw-r--r--   0        0        0      631 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/api.py
+-rw-r--r--   0        0        0     3139 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      493 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/entities.py
+-rw-r--r--   0        0        0      551 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/errors.py
+-rw-r--r--   0        0        0     2773 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/json.py
+-rw-r--r--   0        0        0     5440 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/logging.py
+-rw-r--r--   0        0        0     1516 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/middlewares.py
+-rw-r--r--   0        0        0      882 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/migrations.py
+-rw-r--r--   0        0        0     4019 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      695 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/register.py
+-rw-r--r--   0        0        0     1471 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/tests/__init__.py
+-rw-r--r--   0        0        0     5031 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/tests/helpers.py
+-rw-r--r--   0        0        0       82 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/tests/make.py
+-rw-r--r--   0        0        0      486 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/text.py
+-rw-r--r--   0        0        0     1088 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/domain/tests/__init__.py
+-rw-r--r--   0        0        0     6690 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/domain/tests/test_urls.py
+-rw-r--r--   0        0        0     4096 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      826 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1937 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/entities.py
+-rw-r--r--   0        0        0      131 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/errors.py
+-rw-r--r--   0        0        0     1027 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      642 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0      561 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
+-rw-r--r--   0        0        0      531 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
+-rw-r--r--   0        0        0      725 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
+-rw-r--r--   0        0        0     4062 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/tests/fixtures.py
+-rw-r--r--   0        0        0     1178 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/tests/make.py
+-rw-r--r--   0        0        0      445 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/tests/test_domain.py
+-rw-r--r--   0        0        0     7782 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      777 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      128 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      573 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/tests/__init__.py
+-rw-r--r--   0        0        0      684 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_collections/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3974 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      553 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      811 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     2326 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/feeds_links/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     5182 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     3850 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      205 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/entities.py
+-rw-r--r--   0        0        0      217 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     2101 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
+-rw-r--r--   0        0        0     3036 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
+-rw-r--r--   0        0        0     5112 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0     1255 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1548 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      468 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3295 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4421 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/tests/test_upper_case_title.py
+-rw-r--r--   0        0        0      434 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/processors/upper_case_title.py
+-rw-r--r--   0        0        0     1089 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/__init__.py
+-rw-r--r--   0        0        0      845 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/fixtures.py
+-rw-r--r--   0        0        0      487 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/helpers.py
+-rw-r--r--   0        0        0      553 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/make.py
+-rw-r--r--   0        0        0     4104 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/test_background_processors.py
+-rw-r--r--   0        0        0    13605 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/test_domain.py
+-rw-r--r--   0        0        0    14031 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/librarian/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/__init__.py
+-rw-r--r--   0        0        0     1509 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/domain.py
+-rw-r--r--   0        0        0     1168 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/entities.py
+-rw-r--r--   0        0        0      149 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/errors.py
+-rw-r--r--   0        0        0     1499 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1289 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      711 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     1125 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
+-rw-r--r--   0        0        0     1003 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
+-rw-r--r--   0        0        0     1195 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
+-rw-r--r--   0        0        0      784 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
+-rw-r--r--   0        0        0     5926 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/tests/__init__.py
+-rw-r--r--   0        0        0      799 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/tests/fixtures.py
+-rw-r--r--   0        0        0     1663 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/tests/make.py
+-rw-r--r--   0        0        0     1414 2024-06-02 16:12:24.904883 ffun-1.7.0/ffun/library/tests/test_domain.py
+-rw-r--r--   0        0        0    15331 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/library/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/__init__.py
+-rw-r--r--   0        0        0     1218 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0     5498 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/domain.py
+-rw-r--r--   0        0        0       82 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/entities.py
+-rw-r--r--   0        0        0      226 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/errors.py
+-rw-r--r--   0        0        0      738 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py
+-rw-r--r--   0        0        0     9639 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/operations.py
+-rw-r--r--   0        0        0      647 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/tests/__init__.py
+-rw-r--r--   0        0        0     9569 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/tests/test_domain.py
+-rw-r--r--   0        0        0     6941 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/loader/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      504 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/entities.py
+-rw-r--r--   0        0        0      856 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     2447 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/markers/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/meta/__init__.py
+-rw-r--r--   0        0        0     3557 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/meta/domain.py
+-rw-r--r--   0        0        0      346 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
+-rw-r--r--   0        0        0      246 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/meta/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/meta/tests/__init__.py
+-rw-r--r--   0        0        0    15939 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/meta/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3840 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1092 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      521 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      800 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1009 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     6307 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/tests/__init__.py
+-rw-r--r--   0        0        0      834 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/tests/fixtures.py
+-rw-r--r--   0        0        0      408 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/tests/helpers.py
+-rw-r--r--   0        0        0     9964 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/ontology/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     6120 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/client.py
+-rw-r--r--   0        0        0      612 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/entities.py
+-rw-r--r--   0        0        0      150 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7597 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0     1803 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/keys_statuses.py
+-rw-r--r--   0        0        0      372 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/tests/__init__.py
+-rw-r--r--   0        0        0      130 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2518 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/tests/fixtures.py
+-rw-r--r--   0        0        0    19734 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/tests/test_keys_rotator.py
+-rw-r--r--   0        0        0     2970 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/openai/tests/test_keys_statuses.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      228 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      567 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     2362 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/__init__.py
+-rw-r--r--   0        0        0     1219 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
+-rw-r--r--   0        0        0      639 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
+-rw-r--r--   0        0        0     4745 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
+-rw-r--r--   0        0        0     1072 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
+-rw-r--r--   0        0        0      974 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/make.py
+-rw-r--r--   0        0        0     1205 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/parsers/tests/test_feed.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      769 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/domain.py
+-rw-r--r--   0        0        0      280 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/entities.py
+-rw-r--r--   0        0        0      120 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/errors.py
+-rw-r--r--   0        0        0      866 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3984 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/tests/test_domain.py
+-rw-r--r--   0        0        0     9480 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/resources/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      884 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/domain.py
+-rw-r--r--   0        0        0      250 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/entities.py
+-rw-r--r--   0        0        0      104 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/errors.py
+-rw-r--r--   0        0        0      852 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0      603 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
+-rw-r--r--   0        0        0     2603 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/tests/__init__.py
+-rw-r--r--   0        0        0     1251 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/tests/test_domain.py
+-rw-r--r--   0        0        0     6810 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/scores/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1578 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/tags/tests/__init__.py
+-rw-r--r--   0        0        0     1352 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/tags/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1842 2024-06-02 16:12:24.908883 ffun-1.7.0/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       54 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      137 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/errors.py
+-rw-r--r--   0        0        0      733 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0      535 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
+-rw-r--r--   0        0        0     1748 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      581 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0      508 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/tests/asserts.py
+-rw-r--r--   0        0        0     6956 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/tests/test_domain.py
+-rw-r--r--   0        0        0     5492 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/tests/test_operations.py
+-rw-r--r--   0        0        0     2297 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      489 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/__init__.py
+-rw-r--r--   0        0        0      586 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/entities.py
+-rw-r--r--   0        0        0      111 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/errors.py
+-rw-r--r--   0        0        0      719 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1232 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/operations.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/tests/fixtures.py
+-rw-r--r--   0        0        0      348 2024-06-02 16:12:24.912883 ffun-1.7.0/ffun/users/tests/make.py
+-rw-r--r--   0        0        0     4715 2024-06-02 16:12:33.192890 ffun-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 ffun-1.7.0/PKG-INFO
```

### Comparing `ffun-1.6.3/ffun/api/entities.py` & `ffun-1.7.0/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/api/http_handlers.py` & `ffun-1.7.0/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/application/application.py` & `ffun-1.7.0/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/application/settings.py` & `ffun-1.7.0/ffun/application/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/application/user_settings.py` & `ffun-1.7.0/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/application/workers.py` & `ffun-1.7.0/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/auth/dependencies.py` & `ffun-1.7.0/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/auth/settings.py` & `ffun-1.7.0/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/auth/supertokens.py` & `ffun-1.7.0/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/cli/commands/configs.py` & `ffun-1.7.0/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/cli/commands/entries.py` & `ffun-1.7.0/ffun/cli/commands/entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/cli/commands/failed_entries.py` & `ffun-1.7.0/ffun/cli/commands/failed_entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/cli/commands/meta.py` & `ffun-1.7.0/ffun/cli/commands/meta.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/cli/commands/supertokens.py` & `ffun-1.7.0/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/cli/commands/workers.py` & `ffun-1.7.0/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/conftest.py` & `ffun-1.7.0/ffun/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-import asyncio
-from typing import AsyncGenerator, Generator
+from typing import AsyncGenerator
 
 import fastapi
-import pytest
 import pytest_asyncio
 
 from ffun.application import application
 from ffun.core import migrations
 from ffun.feeds.tests.fixtures import *  # noqa
 from ffun.feeds_collections.tests.fixtures import *  # noqa
 from ffun.librarian.tests.fixtures import *  # noqa
 from ffun.library.tests.fixtures import *  # noqa
 from ffun.ontology.tests.fixtures import *  # noqa
 from ffun.openai.tests.fixtures import *  # noqa
 from ffun.users.tests.fixtures import *  # noqa
 
 
-@pytest.fixture(scope="session", autouse=True)
-def event_loop() -> Generator[asyncio.AbstractEventLoop, asyncio.AbstractEventLoop, None]:
-    loop = asyncio.get_event_loop_policy().new_event_loop()
-    yield loop
-    loop.close()
-
-
 @pytest_asyncio.fixture(scope="session", autouse=True)
 async def app() -> AsyncGenerator[fastapi.FastAPI, None]:
     async with application.with_app() as app:
         yield app
 
 
 @pytest_asyncio.fixture(scope="session", autouse=True)
 async def prepare_db(
     app: AsyncGenerator[fastapi.FastAPI, None],
-    event_loop: asyncio.AbstractEventLoop,
 ) -> AsyncGenerator[None, None]:
     # database migrations may be in an inconsistent state
     await migrations.rollback_all()
 
     await migrations.apply_all()
     yield
     await migrations.rollback_all()
```

### Comparing `ffun-1.6.3/ffun/core/api.py` & `ffun-1.7.0/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/background_tasks.py` & `ffun-1.7.0/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/errors.py` & `ffun-1.7.0/ffun/core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         for key, value in kwargs.items():
             setattr(self, key, value)
 
         # TODO: send to Sentry
         if "fingerprint" not in kwargs:
             self.fingerprint = None
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         attributes = ", ".join(f"{key}={value}" for key, value in self.__dict__.items())
 
         return f"{self.__class__.__name__}: {attributes}"
 
 
 class CoreError(Error):
     pass
```

### Comparing `ffun-1.6.3/ffun/core/json.py` & `ffun-1.7.0/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/logging.py` & `ffun-1.7.0/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/middlewares.py` & `ffun-1.7.0/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/migrations.py` & `ffun-1.7.0/ffun/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/postgresql.py` & `ffun-1.7.0/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/register.py` & `ffun-1.7.0/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/sentry.py` & `ffun-1.7.0/ffun/core/sentry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from sentry_sdk import init as initialize_sentry
+
+if TYPE_CHECKING:
+    from sentry_sdk._types import Event
+
 from sentry_sdk.integrations.fastapi import FastApiIntegration
 from sentry_sdk.integrations.logging import LoggingIntegration
 from sentry_sdk.integrations.starlette import StarletteIntegration
 
 from ffun.core.errors import Error
 
 
-def improve_fingerprint(event: dict[str, Any], hint: dict[str, Any]) -> dict[str, Any]:
+def improve_fingerprint(event: "Event", hint: dict[str, Any]) -> "Event":
     if "exc_info" not in hint:
         return event
 
     _, e, _ = hint["exc_info"]
 
     if isinstance(e, Error) and e.fingerprint is not None:
         event["fingerprint"] = ["{{ default }}", e.fingerprint]
 
     return event
 
 
-def before_send(event: dict[str, Any], hint: dict[str, Any]) -> dict[str, Any]:
-    event = improve_fingerprint(event, hint)
-    return event
+def before_send(event: "Event", hint: dict[str, Any]) -> "Event":
+    return improve_fingerprint(event, hint)
 
 
 def initialize(dsn: str, sample_rate: float, traces_sample_rate: float, environment: str) -> None:
     initialize_sentry(
         dsn=dsn,
         sample_rate=sample_rate,
         traces_sample_rate=traces_sample_rate,
```

### Comparing `ffun-1.6.3/ffun/core/tests/helpers.py` & `ffun-1.7.0/ffun/core/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/core/utils.py` & `ffun-1.7.0/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/domain/tests/test_urls.py` & `ffun-1.7.0/ffun/domain/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/domain/urls.py` & `ffun-1.7.0/ffun/domain/urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/domain.py` & `ffun-1.7.0/ffun/feeds/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/entities.py` & `ffun-1.7.0/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-1.7.0/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-1.7.0/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 add-title-and-description
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230329_01_ilwfq-feeds-table"}
```

### Comparing `ffun-1.6.3/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py` & `ffun-1.7.0/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py` & `ffun-1.7.0/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py` & `ffun-1.7.0/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/operations.py` & `ffun-1.7.0/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/tests/fixtures.py` & `ffun-1.7.0/ffun/feeds/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/tests/make.py` & `ffun-1.7.0/ffun/feeds/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds/tests/test_operations.py` & `ffun-1.7.0/ffun/feeds/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_collections/collections/gamedev.py` & `ffun-1.7.0/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_collections/domain.py` & `ffun-1.7.0/ffun/feeds_collections/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_collections/predefines.py` & `ffun-1.7.0/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_collections/tests/fixtures.py` & `ffun-1.7.0/ffun/feeds_collections/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_discoverer/domain.py` & `ffun-1.7.0/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_links/domain.py` & `ffun-1.7.0/ffun/feeds_links/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-1.7.0/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 add-feeds-links
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/feeds_links/operations.py` & `ffun-1.7.0/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/feeds_links/tests/test_operations.py` & `ffun-1.7.0/ffun/feeds_links/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/background_processors.py` & `ffun-1.7.0/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/domain.py` & `ffun-1.7.0/ffun/librarian/domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         await o_domain.apply_tags_to_entry(entry.id, processor_id, tags)
 
         logger.info("processor_successed")
     except errors.SkipEntryProcessing as e:
         # do nothing in such case, see: https://github.com/Tiendil/feeds.fun/issues/176
         logger.warning("processor_requested_to_skip_entry", error_info=str(e))
     except Exception as e:
+        logger.exception("processor_failed", entry_id=entry.id, processor_id=processor_id)
         await operations.add_entries_to_failed_storage(processor_id, [entry.id])
         raise errors.UnexpectedErrorInProcessor(processor_id=processor_id, entry_id=entry.id) from e
     finally:
         await operations.remove_entries_from_processor_queue(execute, processor_id, [entry.id])
 
     logger.info("entry_processed")
```

### Comparing `ffun-1.6.3/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py` & `ffun-1.7.0/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py` & `ffun-1.7.0/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 migrate_to_processors_queue
 """
+
 import uuid
 from typing import Any
 
 from psycopg import Connection
 from psycopg.rows import dict_row
 from pypika import PostgreSQLQuery
 from yoyo import step
```

### Comparing `ffun-1.6.3/ffun/librarian/operations.py` & `ffun-1.7.0/ffun/librarian/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/processors/base.py` & `ffun-1.7.0/ffun/librarian/processors/base.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/processors/domain.py` & `ffun-1.7.0/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-1.7.0/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-1.7.0/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/processors/tests/test_upper_case_title.py` & `ffun-1.7.0/ffun/librarian/processors/tests/test_upper_case_title.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/settings.py` & `ffun-1.7.0/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/tests/fixtures.py` & `ffun-1.7.0/ffun/librarian/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/tests/make.py` & `ffun-1.7.0/ffun/librarian/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/tests/test_background_processors.py` & `ffun-1.7.0/ffun/librarian/tests/test_background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/tests/test_domain.py` & `ffun-1.7.0/ffun/librarian/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/librarian/tests/test_operations.py` & `ffun-1.7.0/ffun/librarian/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/domain.py` & `ffun-1.7.0/ffun/library/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/entities.py` & `ffun-1.7.0/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-1.7.0/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 entries_table
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-1.7.0/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 fix-entries-unique-index
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230331_01_UsHwp-entries-table"}
```

### Comparing `ffun-1.6.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-1.7.0/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 processed-state
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230427_01_pv33u-fix-entries-unique-index"}
```

### Comparing `ffun-1.6.3/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py` & `ffun-1.7.0/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py` & `ffun-1.7.0/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py` & `ffun-1.7.0/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 remove-duplicated-entries-from-feeds
 """
+
 from typing import Any
 
 from psycopg import Connection
 from psycopg.rows import dict_row
 from yoyo import step
 
 __depends__ = {"20240503_01_Bmzw6-remove-l-entry-process-info"}
```

### Comparing `ffun-1.6.3/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py` & `ffun-1.7.0/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/operations.py` & `ffun-1.7.0/ffun/library/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/tests/fixtures.py` & `ffun-1.7.0/ffun/library/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/tests/make.py` & `ffun-1.7.0/ffun/library/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/tests/test_domain.py` & `ffun-1.7.0/ffun/library/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/library/tests/test_operations.py` & `ffun-1.7.0/ffun/library/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/background_loader.py` & `ffun-1.7.0/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/domain.py` & `ffun-1.7.0/ffun/loader/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py` & `ffun-1.7.0/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/operations.py` & `ffun-1.7.0/ffun/loader/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/settings.py` & `ffun-1.7.0/ffun/loader/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/tests/test_domain.py` & `ffun-1.7.0/ffun/loader/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/loader/tests/test_operations.py` & `ffun-1.7.0/ffun/loader/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-1.7.0/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 markers-tables
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/markers/operations.py` & `ffun-1.7.0/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/markers/tests/test_operations.py` & `ffun-1.7.0/ffun/markers/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/meta/domain.py` & `ffun-1.7.0/ffun/meta/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/meta/tests/test_domain.py` & `ffun-1.7.0/ffun/meta/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/ontology/domain.py` & `ffun-1.7.0/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/ontology/entities.py` & `ffun-1.7.0/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-1.7.0/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-1.7.0/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 rename-tags-names-to-uid
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230404_01_ZUBsm-ontology-tables"}
```

### Comparing `ffun-1.6.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-1.7.0/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 tags-relationship-processor-tracking
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230617_01_XDdNG-rename-tags-names-to-uid"}
```

### Comparing `ffun-1.6.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-1.7.0/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 tags-properties
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230617_02_L0MmA-tags-relationship-processor-tracking"}
```

### Comparing `ffun-1.6.3/ffun/ontology/operations.py` & `ffun-1.7.0/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/ontology/tests/fixtures.py` & `ffun-1.7.0/ffun/ontology/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/ontology/tests/test_operations.py` & `ffun-1.7.0/ffun/ontology/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/openai/client.py` & `ffun-1.7.0/ffun/openai/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import math
 from typing import Any
 
 import async_lru
 import openai
 import tiktoken
 import typer
+from openai import AsyncOpenAI
 
 from ffun.core import logging
 from ffun.openai import entities, errors
 from ffun.openai.keys_statuses import statuses, track_key_status
 
 logger = logging.get_module_logger()
 
@@ -114,41 +115,44 @@
 
     if function is not None:
         arguments["functions"] = [function]
         arguments["function_call"] = {"name": function["name"]}
 
     with track_key_status(api_key):
         try:
-            answer = await openai.ChatCompletion.acreate(
-                api_key=api_key,
+            answer = await AsyncOpenAI(api_key=api_key).chat.completions.create(
                 model=model,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 presence_penalty=presence_penalty,
                 frequency_penalty=frequency_penalty,
-                messages=messages,
+                messages=messages,  # type: ignore
                 **arguments
             )
-        except openai.error.APIError as e:
+        except openai.APIError as e:
             logger.info("openai_api_error", message=str(e))
             raise errors.TemporaryError(message=str(e)) from e
 
     logger.info("openai_response")
 
     if function:
-        content = answer["choices"][0]["message"]["function_call"]["arguments"]
+        assert answer.choices[0].message.function_call is not None
+        content = answer.choices[0].message.function_call.arguments
     else:
-        content = answer["choices"][0]["message"]["content"]
+        assert answer.choices[0].message.content is not None
+        content = answer.choices[0].message.content
+
+    assert answer.usage is not None
 
     return entities.OpenAIAnswer(
         content=content,
-        prompt_tokens=answer["usage"]["prompt_tokens"],
-        completion_tokens=answer["usage"]["completion_tokens"],
-        total_tokens=answer["usage"]["total_tokens"],
+        prompt_tokens=answer.usage.prompt_tokens,
+        completion_tokens=answer.usage.completion_tokens,
+        total_tokens=answer.usage.total_tokens,
     )
 
 
 async def multiple_requests(  # noqa: CFQ002
     api_key: str,
     model: str,
     messages: list[list[dict[str, str]]],
@@ -181,12 +185,12 @@
 
     return results
 
 
 async def check_api_key(api_key: str) -> entities.KeyStatus:
     with track_key_status(api_key):
         try:
-            await openai.Model.alist(api_key=api_key)
-        except openai.error.APIError:
+            await AsyncOpenAI(api_key=api_key).models.list()
+        except openai.APIError:
             pass
 
     return statuses.get(api_key)
```

### Comparing `ffun-1.6.3/ffun/openai/entities.py` & `ffun-1.7.0/ffun/openai/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/openai/keys_rotator.py` & `ffun-1.7.0/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/openai/keys_statuses.py` & `ffun-1.7.0/ffun/openai/keys_statuses.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,23 +48,20 @@
 
 
 @contextlib.contextmanager
 def track_key_status(key: str, statuses: Statuses = statuses) -> Generator[None, None, None]:
     try:
         yield
         statuses.set(key, KeyStatus.works)
-    except openai.error.AuthenticationError:
+    except openai.AuthenticationError:
         statuses.set(key, KeyStatus.broken)
         raise
-    except openai.error.RateLimitError:
+    except openai.RateLimitError:
         statuses.set(key, KeyStatus.quota)
         raise
-    except openai.error.PermissionError:
-        statuses.set(key, KeyStatus.broken)
-        raise
-    except openai.error.InvalidAPIType:
+    except openai.PermissionDeniedError:
         statuses.set(key, KeyStatus.broken)
         raise
     # TODO: test
-    except openai.error.APIError:
+    except openai.APIError:
         statuses.set(key, KeyStatus.unknown)
         raise
```

### Comparing `ffun-1.6.3/ffun/openai/tests/fixtures.py` & `ffun-1.7.0/ffun/openai/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/openai/tests/test_keys_rotator.py` & `ffun-1.7.0/ffun/openai/tests/test_keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/openai/tests/test_keys_statuses.py` & `ffun-1.7.0/ffun/openai/tests/test_keys_statuses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 from typing import Type
+from unittest.mock import MagicMock
 
 import openai
 import pytest
 from pytest_mock import MockerFixture
 
 from ffun.openai.entities import KeyStatus
 from ffun.openai.keys_statuses import Statuses, track_key_status
@@ -55,24 +56,22 @@
 class TestTrackKeyStatus:
     def test_works(self, statuses: Statuses) -> None:
         with track_key_status("key_1", statuses):
             pass
 
         assert statuses.get("key_1") == KeyStatus.works
 
-    @pytest.mark.parametrize(
-        "exception", [openai.error.AuthenticationError, openai.error.PermissionError, openai.error.InvalidAPIType]
-    )
+    @pytest.mark.parametrize("exception", [openai.AuthenticationError, openai.PermissionDeniedError])
     def test_authentication_error(self, exception: Type[Exception], statuses: Statuses) -> None:
         with pytest.raises(exception):
             with track_key_status("key_1", statuses):
-                raise exception()
+                raise exception(message="test-message", response=MagicMock(), body=MagicMock())  # type: ignore
 
         assert statuses.get("key_1") == KeyStatus.broken
 
-    @pytest.mark.parametrize("exception", [openai.error.RateLimitError])
+    @pytest.mark.parametrize("exception", [openai.RateLimitError])
     def test_quota_error(self, exception: Type[Exception], statuses: Statuses) -> None:
         with pytest.raises(exception):
             with track_key_status("key_1", statuses):
-                raise exception()
+                raise exception(message="test-message", response=MagicMock(), body=MagicMock())  # type: ignore
 
         assert statuses.get("key_1") == KeyStatus.quota
```

### Comparing `ffun-1.6.3/ffun/parsers/entities.py` & `ffun-1.7.0/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/feed.py` & `ffun-1.7.0/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/feedly.py` & `ffun-1.7.0/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml` & `ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json` & `ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml` & `ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json` & `ffun-1.7.0/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/parsers/tests/make.py` & `ffun-1.7.0/ffun/parsers/tests/make.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 
 def fake_entry_info(**kwargs: Any) -> EntryInfo:
     return EntryInfo(
         title=fake_title() if "title" not in kwargs else kwargs["title"],
         body=fake_body() if "body" not in kwargs else kwargs["body"],
         external_id=uuid.uuid4().hex if "external_id" not in kwargs else kwargs["external_id"],
         external_url=fake_url() if "external_url" not in kwargs else kwargs["external_url"],
-        external_tags={uuid.uuid4().hex, uuid.uuid4().hex}
-        if "external_tags" not in kwargs
-        else kwargs["external_tags"],
+        external_tags=(
+            {uuid.uuid4().hex, uuid.uuid4().hex} if "external_tags" not in kwargs else kwargs["external_tags"]
+        ),
         published_at=utils.now() if "published_at" not in kwargs else kwargs["published_at"],
     )
```

### Comparing `ffun-1.6.3/ffun/parsers/tests/test_feed.py` & `ffun-1.7.0/ffun/parsers/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/resources/domain.py` & `ffun-1.7.0/ffun/resources/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-1.7.0/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 resources-table
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/resources/operations.py` & `ffun-1.7.0/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/resources/tests/test_domain.py` & `ffun-1.7.0/ffun/resources/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/resources/tests/test_operations.py` & `ffun-1.7.0/ffun/resources/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/scores/domain.py` & `ffun-1.7.0/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-1.7.0/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 scores-tables
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py` & `ffun-1.7.0/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/scores/operations.py` & `ffun-1.7.0/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/scores/tests/test_domain.py` & `ffun-1.7.0/ffun/scores/tests/test_domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,9 +19,9 @@
             [[rule(4, {1, 2}), rule(5, {1, 3})], {1, 2, 3, 4}, (9, {1: 9, 2: 4, 3: 5})],
             [[rule(6, {1, 2}), rule(-7, {3, 5}), rule(8, {1, 4})], {2, 3, 4}, (0, {})],
             [[rule(9, {1, 2}), rule(-10, {3, 5}), rule(11, {4, 5})], {2, 3, 4, 5}, (1, {3: -10, 4: 11, 5: 1})],
             [[rule(9, {1, 2}), rule(-10, {3, 5}), rule(11, {4})], {2, 3, 4, 5}, (1, {3: -10, 4: 11, 5: -10})],
             [[rule(12, {1, 2}), rule(-12, {2, 3})], {1, 2, 3, 4, 5}, (0, {1: 12, 2: 0, 3: -12})],
         ],
     )
-    def test(self, rules: list[entities.BaseRule], tags: set[int], contributions: dict[int, int]) -> None:
+    def test(self, rules: list[entities.BaseRule], tags: set[int], contributions: tuple[int, dict[int, int]]) -> None:
         assert domain.get_score_contributions(rules, tags) == contributions
```

### Comparing `ffun-1.6.3/ffun/scores/tests/test_operations.py` & `ffun-1.7.0/ffun/scores/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/tags/converters.py` & `ffun-1.7.0/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/tags/tests/test_converters.py` & `ffun-1.7.0/ffun/tags/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/user_settings/domain.py` & `ffun-1.7.0/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-1.7.0/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 settings-table
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py` & `ffun-1.7.0/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 index-to-search-by-value
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__ = {"20230701_01_7zBP0-settings-table"}
```

### Comparing `ffun-1.6.3/ffun/user_settings/operations.py` & `ffun-1.7.0/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/user_settings/settings.py` & `ffun-1.7.0/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/user_settings/tests/test_domain.py` & `ffun-1.7.0/ffun/user_settings/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/user_settings/tests/test_operations.py` & `ffun-1.7.0/ffun/user_settings/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/user_settings/types.py` & `ffun-1.7.0/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/users/domain.py` & `ffun-1.7.0/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-1.7.0/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 users-mapping
 """
+
 from typing import Any
 
 from psycopg import Connection
 from yoyo import step
 
 __depends__: set[str] = set()
```

### Comparing `ffun-1.6.3/ffun/users/operations.py` & `ffun-1.7.0/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/ffun/users/tests/fixtures.py` & `ffun-1.7.0/ffun/users/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.6.3/pyproject.toml` & `ffun-1.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "1.6.3"
+version = "1.7.0"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
@@ -16,107 +16,111 @@
         "Framework :: AsyncIO",
         "Framework :: FastAPI",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Communications",
         "Topic :: Office/Business :: News/Diary",
         "Topic :: Text Processing",
         "Topic :: Text Processing :: Linguistic",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
         "Topic :: Internet :: WWW/HTTP :: HTTP Servers"]
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.12"
 
 uvicorn = {extras = ["standard"], version = "0.*"}
-fastapi = "0.103.*"
-pydantic = "2.4.*"
-pydantic-settings = "2.0.*"
-typer = "0.9.*"
+fastapi = "0.111.*"
+pydantic = "2.7.*"
+pydantic-settings = "2.2.*"
+typer = "0.12.*"
+
+# upgrade furher are blocked by supertokens-python
+httpx = "0.26.*"
 
-httpx = "0.24.*"
 brotlicffi = "1.1.*"
 # zstandard = "0.22.*"
 
-openai = "0.27.*"
-tiktoken = "0.4.*"
+openai = "1.30.*"
+tiktoken = "0.7.*"
 
-bidict = "0.22.*"
+bidict = "0.23.*"
 
 feedparser = "6.0.*"
 
 beautifulsoup4 = "4.12.*"
 
 async-lru = "2.0.*"
 
 psycopg = "3.1.*"
-psycopg-pool = "3.1.*"
+psycopg-pool = "3.2.*"
 yoyo-migrations = "8.2.*"
 PyPika = "0.48.*"
 
-structlog = "23.1.*"
+structlog = "24.2.*"
 
 yarl = "1.9.*"
 
 python-multipart = "0.0.*"
 
-supertokens-python = "0.14.*"
+supertokens-python = "0.21.*"
 
 python-slugify = "8.0.*"
 
-sentry-sdk = "1.29.*"
+sentry-sdk = "2.3.*"
 
 tabulate = "0.9.*"
 
-cryptography = "41.0.*"
+cryptography = "42.0.*"
 
-markdown = "3.4.*"
+markdown = "3.6.*"
 
 furl = "2.1.*"
 
 [tool.poetry.dev-dependencies]
 
-pytest = "7.4.*"
-pytest-asyncio = "0.21.*"
-pytest-mock = "3.11.*"
+changy = "0.*"
+
+pytest = "8.2.*"
+pytest-asyncio = "0.23.*"
+pytest-mock = "3.14.*"
 
 respx = "0.21.*"
 
-isort = "5.12.*"
-black = "23.7.*"
+isort = "5.13.*"
+black = "24.4.*"
 
-flake8 = "6.1.*"
+flake8 = "7.0.*"
 flake8-docstrings = "1.7.*"
 flake8-functions = "0.0.*"
 flake8-annotations-complexity = "0.0.*"
 flake8-cognitive-complexity = "0.1.*"
 flake8-pytest = "1.4.*"
 flake8-bandit = "4.1.*"
 flake8-absolute-import = "1.0.*"
 flake8-print = "5.0.*"
 flake8-pyproject = "1.2.*"
 flake8-eradicate = "1.5.*"
-autoflake = "2.2.*"
+autoflake = "2.3.*"
 
 # mypy fails in the latest versions
-mypy = "1.5.1"
+mypy = "1.10.*"
 
 types-python-slugify = "8.0.*"
 types-beautifulsoup4 = "4.12.*"
-types-markdown = "3.4.*"
+types-markdown = "3.6.*"
 types-pkg-resources = "0.1.*"
 types-tabulate = "0.9.*"
 
 [tool.poetry.scripts]
 
 ffun = "ffun.cli.cli:app"
 
@@ -163,17 +167,25 @@
 [[tool.mypy.overrides]]
 module = "pypika.*"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = """-x -vv --strict-markers -p no:cacheprovider"""
 filterwarnings = [
-   "error",
-    "ignore::DeprecationWarning:feedparser.encodings:29",
-    "ignore::DeprecationWarning:yoyo.migrations:34",
+  "error",
+  "ignore::DeprecationWarning:feedparser.encodings:29",
+  "ignore::DeprecationWarning:yoyo.migrations:34",
+
+  # datetime.datetime.utcnow
+  "ignore::DeprecationWarning:yoyo.backends.base:341",
+  "ignore::DeprecationWarning:yoyo.backends.base:541",
+  "ignore::DeprecationWarning:yoyo.backends.base:562",
+  "ignore::DeprecationWarning:yoyo.internalmigrations:68",
+
+  "ignore::pytest.PytestDeprecationWarning:pytest_asyncio.plugin:231"
 ]
 
 [tool.flake8]
 ignore = [
     "D100",
     "D101",
     "D102",
```

### Comparing `ffun-1.6.3/PKG-INFO` & `ffun-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 1.6.3
+Version: 1.7.0
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
@@ -30,35 +29,35 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Topic :: Office/Business :: News/Diary
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: PyPika (==0.48.*)
 Requires-Dist: async-lru (==2.0.*)
 Requires-Dist: beautifulsoup4 (==4.12.*)
-Requires-Dist: bidict (==0.22.*)
+Requires-Dist: bidict (==0.23.*)
 Requires-Dist: brotlicffi (==1.1.*)
-Requires-Dist: cryptography (==41.0.*)
-Requires-Dist: fastapi (==0.103.*)
+Requires-Dist: cryptography (==42.0.*)
+Requires-Dist: fastapi (==0.111.*)
 Requires-Dist: feedparser (==6.0.*)
 Requires-Dist: furl (==2.1.*)
-Requires-Dist: httpx (==0.24.*)
-Requires-Dist: markdown (==3.4.*)
-Requires-Dist: openai (==0.27.*)
+Requires-Dist: httpx (==0.26.*)
+Requires-Dist: markdown (==3.6.*)
+Requires-Dist: openai (==1.30.*)
 Requires-Dist: psycopg (==3.1.*)
-Requires-Dist: psycopg-pool (==3.1.*)
-Requires-Dist: pydantic (==2.4.*)
-Requires-Dist: pydantic-settings (==2.0.*)
+Requires-Dist: psycopg-pool (==3.2.*)
+Requires-Dist: pydantic (==2.7.*)
+Requires-Dist: pydantic-settings (==2.2.*)
 Requires-Dist: python-multipart (==0.0.*)
 Requires-Dist: python-slugify (==8.0.*)
-Requires-Dist: sentry-sdk (==1.29.*)
-Requires-Dist: structlog (==23.1.*)
-Requires-Dist: supertokens-python (==0.14.*)
+Requires-Dist: sentry-sdk (==2.3.*)
+Requires-Dist: structlog (==24.2.*)
+Requires-Dist: supertokens-python (==0.21.*)
 Requires-Dist: tabulate (==0.9.*)
-Requires-Dist: tiktoken (==0.4.*)
-Requires-Dist: typer (==0.9.*)
+Requires-Dist: tiktoken (==0.7.*)
+Requires-Dist: typer (==0.12.*)
 Requires-Dist: uvicorn[standard] (==0.*)
 Requires-Dist: yarl (==1.9.*)
 Requires-Dist: yoyo-migrations (==8.2.*)
 Project-URL: Repository, https://github.com/Tiendil/feeds.fun
 Description-Content-Type: text/markdown
 
 # Backend for Feeds Fun
```

