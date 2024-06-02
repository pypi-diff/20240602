# Comparing `tmp/buildz-0.5.8.tar.gz` & `tmp/buildz-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.8.tar", last modified: Thu May 30 13:45:08 2024, max compression
+gzip compressed data, was "buildz-0.5.9.tar", last modified: Sun Jun  2 05:21:38 2024, max compression
```

## Comparing `buildz-0.5.8.tar` & `buildz-0.5.9.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.871557 buildz-0.5.8/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.8/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2823 2024-05-30 13:45:08.871557 buildz-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.379677 buildz-0.5.8/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.8/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.8/buildz/__main__.py
--rw-rw-rw-   0        0        0     3530 2024-05-30 08:05:41.000000 buildz-0.5.8/buildz/argx.py
--rw-rw-rw-   0        0        0     2324 2024-05-30 12:26:10.000000 buildz-0.5.8/buildz/cmd.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.410089 buildz-0.5.8/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.425284 buildz-0.5.8/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.8/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.8/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.435724 buildz-0.5.8/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.8/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.8/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.450698 buildz-0.5.8/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.450698 buildz-0.5.8/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.8/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.8/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.8/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.8/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.8/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.457201 buildz-0.5.8/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.8/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.8/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.8/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.8/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.8/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-05-16 07:51:44.000000 buildz-0.5.8/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.457201 buildz-0.5.8/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.8/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.8/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.8/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.472902 buildz-0.5.8/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.8/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.8/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.472902 buildz-0.5.8/buildz/fz/
--rw-rw-rw-   0        0        0      317 2024-05-30 13:16:11.000000 buildz-0.5.8/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     2293 2024-05-20 08:56:56.000000 buildz-0.5.8/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      285 2024-05-24 11:29:24.000000 buildz-0.5.8/buildz/fz/fhs.py
--rw-rw-rw-   0        0        0     1298 2024-05-30 13:33:48.000000 buildz-0.5.8/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     3425 2024-05-20 14:01:07.000000 buildz-0.5.8/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.481262 buildz-0.5.8/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.8/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      121 2024-05-16 11:49:03.000000 buildz-0.5.8/buildz/ioc/base.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.8/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.488768 buildz-0.5.8/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2554 2024-05-21 09:04:50.000000 buildz-0.5.8/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     7462 2024-05-22 09:13:57.000000 buildz-0.5.8/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13616 2024-05-30 06:10:36.000000 buildz-0.5.8/buildz/ioc/ioc/confs.py
--rw-rw-rw-   0        0        0     1521 2024-05-16 15:35:31.000000 buildz-0.5.8/buildz/ioc/ioc/single.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.567910 buildz-0.5.8/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     6490 2024-05-21 12:22:23.000000 buildz-0.5.8/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1255 2024-05-16 14:17:26.000000 buildz-0.5.8/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.583950 buildz-0.5.8/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/iocf_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      352 2024-05-22 16:41:38.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.8/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0     1059 2024-05-16 14:13:56.000000 buildz-0.5.8/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      975 2024-05-16 14:13:36.000000 buildz-0.5.8/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.8/buildz/ioc/ioc_deal/iocf.py
--rw-rw-rw-   0        0        0      944 2024-05-16 14:13:13.000000 buildz-0.5.8/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1102 2024-05-16 14:12:34.000000 buildz-0.5.8/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1033 2024-05-16 14:17:05.000000 buildz-0.5.8/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6546 2024-05-16 15:31:49.000000 buildz-0.5.8/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1276 2024-05-16 14:15:31.000000 buildz-0.5.8/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      744 2024-05-16 14:45:17.000000 buildz-0.5.8/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1023 2024-05-22 16:42:24.000000 buildz-0.5.8/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.8/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     2295 2024-05-16 11:50:23.000000 buildz-0.5.8/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.591737 buildz-0.5.8/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.8/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.8/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.631213 buildz-0.5.8/buildz/xf/
--rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.8/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.8/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.8/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.663028 buildz-0.5.8/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.8/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.8/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.710453 buildz-0.5.8/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.8/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.8/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.8/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.8/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.8/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.8/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.8/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.8/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.8/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.8/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.8/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.8/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.8/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.8/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.766606 buildz-0.5.8/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.8/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.8/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.806146 buildz-0.5.8/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      988 2024-05-29 06:52:25.000000 buildz-0.5.8/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     2056 2024-05-16 07:51:17.000000 buildz-0.5.8/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1156 2024-05-16 07:57:06.000000 buildz-0.5.8/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0     1168 2024-05-29 06:53:06.000000 buildz-0.5.8/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      775 2024-05-29 06:45:07.000000 buildz-0.5.8/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.8/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.8/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      429 2024-05-29 06:44:45.000000 buildz-0.5.8/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.8/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     5683 2024-05-29 06:49:29.000000 buildz-0.5.8/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.8/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.8/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.8/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.8/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.8/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0      110 2024-05-29 06:55:41.000000 buildz-0.5.8/buildz/xf/loaderz/test1.py
--rw-rw-rw-   0        0        0     3681 2024-05-22 10:11:30.000000 buildz-0.5.8/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.8/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2815 2024-05-29 06:56:33.000000 buildz-0.5.8/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.8/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.8/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.821792 buildz-0.5.8/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.8/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.8/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.870563 buildz-0.5.8/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.8/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.8/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.8/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.8/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.8/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.8/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.8/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.8/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.393801 buildz-0.5.8/buildz.egg-info/
--rw-rw-rw-   0        0        0     2823 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3874 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 13:45:08.871557 buildz-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-05-30 13:42:20.000000 buildz-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.490450 buildz-0.5.9/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2823 2024-06-02 05:21:38.490450 buildz-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.220831 buildz-0.5.9/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.9/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.9/buildz/__main__.py
+-rw-rw-rw-   0        0        0     3530 2024-05-30 08:05:41.000000 buildz-0.5.9/buildz/argx.py
+-rw-rw-rw-   0        0        0     2330 2024-06-02 04:28:05.000000 buildz-0.5.9/buildz/cmd.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.247402 buildz-0.5.9/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.261526 buildz-0.5.9/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.9/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.9/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.261526 buildz-0.5.9/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.9/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.9/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.276542 buildz-0.5.9/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.323882 buildz-0.5.9/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.9/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.9/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.9/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.9/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.9/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.349474 buildz-0.5.9/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.9/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.9/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.9/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.9/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.9/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-05-16 07:51:44.000000 buildz-0.5.9/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.356212 buildz-0.5.9/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.9/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.9/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.9/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.371214 buildz-0.5.9/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.9/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.9/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.379974 buildz-0.5.9/buildz/fz/
+-rw-rw-rw-   0        0        0      332 2024-06-01 19:51:34.000000 buildz-0.5.9/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     2293 2024-05-20 08:56:56.000000 buildz-0.5.9/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      285 2024-05-24 11:29:24.000000 buildz-0.5.9/buildz/fz/fhs.py
+-rw-rw-rw-   0        0        0     1575 2024-06-02 03:17:21.000000 buildz-0.5.9/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     3425 2024-05-20 14:01:07.000000 buildz-0.5.9/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.379974 buildz-0.5.9/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.9/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-05-16 11:49:03.000000 buildz-0.5.9/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.9/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.379974 buildz-0.5.9/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2554 2024-05-21 09:04:50.000000 buildz-0.5.9/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     7462 2024-05-22 09:13:57.000000 buildz-0.5.9/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13616 2024-05-30 06:10:36.000000 buildz-0.5.9/buildz/ioc/ioc/confs.py
+-rw-rw-rw-   0        0        0     1521 2024-05-16 15:35:31.000000 buildz-0.5.9/buildz/ioc/ioc/single.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.408404 buildz-0.5.9/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     6490 2024-05-21 12:22:23.000000 buildz-0.5.9/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.9/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1255 2024-05-16 14:17:26.000000 buildz-0.5.9/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.421647 buildz-0.5.9/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/iocf_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      352 2024-05-22 16:41:38.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.9/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.9/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.9/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0     1059 2024-05-16 14:13:56.000000 buildz-0.5.9/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      975 2024-05-16 14:13:36.000000 buildz-0.5.9/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.9/buildz/ioc/ioc_deal/iocf.py
+-rw-rw-rw-   0        0        0      944 2024-05-16 14:13:13.000000 buildz-0.5.9/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1102 2024-05-16 14:12:34.000000 buildz-0.5.9/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1033 2024-05-16 14:17:05.000000 buildz-0.5.9/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.9/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6546 2024-05-16 15:31:49.000000 buildz-0.5.9/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.9/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1276 2024-05-16 14:15:31.000000 buildz-0.5.9/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      744 2024-05-16 14:45:17.000000 buildz-0.5.9/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1023 2024-05-22 16:42:24.000000 buildz-0.5.9/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.9/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     2429 2024-06-01 20:27:08.000000 buildz-0.5.9/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.435074 buildz-0.5.9/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.9/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.9/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.450709 buildz-0.5.9/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.9/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.9/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.9/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.450709 buildz-0.5.9/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.9/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.9/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.450709 buildz-0.5.9/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.9/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.9/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.9/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.9/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.9/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.9/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.9/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.9/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.9/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.9/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.9/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.9/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.9/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.9/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.466331 buildz-0.5.9/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.9/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.9/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.481956 buildz-0.5.9/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      988 2024-05-29 06:52:25.000000 buildz-0.5.9/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     2056 2024-05-16 07:51:17.000000 buildz-0.5.9/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1156 2024-05-16 07:57:06.000000 buildz-0.5.9/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0     1168 2024-05-29 06:53:06.000000 buildz-0.5.9/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      775 2024-05-29 06:45:07.000000 buildz-0.5.9/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.9/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.9/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      429 2024-05-29 06:44:45.000000 buildz-0.5.9/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.9/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     5683 2024-05-29 06:49:29.000000 buildz-0.5.9/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.9/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.9/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.9/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.9/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.9/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0      110 2024-05-29 06:55:41.000000 buildz-0.5.9/buildz/xf/loaderz/test1.py
+-rw-rw-rw-   0        0        0     3681 2024-05-22 10:11:30.000000 buildz-0.5.9/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.9/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2815 2024-05-29 06:56:33.000000 buildz-0.5.9/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.9/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.9/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.481956 buildz-0.5.9/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.9/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.9/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.490450 buildz-0.5.9/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.9/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.9/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.9/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.9/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.9/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.9/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.9/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.9/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:21:38.244931 buildz-0.5.9/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2823 2024-06-02 05:21:38.000000 buildz-0.5.9/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3874 2024-06-02 05:21:38.000000 buildz-0.5.9/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 05:21:38.000000 buildz-0.5.9/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-02 05:21:38.000000 buildz-0.5.9/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 05:21:38.490450 buildz-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-06-02 05:20:57.000000 buildz-0.5.9/setup.py
```

### Comparing `buildz-0.5.8/LICENSE` & `buildz-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/PKG-INFO` & `buildz-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.8
+Version: 0.5.9
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.8/README.md` & `buildz-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/argx.py` & `buildz-0.5.9/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/cmd.py` & `buildz-0.5.9/buildz/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,11 +68,11 @@
                 else:
                     fc = getattr(self.obj, fc)
                 params = arr[1:]
                 tmp = fc(*params)
                 print(tmp)
             except Exception as exp:
                 import traceback
