# Comparing `tmp/tcrutils-12.0.179.tar.gz` & `tmp/tcrutils-12.0.180.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcrutils-12.0.179.tar", max compression
+gzip compressed data, was "tcrutils-12.0.180.tar", max compression
```

## Comparing `tcrutils-12.0.179.tar` & `tcrutils-12.0.180.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.179/LICENSE
--rw-r--r--   0        0        0      609 2024-05-31 23:41:06.207384 tcrutils-12.0.179/pyproject.toml
--rw-r--r--   0        0        0     2702 2024-05-30 00:41:07.849953 tcrutils-12.0.179/README.md
--rw-r--r--   0        0        0     4989 2024-05-31 23:41:02.379226 tcrutils-12.0.179/tcrutils/__init__.py
--rw-r--r--   0        0        0      209 2024-05-31 23:41:08.731741 tcrutils-12.0.179/tcrutils/_version.py
--rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.179/tcrutils/discord/__init__.py
--rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.179/tcrutils/discord/tcrd_alias.py
--rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.179/tcrutils/discord/tcrd_constants.py
--rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.179/tcrutils/discord/tcrd_embeds.py
--rw-r--r--   0        0        0      445 2024-05-22 16:38:45.538275 tcrutils-12.0.179/tcrutils/discord/tcrd_limits.py
--rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.179/tcrutils/discord/tcrd_permissions.py
--rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.179/tcrutils/discord/tcrd_snowflake.py
--rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.179/tcrutils/discord/tcrd_string.py
--rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.179/tcrutils/discord/tcrd_types.py
--rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.179/tcrutils/dr/__init__.py
--rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.179/tcrutils/dr/core.py
--rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.179/tcrutils/dr/error.py
--rw-r--r--   0        0        0     5744 2024-05-15 21:25:46.216676 tcrutils-12.0.179/tcrutils/dr/EXECUTE.md
--rw-r--r--   0        0        0     3647 2024-05-15 22:09:37.638712 tcrutils-12.0.179/tcrutils/dr/placeholder_sets.py
--rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.179/tcrutils/dr/placeholders/__init__.py
--rw-r--r--   0        0        0     9539 2024-05-15 15:53:54.306491 tcrutils-12.0.179/tcrutils/dr/placeholders/p_discord.py
--rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.179/tcrutils/dr/placeholders/p_math.py
--rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.179/tcrutils/dr/placeholders/p_text.py
--rw-r--r--   0        0        0    14654 2024-05-18 16:30:33.599876 tcrutils-12.0.179/tcrutils/dr/PLACEHOLDERS.md
--rw-r--r--   0        0        0     6233 2024-05-15 22:16:27.695353 tcrutils-12.0.179/tcrutils/dr/util.py
--rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.179/tcrutils/imgui/__init__.py
--rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.179/tcrutils/imgui/tcri_dependencies.py
--rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.179/tcrutils/imgui/tcri_handler.py
--rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.179/tcrutils/imgui/types/tcri_types_imgui.py
--rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.179/tcrutils/src/tcr_b64.py
--rw-r--r--   0        0        0      980 2024-05-22 09:51:37.173518 tcrutils-12.0.179/tcrutils/src/tcr_class.py
--rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.179/tcrutils/src/tcr_classfuncs.py
--rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.179/tcrutils/src/tcr_cloud_imports.py
--rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.179/tcrutils/src/tcr_compare.py
--rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.179/tcrutils/src/tcr_console.py
--rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.179/tcrutils/src/tcr_constants.py
--rw-r--r--   0        0        0     6457 2024-05-22 16:38:45.539276 tcrutils-12.0.179/tcrutils/src/tcr_decorator.py
--rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.179/tcrutils/src/tcr_dev.py
--rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.179/tcrutils/src/tcr_dict.py
--rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.179/tcrutils/src/tcr_dir.py
--rw-r--r--   0        0        0     2279 2024-05-29 19:59:54.249054 tcrutils-12.0.179/tcrutils/src/tcr_ensure_deps.py
--rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.179/tcrutils/src/tcr_error.py
--rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.179/tcrutils/src/tcr_extract_error.py
--rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.179/tcrutils/src/tcr_F.py
--rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.179/tcrutils/src/tcr_getch.py
--rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.179/tcrutils/src/tcr_inject.py
--rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.179/tcrutils/src/tcr_input.py
--rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.179/tcrutils/src/tcr_inspect.py
--rw-r--r--   0        0        0     1106 2024-05-14 16:33:00.727996 tcrutils-12.0.179/tcrutils/src/tcr_int.py
--rw-r--r--   0        0        0     7706 2024-05-23 12:53:10.953982 tcrutils-12.0.179/tcrutils/src/tcr_iterable.py
--rw-r--r--   0        0        0     3438 2024-05-15 16:14:26.304132 tcrutils-12.0.179/tcrutils/src/tcr_joke.py
--rw-r--r--   0        0        0     2865 2024-05-31 22:49:34.035185 tcrutils-12.0.179/tcrutils/src/tcr_language.py
--rw-r--r--   0        0        0     2860 2024-05-22 16:38:45.539276 tcrutils-12.0.179/tcrutils/src/tcr_markdown.py
--rw-r--r--   0        0        0      421 2024-05-29 19:34:31.473824 tcrutils-12.0.179/tcrutils/src/tcr_menuconfig.py
--rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.179/tcrutils/src/tcr_misspellings.py
--rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.179/tcrutils/src/tcr_null.py
--rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.179/tcrutils/src/tcr_other.py
--rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.179/tcrutils/src/tcr_overload.py
--rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.179/tcrutils/src/tcr_path.py
--rw-r--r--   0        0        0    29421 2024-05-21 21:23:31.164988 tcrutils-12.0.179/tcrutils/src/tcr_print.py
--rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.179/tcrutils/src/tcr_regex.py
--rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.179/tcrutils/src/tcr_run.py
--rw-r--r--   0        0        0     5396 2024-05-22 20:58:16.446539 tcrutils-12.0.179/tcrutils/src/tcr_sdb.py
--rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.179/tcrutils/src/tcr_string.py
--rw-r--r--   0        0        0      358 2024-05-22 10:36:37.266846 tcrutils-12.0.179/tcrutils/src/tcr_temp.py
--rw-r--r--   0        0        0     1451 2024-05-29 17:59:30.096505 tcrutils-12.0.179/tcrutils/src/tcr_terminal.py
--rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.179/tcrutils/src/tcr_test.py
--rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.179/tcrutils/src/tcr_timestr.py
--rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.179/tcrutils/src/tcr_types.py
--rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.179/tcrutils/src/tcr_uptime.py
--rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.179/tcrutils/src/tcr_void.py
--rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 tcrutils-12.0.179/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.180/LICENSE
+-rw-r--r--   0        0        0      609 2024-06-02 21:24:37.323516 tcrutils-12.0.180/pyproject.toml
+-rw-r--r--   0        0        0     2702 2024-05-30 00:41:07.849953 tcrutils-12.0.180/README.md
+-rw-r--r--   0        0        0     4989 2024-06-02 21:11:42.185850 tcrutils-12.0.180/tcrutils/__init__.py
+-rw-r--r--   0        0        0      209 2024-06-02 21:24:40.055802 tcrutils-12.0.180/tcrutils/_version.py
+-rw-r--r--   0        0        0      851 2024-06-02 21:10:46.109895 tcrutils-12.0.180/tcrutils/discord/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.180/tcrutils/discord/tcrd_alias.py
+-rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.180/tcrutils/discord/tcrd_constants.py
+-rw-r--r--   0        0        0     5450 2024-06-02 21:09:40.879309 tcrutils-12.0.180/tcrutils/discord/tcrd_dpy.py
+-rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.180/tcrutils/discord/tcrd_embeds.py
+-rw-r--r--   0        0        0      445 2024-05-22 16:38:45.538275 tcrutils-12.0.180/tcrutils/discord/tcrd_limits.py
+-rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.180/tcrutils/discord/tcrd_permissions.py
+-rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.180/tcrutils/discord/tcrd_snowflake.py
+-rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.180/tcrutils/discord/tcrd_string.py
+-rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.180/tcrutils/discord/tcrd_types.py
+-rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.180/tcrutils/dr/__init__.py
+-rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.180/tcrutils/dr/core.py
+-rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.180/tcrutils/dr/error.py
+-rw-r--r--   0        0        0     5744 2024-05-15 21:25:46.216676 tcrutils-12.0.180/tcrutils/dr/EXECUTE.md
+-rw-r--r--   0        0        0     3647 2024-05-15 22:09:37.638712 tcrutils-12.0.180/tcrutils/dr/placeholder_sets.py
+-rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.180/tcrutils/dr/placeholders/__init__.py
+-rw-r--r--   0        0        0     9539 2024-05-15 15:53:54.306491 tcrutils-12.0.180/tcrutils/dr/placeholders/p_discord.py
+-rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.180/tcrutils/dr/placeholders/p_math.py
+-rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.180/tcrutils/dr/placeholders/p_text.py
+-rw-r--r--   0        0        0    14654 2024-05-18 16:30:33.599876 tcrutils-12.0.180/tcrutils/dr/PLACEHOLDERS.md
+-rw-r--r--   0        0        0     6233 2024-05-15 22:16:27.695353 tcrutils-12.0.180/tcrutils/dr/util.py
+-rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.180/tcrutils/imgui/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.180/tcrutils/imgui/tcri_dependencies.py
+-rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.180/tcrutils/imgui/tcri_handler.py
+-rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.180/tcrutils/imgui/types/tcri_types_imgui.py
+-rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.180/tcrutils/src/tcr_b64.py
+-rw-r--r--   0        0        0      980 2024-05-22 09:51:37.173518 tcrutils-12.0.180/tcrutils/src/tcr_class.py
+-rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.180/tcrutils/src/tcr_classfuncs.py
+-rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.180/tcrutils/src/tcr_cloud_imports.py
+-rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.180/tcrutils/src/tcr_compare.py
+-rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.180/tcrutils/src/tcr_console.py
+-rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.180/tcrutils/src/tcr_constants.py
+-rw-r--r--   0        0        0      137 2024-06-02 21:19:15.105584 tcrutils-12.0.180/tcrutils/src/tcr_context.py
+-rw-r--r--   0        0        0     6457 2024-05-22 16:38:45.539276 tcrutils-12.0.180/tcrutils/src/tcr_decorator.py
+-rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.180/tcrutils/src/tcr_dev.py
+-rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.180/tcrutils/src/tcr_dict.py
+-rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.180/tcrutils/src/tcr_dir.py
+-rw-r--r--   0        0        0     2279 2024-05-29 19:59:54.249054 tcrutils-12.0.180/tcrutils/src/tcr_ensure_deps.py
+-rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.180/tcrutils/src/tcr_error.py
+-rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.180/tcrutils/src/tcr_extract_error.py
+-rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.180/tcrutils/src/tcr_F.py
+-rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.180/tcrutils/src/tcr_getch.py
+-rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.180/tcrutils/src/tcr_inject.py
+-rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.180/tcrutils/src/tcr_input.py
+-rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.180/tcrutils/src/tcr_inspect.py
+-rw-r--r--   0        0        0     1106 2024-05-14 16:33:00.727996 tcrutils-12.0.180/tcrutils/src/tcr_int.py
+-rw-r--r--   0        0        0     7706 2024-05-23 12:53:10.953982 tcrutils-12.0.180/tcrutils/src/tcr_iterable.py
+-rw-r--r--   0        0        0     3438 2024-05-15 16:14:26.304132 tcrutils-12.0.180/tcrutils/src/tcr_joke.py
+-rw-r--r--   0        0        0     2865 2024-05-31 22:49:34.035185 tcrutils-12.0.180/tcrutils/src/tcr_language.py
+-rw-r--r--   0        0        0     2860 2024-05-22 16:38:45.539276 tcrutils-12.0.180/tcrutils/src/tcr_markdown.py
+-rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.180/tcrutils/src/tcr_misspellings.py
+-rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.180/tcrutils/src/tcr_null.py
+-rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.180/tcrutils/src/tcr_other.py
+-rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.180/tcrutils/src/tcr_overload.py
+-rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.180/tcrutils/src/tcr_path.py
+-rw-r--r--   0        0        0    29421 2024-05-21 21:23:31.164988 tcrutils-12.0.180/tcrutils/src/tcr_print.py
+-rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.180/tcrutils/src/tcr_regex.py
+-rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.180/tcrutils/src/tcr_run.py
+-rw-r--r--   0        0        0     5396 2024-05-22 20:58:16.446539 tcrutils-12.0.180/tcrutils/src/tcr_sdb.py
+-rw-r--r--   0        0        0     4073 2024-06-02 21:24:24.002149 tcrutils-12.0.180/tcrutils/src/tcr_string.py
+-rw-r--r--   0        0        0      358 2024-05-22 10:36:37.266846 tcrutils-12.0.180/tcrutils/src/tcr_temp.py
+-rw-r--r--   0        0        0     1451 2024-05-29 17:59:30.096505 tcrutils-12.0.180/tcrutils/src/tcr_terminal.py
+-rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.180/tcrutils/src/tcr_test.py
+-rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.180/tcrutils/src/tcr_timestr.py
+-rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.180/tcrutils/src/tcr_types.py
+-rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.180/tcrutils/src/tcr_uptime.py
+-rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.180/tcrutils/src/tcr_void.py
+-rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 tcrutils-12.0.180/PKG-INFO
```

### Comparing `tcrutils-12.0.179/LICENSE` & `tcrutils-12.0.180/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/pyproject.toml` & `tcrutils-12.0.180/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 extend = "C:/CUSTOM_ASSETS/pyproject.toml"
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 
 [tool.poetry]
 name = "tcrutils"