-                print(f"error:{exp}")
+                print(f"[CMD] error:{exp}")
                 traceback.print_exc()
 
 pass
```

### Comparing `buildz-0.5.8/buildz/demo/ioc/deal.py` & `buildz-0.5.9/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/ioc/help.py` & `buildz-0.5.9/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/myers/deal.py` & `buildz-0.5.9/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/res/conf/main.js` & `buildz-0.5.9/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/res/help/ioc.js` & `buildz-0.5.9/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/res/help/myers.js` & `buildz-0.5.9/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/res/help/search.js` & `buildz-0.5.9/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/res/help/xf.js` & `buildz-0.5.9/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/res/test.js` & `buildz-0.5.9/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/search/deal.py` & `buildz-0.5.9/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/demo/test.py` & `buildz-0.5.9/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/fz/dirz.py` & `buildz-0.5.9/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/fz/fio.py` & `buildz-0.5.9/buildz/fz/fio.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,21 +52,33 @@
         fp = os.path.dirname(fp)
     return fp
 
 pass
 
 dirname = dirpath
 
-def removes(fp):
+def fcover(filepath, wsize = 1024*10):
+	st = os.stat(filepath)
+	size = st.st_size
+	bs = b'a'*wsize
+	with open(filepath, 'wb') as f:
+		for i in range(0, size, wsize):
+			f.write(bs)
+
+pass
+cover = fcover
+def removes(fp, cover = False):
     if not os.path.exists(fp):
         return
     if os.path.isfile(fp):
         #print(f"remove file '{fp}'")
+        if cover:
+            fcover(fp)
         os.remove(fp)
         return
     fps = os.listdir(fp)
     fps = [os.path.join(fp, f) for f in fps]
-    [removes(f) for f in fps]
+    [removes(f, cover) for f in fps]
     #print(f"removedirs '{fp}'")
     os.rmdir(fp)
 
 pass
```

### Comparing `buildz-0.5.8/buildz/fz/lsf.py` & `buildz-0.5.9/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc/base.py` & `buildz-0.5.9/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc/conf.py` & `buildz-0.5.9/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc/confs.py` & `buildz-0.5.9/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc/single.py` & `buildz-0.5.9/buildz/ioc/ioc/single.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.9/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.9/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/conf/ref_lists.js` & `buildz-0.5.9/buildz/ioc/ioc_deal/conf/ref_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/iocf.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/iocf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/ioc/ioc_deal/xfile.py` & `buildz-0.5.9/buildz/ioc/ioc_deal/xfile.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/pyz.py` & `buildz-0.5.9/buildz/pyz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 
 import sys
 import os
+import hashlib
+def hashcode(s):
+    if type(s)==str:
+        s = s.encode("utf-8")
+    return hashlib.md5(s).hexdigest()
+
+pass
 def test_current(fp, up = 1):
     """
         将当前目录的上{up}层目录加入sys.path，这样可以在同层写测试代码，但是import还是要当在上{up}层做import
     """
     dp = os.path.dirname(os.path.abspath(fp))
     for i in range(up):
         dp = os.path.dirname(dp)