-version = "12.0.179"
+version = "12.0.180"
 description = "Useful stuff for TCR projects!"
 authors = ["TheCreatorrrr"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11.0,<3.13"
```

### Comparing `tcrutils-12.0.179/README.md` & `tcrutils-12.0.180/README.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/__init__.py` & `tcrutils-12.0.180/tcrutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 from .discord.tcrd_embeds import embed, modal
 from .discord.tcrd_limits import DiscordLimits
 from .discord.tcrd_string import get_token
 from .dr import placeholder_set as dr_placeholder_sets
 from .dr import placeholders as dr_placeholders
 from .src import tcr_ensure_deps as ensure_depencencies
 from .src import tcr_joke as joke
-from .src import tcr_menuconfig as menuconfig
 from .src import tcr_types as types
 from .src.tcr_b64 import b64
 from .src.tcr_class import NoInit, Singleton
 from .src.tcr_classfuncs import get_classname, get_name_classname, get_qualname_classname
 from .src.tcr_compare import able, isdunder
 from .src.tcr_console import breakpoint, console, start_eval_session
 from .src.tcr_console import console as c
 from .src.tcr_constants import *
+from .src.tcr_context import random_seed_lock
 from .src.tcr_decorator import autorun, convert, copy_kwargs, instance, skip_first_call, skip_first_call_async, test, timeit
 from .src.tcr_dev import generate_function_argument_typehints, generate_type_hinter
 from .src.tcr_dict import DotDict, JSDict, JSDotDict, clean_dunder_dict, dict_zip, merge_dicts
 from .src.tcr_dir import dir2, dir3
 from .src.tcr_error import error  # 'tcrerror' in star imports, either in 'tcr.error'/'tcr.tcrerror'
 from .src.tcr_error import error as tcrerror
 from .src.tcr_extract_error import extract_error, extract_traceback
```

### Comparing `tcrutils-12.0.179/tcrutils/discord/__init__.py` & `tcrutils-12.0.180/tcrutils/discord/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """TCRUtils Discord. Contains various features related to bot development on discord and other stuff maybe."""
 
 from . import tcrd_types as types
 from .tcrd_alias import get_guild_count
 from .tcrd_constants import DISCORD_EPOCH
+from .tcrd_dpy import escape_markdown, escape_mentions, remove_markdown
 from .tcrd_embeds import embed, modal
 from .tcrd_limits import DiscordLimits
 from .tcrd_permissions import PERMISSIONS_DICT, Permission, permissions
 from .tcrd_permissions import Permission as DiscordPermission
 from .tcrd_permissions import permissions as discord_permissions
 from .tcrd_snowflake import Snowflake, is_snowflake
 from .tcrd_string import IFYs, get_token
```

### Comparing `tcrutils-12.0.179/tcrutils/discord/tcrd_embeds.py` & `tcrutils-12.0.180/tcrutils/discord/tcrd_embeds.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/discord/tcrd_permissions.py` & `tcrutils-12.0.180/tcrutils/discord/tcrd_permissions.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/discord/tcrd_snowflake.py` & `tcrutils-12.0.180/tcrutils/discord/tcrd_snowflake.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/discord/tcrd_string.py` & `tcrutils-12.0.180/tcrutils/discord/tcrd_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/discord/tcrd_types.py` & `tcrutils-12.0.180/tcrutils/discord/tcrd_types.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/core.py` & `tcrutils-12.0.180/tcrutils/dr/core.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/error.py` & `tcrutils-12.0.180/tcrutils/dr/error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/EXECUTE.md` & `tcrutils-12.0.180/tcrutils/dr/EXECUTE.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/placeholder_sets.py` & `tcrutils-12.0.180/tcrutils/dr/placeholder_sets.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/placeholders/p_discord.py` & `tcrutils-12.0.180/tcrutils/dr/placeholders/p_discord.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/placeholders/p_math.py` & `tcrutils-12.0.180/tcrutils/dr/placeholders/p_math.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/placeholders/p_text.py` & `tcrutils-12.0.180/tcrutils/dr/placeholders/p_text.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/PLACEHOLDERS.md` & `tcrutils-12.0.180/tcrutils/dr/PLACEHOLDERS.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/dr/util.py` & `tcrutils-12.0.180/tcrutils/dr/util.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/imgui/tcri_dependencies.py` & `tcrutils-12.0.180/tcrutils/imgui/tcri_dependencies.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/imgui/tcri_handler.py` & `tcrutils-12.0.180/tcrutils/imgui/tcri_handler.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/imgui/types/tcri_types_imgui.py` & `tcrutils-12.0.180/tcrutils/imgui/types/tcri_types_imgui.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_class.py` & `tcrutils-12.0.180/tcrutils/src/tcr_class.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_classfuncs.py` & `tcrutils-12.0.180/tcrutils/src/tcr_classfuncs.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_cloud_imports.py` & `tcrutils-12.0.180/tcrutils/src/tcr_cloud_imports.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_compare.py` & `tcrutils-12.0.180/tcrutils/src/tcr_compare.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_console.py` & `tcrutils-12.0.180/tcrutils/src/tcr_console.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_decorator.py` & `tcrutils-12.0.180/tcrutils/src/tcr_decorator.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_dev.py` & `tcrutils-12.0.180/tcrutils/src/tcr_dev.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_dict.py` & `tcrutils-12.0.180/tcrutils/src/tcr_dict.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_ensure_deps.py` & `tcrutils-12.0.180/tcrutils/src/tcr_ensure_deps.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_error.py` & `tcrutils-12.0.180/tcrutils/src/tcr_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_extract_error.py` & `tcrutils-12.0.180/tcrutils/src/tcr_extract_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_getch.py` & `tcrutils-12.0.180/tcrutils/src/tcr_getch.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_inject.py` & `tcrutils-12.0.180/tcrutils/src/tcr_inject.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_input.py` & `tcrutils-12.0.180/tcrutils/src/tcr_input.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_inspect.py` & `tcrutils-12.0.180/tcrutils/src/tcr_inspect.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_int.py` & `tcrutils-12.0.180/tcrutils/src/tcr_int.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_iterable.py` & `tcrutils-12.0.180/tcrutils/src/tcr_iterable.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_joke.py` & `tcrutils-12.0.180/tcrutils/src/tcr_joke.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_language.py` & `tcrutils-12.0.180/tcrutils/src/tcr_language.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_markdown.py` & `tcrutils-12.0.180/tcrutils/src/tcr_markdown.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_misspellings.py` & `tcrutils-12.0.180/tcrutils/src/tcr_misspellings.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_null.py` & `tcrutils-12.0.180/tcrutils/src/tcr_null.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_overload.py` & `tcrutils-12.0.180/tcrutils/src/tcr_overload.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_path.py` & `tcrutils-12.0.180/tcrutils/src/tcr_path.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_print.py` & `tcrutils-12.0.180/tcrutils/src/tcr_print.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_regex.py` & `tcrutils-12.0.180/tcrutils/src/tcr_regex.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_run.py` & `tcrutils-12.0.180/tcrutils/src/tcr_run.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_sdb.py` & `tcrutils-12.0.180/tcrutils/src/tcr_sdb.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_string.py` & `tcrutils-12.0.180/tcrutils/src/tcr_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re as regex
 
-from .tcr_int import clamp, float2int
+from .tcr_int import clamp
 
 
 def commafy(text: str | int, splitter: str = ','):
   """Commafy a number.
 
   Returns a string of that number split by commas if needed, or any character passed as splitter.
   """
@@ -29,15 +29,15 @@
 class SlashableString(str):
   """Represents a string that can be concatenated with another string along with a splitter by the use of the divide operator.
 
   Example:
   ```py
   s = SlashableString("a")
   s1 = s / 'c'
-  print(repr(s)) # -> 'a/c'
+  print(repr(s1)) # -> 'a/c'
   ```
   Splitter can be changed with the `splitter` argument. (the splitter is '/' by default to be consistent with the division symbol)
   If strip argument is True, the string will be stripped of any leading or trailing splitters.
   If cleanup argument is True, the string will be cleaned up by replacing any double splitters with a single splitter (a.com//////b -> a.com/b).
 
   The floor division operator (`//`) is the same as the slash operator (`/`) except that it doesn't strip or cleanup the string afterwards, regardless of the settings.
   """
```

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_terminal.py` & `tcrutils-12.0.180/tcrutils/src/tcr_terminal.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_test.py` & `tcrutils-12.0.180/tcrutils/src/tcr_test.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_timestr.py` & `tcrutils-12.0.180/tcrutils/src/tcr_timestr.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_uptime.py` & `tcrutils-12.0.180/tcrutils/src/tcr_uptime.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/tcrutils/src/tcr_void.py` & `tcrutils-12.0.180/tcrutils/src/tcr_void.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.179/PKG-INFO` & `tcrutils-12.0.180/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcrutils
-Version: 12.0.179
+Version: 12.0.180
 Summary: Useful stuff for TCR projects!
 License: GPL-3.0
 Author: TheCreatorrrr
 Requires-Python: >=3.11.0,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tcrutils Version: 12.0.179 Summary: Useful stuff
+Metadata-Version: 2.1 Name: tcrutils Version: 12.0.180 Summary: Useful stuff
 for TCR projects! License: GPL-3.0 Author: TheCreatorrrr Requires-Python:
 >=3.11.0,<3.13 Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: attr (>=0.3.2,<0.4.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: colored (>=2.2.4,<3.0.0) Requires-Dist: hikari
 (>=2.0.0.dev122,<3.0.0) Requires-Dist: hikari-arc (>=1.3.0,<2.0.0) Requires-
```