```

### Comparing `buildz-0.5.8/buildz/tz/myers_diff.py` & `buildz-0.5.9/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/file.py` & `buildz-0.5.9/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/base.py` & `buildz-0.5.9/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/buffer.py` & `buildz-0.5.9/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/listz.py` & `buildz-0.5.9/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/lr.py` & `buildz-0.5.9/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.9/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.9/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.9/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/reval.py` & `buildz-0.5.9/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/setz.py` & `buildz-0.5.9/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/spt.py` & `buildz-0.5.9/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/deal/strz.py` & `buildz-0.5.9/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/item.py` & `buildz-0.5.9/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/mg.py` & `buildz-0.5.9/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loader/pos.py` & `buildz-0.5.9/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/base.py` & `buildz-0.5.9/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/buffer.py` & `buildz-0.5.9/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/nextz.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.9/buildz/xf/loaderz/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/item.py` & `buildz-0.5.9/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/mg.py` & `buildz-0.5.9/buildz/xf/loaderz/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/pos.py` & `buildz-0.5.9/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/loaderz/test.py` & `buildz-0.5.9/buildz/xf/loaderz/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/mapz.py` & `buildz-0.5.9/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/read.py` & `buildz-0.5.9/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/readz.py` & `buildz-0.5.9/buildz/xf/readz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/stack.py` & `buildz-0.5.9/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/write.py` & `buildz-0.5.9/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/base.py` & `buildz-0.5.9/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/conf.py` & `buildz-0.5.9/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/deal/listz.py` & `buildz-0.5.9/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.9/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/deal/strz.py` & `buildz-0.5.9/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/itemz.py` & `buildz-0.5.9/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/writer/mg.py` & `buildz-0.5.9/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz/xf/xargs.py` & `buildz-0.5.9/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/buildz.egg-info/PKG-INFO` & `buildz-0.5.9/buildz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.8
+Version: 0.5.9
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.8/buildz.egg-info/SOURCES.txt` & `buildz-0.5.9/buildz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildz-0.5.8/setup.py` & `buildz-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.8',
+    version = '0.5.9',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

