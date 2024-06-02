# Comparing `tmp/mapdata-3.7.2.tar.gz` & `tmp/mapdata-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-3.7.2.tar", last modified: Wed May 29 20:15:00 2024, max compression
+gzip compressed data, was "mapdata-3.8.0.tar", last modified: Sun Jun  2 16:56:21 2024, max compression
```

## Comparing `mapdata-3.7.2.tar` & `mapdata-3.8.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.634091 mapdata-3.7.2/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.7.2/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.7.2/MANIFEST.in
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-29 20:15:00.630091 mapdata-3.7.2/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     6421 2024-05-04 17:16:18.000000 mapdata-3.7.2/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.574090 mapdata-3.7.2/mapdata/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.578091 mapdata-3.7.2/mapdata/configfile/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.7.2/mapdata/configfile/mapdata.conf
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   693471 2024-05-29 19:29:21.000000 mapdata-3.7.2/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.574090 mapdata-3.7.2/mapdata/symbols/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/16x16/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/0.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.7.2/mapdata/symbols/16x16/1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.7.2/mapdata/symbols/16x16/2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.7.2/mapdata/symbols/16x16/4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.7.2/mapdata/symbols/16x16/5.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.7.2/mapdata/symbols/16x16/6.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/7.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.7.2/mapdata/symbols/16x16/9.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/A.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.7.2/mapdata/symbols/16x16/B.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/C.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/D.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.7.2/mapdata/symbols/16x16/E.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/F.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/G.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/H.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.7.2/mapdata/symbols/16x16/I.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.7.2/mapdata/symbols/16x16/J.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/K.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.7.2/mapdata/symbols/16x16/L.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.7.2/mapdata/symbols/16x16/M.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.7.2/mapdata/symbols/16x16/N.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/O.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/P.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.7.2/mapdata/symbols/16x16/Q.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.7.2/mapdata/symbols/16x16/R.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.7.2/mapdata/symbols/16x16/S.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/T.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/U.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.7.2/mapdata/symbols/16x16/V.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.7.2/mapdata/symbols/16x16/W.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/X.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/Y.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/Z.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.7.2/mapdata/symbols/16x16/airplane.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.7.2/mapdata/symbols/16x16/anchor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/ball.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/ball_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.7.2/mapdata/symbols/16x16/bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.7.2/mapdata/symbols/16x16/bars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/binoculars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/bird.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/block.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.7.2/mapdata/symbols/16x16/block_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/bookmark.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.7.2/mapdata/symbols/16x16/box_stack.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/camera.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/cancel.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/car.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/car2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/center8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/check.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/check_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.7.2/mapdata/symbols/16x16/checkbox.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/checkerboard.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.7.2/mapdata/symbols/16x16/chevrons.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.7.2/mapdata/symbols/16x16/circle_x.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/clock.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.7.2/mapdata/symbols/16x16/columns.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.7.2/mapdata/symbols/16x16/contract.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.7.2/mapdata/symbols/16x16/cross.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/darkeye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.7.2/mapdata/symbols/16x16/decrease.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.7.2/mapdata/symbols/16x16/deposition.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_ll.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_lr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_ul.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/diag_ur.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/dialog.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.7.2/mapdata/symbols/16x16/diamond.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/donkey.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/dot.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.7.2/mapdata/symbols/16x16/down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.7.2/mapdata/symbols/16x16/drop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/elephant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/expand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.7.2/mapdata/symbols/16x16/eye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.7.2/mapdata/symbols/16x16/fire.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/fish.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.7.2/mapdata/symbols/16x16/flag.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.7.2/mapdata/symbols/16x16/flag2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/four_arrows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.7.2/mapdata/symbols/16x16/graph.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/hand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/hash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.7.2/mapdata/symbols/16x16/heart.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/hidden.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/hourglass.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.7.2/mapdata/symbols/16x16/house.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/increase.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/info.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.7.2/mapdata/symbols/16x16/leaf.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.7.2/mapdata/symbols/16x16/lightbulb.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/lightning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.7.2/mapdata/symbols/16x16/lightning2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/location_ptr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.7.2/mapdata/symbols/16x16/mine.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/nested_boxes.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.7.2/mapdata/symbols/16x16/pennant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/pennant2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.7.2/mapdata/symbols/16x16/people.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/person.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/person2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/person3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.7.2/mapdata/symbols/16x16/phone.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/photo.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/picnic.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.7.2/mapdata/symbols/16x16/plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/point_up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_ne.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_nw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_se.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/pointer_sw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.7.2/mapdata/symbols/16x16/puzzle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/q1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.7.2/mapdata/symbols/16x16/q1_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.7.2/mapdata/symbols/16x16/q2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.7.2/mapdata/symbols/16x16/q2_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.7.2/mapdata/symbols/16x16/q3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.7.2/mapdata/symbols/16x16/q3_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/q4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/q4_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.7.2/mapdata/symbols/16x16/qmark_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.7.2/mapdata/symbols/16x16/qmark_circle2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/raincloud.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/rocket.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/rocket2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.7.2/mapdata/symbols/16x16/rose.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/rows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/scales.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/search.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.7.2/mapdata/symbols/16x16/search2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.7.2/mapdata/symbols/16x16/skull.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.7.2/mapdata/symbols/16x16/square.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.7.2/mapdata/symbols/16x16/star.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.7.2/mapdata/symbols/16x16/stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/stop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/surprise_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.7.2/mapdata/symbols/16x16/swamp.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/target.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.7.2/mapdata/symbols/16x16/target2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/ten.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.7.2/mapdata/symbols/16x16/trash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/tree.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.7.2/mapdata/symbols/16x16/tree2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.7.2/mapdata/symbols/16x16/tree3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.7.2/mapdata/symbols/16x16/triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.7.2/mapdata/symbols/16x16/triangle_open.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.7.2/mapdata/symbols/16x16/triangle_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.7.2/mapdata/symbols/16x16/up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.7.2/mapdata/symbols/16x16/vapor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.7.2/mapdata/symbols/16x16/warning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.7.2/mapdata/symbols/16x16/wave.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.7.2/mapdata/symbols/16x16/wave2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.7.2/mapdata/symbols/16x16/wave3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/weather.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.7.2/mapdata/symbols/16x16/wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.7.2/mapdata/symbols/16x16/wedge_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.7.2/mapdata/symbols/16x16/wedges_3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.7.2/mapdata/symbols/16x16/well.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.7.2/mapdata/symbols/16x16/whale.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.7.2/mapdata/symbols/16x16/whale2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.7.2/mapdata/symbols/16x16/wheelchair.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.7.2/mapdata/symbols/16x16/zigzags.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.7.2/mapdata/symbols/16x16/zigzags2.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/20x20/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.7.2/mapdata/symbols/20x20/ball20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.7.2/mapdata/symbols/20x20/block20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.7.2/mapdata/symbols/20x20/circle20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.7.2/mapdata/symbols/20x20/q1_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.7.2/mapdata/symbols/20x20/q2_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.7.2/mapdata/symbols/20x20/q3_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.7.2/mapdata/symbols/20x20/q4_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.7.2/mapdata/symbols/20x20/square20.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/24x24/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.7.2/mapdata/symbols/24x24/ball24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.7.2/mapdata/symbols/24x24/block24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.7.2/mapdata/symbols/24x24/circle24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.7.2/mapdata/symbols/24x24/square24.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata/symbols/28x28/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.7.2/mapdata/symbols/28x28/ball28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.7.2/mapdata/symbols/28x28/block28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.7.2/mapdata/symbols/28x28/circle28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.7.2/mapdata/symbols/28x28/square28.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-29 20:15:00.630091 mapdata-3.7.2/mapdata.egg-info/
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/requires.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-05-29 20:15:00.000000 mapdata-3.7.2/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-05-29 20:15:00.634091 mapdata-3.7.2/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-05-29 19:30:39.000000 mapdata-3.7.2/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.891100 mapdata-3.8.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.8.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.8.0/MANIFEST.in
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-06-02 16:56:21.891100 mapdata-3.8.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     6421 2024-05-04 17:16:18.000000 mapdata-3.8.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.855100 mapdata-3.8.0/mapdata/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.855100 mapdata-3.8.0/mapdata/configfile/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.8.0/mapdata/configfile/mapdata.conf
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   697940 2024-06-02 16:15:53.000000 mapdata-3.8.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.855100 mapdata-3.8.0/mapdata/symbols/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.891100 mapdata-3.8.0/mapdata/symbols/16x16/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.8.0/mapdata/symbols/16x16/0.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.8.0/mapdata/symbols/16x16/1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.8.0/mapdata/symbols/16x16/2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.8.0/mapdata/symbols/16x16/3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.8.0/mapdata/symbols/16x16/4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.8.0/mapdata/symbols/16x16/5.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.8.0/mapdata/symbols/16x16/6.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.8.0/mapdata/symbols/16x16/7.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.8.0/mapdata/symbols/16x16/8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.8.0/mapdata/symbols/16x16/9.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.8.0/mapdata/symbols/16x16/A.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.8.0/mapdata/symbols/16x16/B.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.8.0/mapdata/symbols/16x16/C.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.8.0/mapdata/symbols/16x16/D.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.8.0/mapdata/symbols/16x16/E.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.8.0/mapdata/symbols/16x16/F.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.8.0/mapdata/symbols/16x16/G.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.8.0/mapdata/symbols/16x16/H.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.8.0/mapdata/symbols/16x16/I.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.8.0/mapdata/symbols/16x16/J.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.8.0/mapdata/symbols/16x16/K.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.8.0/mapdata/symbols/16x16/L.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.8.0/mapdata/symbols/16x16/M.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.8.0/mapdata/symbols/16x16/N.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.8.0/mapdata/symbols/16x16/O.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.8.0/mapdata/symbols/16x16/P.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.8.0/mapdata/symbols/16x16/Q.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.8.0/mapdata/symbols/16x16/R.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.8.0/mapdata/symbols/16x16/S.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.8.0/mapdata/symbols/16x16/T.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.8.0/mapdata/symbols/16x16/U.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.8.0/mapdata/symbols/16x16/V.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.8.0/mapdata/symbols/16x16/W.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.8.0/mapdata/symbols/16x16/X.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.8.0/mapdata/symbols/16x16/Y.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.8.0/mapdata/symbols/16x16/Z.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.8.0/mapdata/symbols/16x16/airplane.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.8.0/mapdata/symbols/16x16/anchor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.8.0/mapdata/symbols/16x16/ball.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.8.0/mapdata/symbols/16x16/ball_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.8.0/mapdata/symbols/16x16/bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.8.0/mapdata/symbols/16x16/bars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.8.0/mapdata/symbols/16x16/binoculars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.8.0/mapdata/symbols/16x16/bird.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.8.0/mapdata/symbols/16x16/block.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.8.0/mapdata/symbols/16x16/block_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.8.0/mapdata/symbols/16x16/bookmark.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.8.0/mapdata/symbols/16x16/box_stack.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.8.0/mapdata/symbols/16x16/camera.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.8.0/mapdata/symbols/16x16/cancel.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.8.0/mapdata/symbols/16x16/car.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.8.0/mapdata/symbols/16x16/car2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.8.0/mapdata/symbols/16x16/center8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.8.0/mapdata/symbols/16x16/check.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.8.0/mapdata/symbols/16x16/check_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.8.0/mapdata/symbols/16x16/checkbox.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.8.0/mapdata/symbols/16x16/checkerboard.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.8.0/mapdata/symbols/16x16/chevrons.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle_bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle_plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle_stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle_triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle_wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.8.0/mapdata/symbols/16x16/circle_x.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.8.0/mapdata/symbols/16x16/clock.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.8.0/mapdata/symbols/16x16/columns.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.8.0/mapdata/symbols/16x16/contract.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.8.0/mapdata/symbols/16x16/cross.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.8.0/mapdata/symbols/16x16/darkeye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.8.0/mapdata/symbols/16x16/decrease.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.8.0/mapdata/symbols/16x16/deposition.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.8.0/mapdata/symbols/16x16/diag_ll.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.8.0/mapdata/symbols/16x16/diag_lr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.8.0/mapdata/symbols/16x16/diag_ul.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.8.0/mapdata/symbols/16x16/diag_ur.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.8.0/mapdata/symbols/16x16/dialog.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.8.0/mapdata/symbols/16x16/diamond.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.8.0/mapdata/symbols/16x16/donkey.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.8.0/mapdata/symbols/16x16/dot.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.8.0/mapdata/symbols/16x16/down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.8.0/mapdata/symbols/16x16/drop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.8.0/mapdata/symbols/16x16/elephant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.8.0/mapdata/symbols/16x16/expand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.8.0/mapdata/symbols/16x16/eye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.8.0/mapdata/symbols/16x16/fire.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.8.0/mapdata/symbols/16x16/fish.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.8.0/mapdata/symbols/16x16/flag.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.8.0/mapdata/symbols/16x16/flag2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.8.0/mapdata/symbols/16x16/four_arrows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.8.0/mapdata/symbols/16x16/graph.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.8.0/mapdata/symbols/16x16/hand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.8.0/mapdata/symbols/16x16/hash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.8.0/mapdata/symbols/16x16/heart.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.8.0/mapdata/symbols/16x16/hidden.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.8.0/mapdata/symbols/16x16/hourglass.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.8.0/mapdata/symbols/16x16/house.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.8.0/mapdata/symbols/16x16/increase.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.8.0/mapdata/symbols/16x16/info.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.8.0/mapdata/symbols/16x16/leaf.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.8.0/mapdata/symbols/16x16/left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.8.0/mapdata/symbols/16x16/lightbulb.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.8.0/mapdata/symbols/16x16/lightning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.8.0/mapdata/symbols/16x16/lightning2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.8.0/mapdata/symbols/16x16/location_ptr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.8.0/mapdata/symbols/16x16/mine.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.8.0/mapdata/symbols/16x16/nested_boxes.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.8.0/mapdata/symbols/16x16/pennant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.8.0/mapdata/symbols/16x16/pennant2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.8.0/mapdata/symbols/16x16/people.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.8.0/mapdata/symbols/16x16/person.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.8.0/mapdata/symbols/16x16/person2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.8.0/mapdata/symbols/16x16/person3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.8.0/mapdata/symbols/16x16/phone.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.8.0/mapdata/symbols/16x16/photo.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.8.0/mapdata/symbols/16x16/picnic.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.8.0/mapdata/symbols/16x16/plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.8.0/mapdata/symbols/16x16/point_down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.8.0/mapdata/symbols/16x16/point_left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.8.0/mapdata/symbols/16x16/point_right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.8.0/mapdata/symbols/16x16/point_up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.8.0/mapdata/symbols/16x16/pointer_ne.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.8.0/mapdata/symbols/16x16/pointer_nw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.8.0/mapdata/symbols/16x16/pointer_se.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.8.0/mapdata/symbols/16x16/pointer_sw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.8.0/mapdata/symbols/16x16/puzzle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.8.0/mapdata/symbols/16x16/q1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.8.0/mapdata/symbols/16x16/q1_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.8.0/mapdata/symbols/16x16/q2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.8.0/mapdata/symbols/16x16/q2_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.8.0/mapdata/symbols/16x16/q3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.8.0/mapdata/symbols/16x16/q3_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.8.0/mapdata/symbols/16x16/q4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.8.0/mapdata/symbols/16x16/q4_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.8.0/mapdata/symbols/16x16/qmark_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.8.0/mapdata/symbols/16x16/qmark_circle2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.8.0/mapdata/symbols/16x16/raincloud.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.8.0/mapdata/symbols/16x16/right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.8.0/mapdata/symbols/16x16/rocket.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.8.0/mapdata/symbols/16x16/rocket2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.8.0/mapdata/symbols/16x16/rose.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.8.0/mapdata/symbols/16x16/rows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.8.0/mapdata/symbols/16x16/scales.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.8.0/mapdata/symbols/16x16/search.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.8.0/mapdata/symbols/16x16/search2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.8.0/mapdata/symbols/16x16/skull.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.8.0/mapdata/symbols/16x16/square.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.8.0/mapdata/symbols/16x16/star.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.8.0/mapdata/symbols/16x16/stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.8.0/mapdata/symbols/16x16/stop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.8.0/mapdata/symbols/16x16/surprise_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.8.0/mapdata/symbols/16x16/swamp.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.8.0/mapdata/symbols/16x16/target.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.8.0/mapdata/symbols/16x16/target2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.8.0/mapdata/symbols/16x16/ten.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.8.0/mapdata/symbols/16x16/trash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.8.0/mapdata/symbols/16x16/tree.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.8.0/mapdata/symbols/16x16/tree2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.8.0/mapdata/symbols/16x16/tree3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.8.0/mapdata/symbols/16x16/triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.8.0/mapdata/symbols/16x16/triangle_open.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.8.0/mapdata/symbols/16x16/triangle_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.8.0/mapdata/symbols/16x16/up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.8.0/mapdata/symbols/16x16/vapor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.8.0/mapdata/symbols/16x16/warning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.8.0/mapdata/symbols/16x16/wave.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.8.0/mapdata/symbols/16x16/wave2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.8.0/mapdata/symbols/16x16/wave3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.8.0/mapdata/symbols/16x16/weather.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.8.0/mapdata/symbols/16x16/wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.8.0/mapdata/symbols/16x16/wedge_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.8.0/mapdata/symbols/16x16/wedges_3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.8.0/mapdata/symbols/16x16/well.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.8.0/mapdata/symbols/16x16/whale.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.8.0/mapdata/symbols/16x16/whale2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.8.0/mapdata/symbols/16x16/wheelchair.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.8.0/mapdata/symbols/16x16/zigzags.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.8.0/mapdata/symbols/16x16/zigzags2.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.891100 mapdata-3.8.0/mapdata/symbols/20x20/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.8.0/mapdata/symbols/20x20/ball20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.8.0/mapdata/symbols/20x20/block20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.8.0/mapdata/symbols/20x20/circle20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.8.0/mapdata/symbols/20x20/q1_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.8.0/mapdata/symbols/20x20/q2_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.8.0/mapdata/symbols/20x20/q3_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.8.0/mapdata/symbols/20x20/q4_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.8.0/mapdata/symbols/20x20/square20.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.891100 mapdata-3.8.0/mapdata/symbols/24x24/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.8.0/mapdata/symbols/24x24/ball24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.8.0/mapdata/symbols/24x24/block24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.8.0/mapdata/symbols/24x24/circle24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.8.0/mapdata/symbols/24x24/square24.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.891100 mapdata-3.8.0/mapdata/symbols/28x28/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.8.0/mapdata/symbols/28x28/ball28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.8.0/mapdata/symbols/28x28/block28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.8.0/mapdata/symbols/28x28/circle28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.8.0/mapdata/symbols/28x28/square28.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-06-02 16:56:21.891100 mapdata-3.8.0/mapdata.egg-info/
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-06-02 16:56:21.000000 mapdata-3.8.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-06-02 16:56:21.000000 mapdata-3.8.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-06-02 16:56:21.000000 mapdata-3.8.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-06-02 16:56:21.000000 mapdata-3.8.0/mapdata.egg-info/requires.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-06-02 16:56:21.000000 mapdata-3.8.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-06-02 16:56:21.891100 mapdata-3.8.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-06-01 17:26:24.000000 mapdata-3.8.0/setup.py
```

### Comparing `mapdata-3.7.2/LICENSE.txt` & `mapdata-3.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/PKG-INFO` & `mapdata-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.7.2
+Version: 3.8.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.7.2/README.md` & `mapdata-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/configfile/mapdata.conf` & `mapdata-3.8.0/mapdata/configfile/mapdata.conf`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/mapdata.py` & `mapdata-3.8.0/mapdata/mapdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "3.7.2"
-vdate = "2024-05-29"
+version = "3.8.0"
+vdate = "2024-06-02"
 
 copyright = "2023-2024"
 
 
 import sys
 import os.path
 import io
@@ -1366,14 +1366,41 @@
 		rowdata.sort(key = lambda c: (c[sortby] is None, c[sortby]))
 	except:
 		for r in range(nrows):
 			rowdata[r][sortby] = str(rowdata[r][sortby])
 		rowdata.sort(key = lambda c: (c[sortby] == 'None', c[sortby]))
 	return [[rowdata[r][c] for r in range(nrows)] for c in range(ncols)]
 
+def check_rowtable(rowtable, headers, parent, tablename=None):
+	# Checks that every row of the table has the same number of elements as the headers.
+	# Halts with a fatal error if not.
+	n_headers = len(headers)
+	for rowno in range(len(rowtable)):
+		if len(rowtable[rowno]) != n_headers:
+			msg = tablename + ": " if tablename is not None else ""
+			msg += f"Row {rowno+1} has {len(rowtable[rowno])} columns but should have {n_headers}.\nBad row: {rowtable[rowno]}"
+			fatal_error(msg, kwargs={'parent': parent})
+
+
+def subset_by_groups(dataset, grouplist):
+	# Returns a dictionary with keys of unique elements of 'grouplist' and values
+	# corresponding elements of 'dataset'.  'dataset' is a column-oriented list of lists.
+	# The length of 'grouplist' must be the same as the lengths of the lists in 'dataset'--this is not checked.
+	groups = list(set(grouplist))
+	ncols = len(dataset)
+	grp_datasets = {}
+	for g in groups:
+		grp_datasets[g] = [[] for _ in range(ncols)]
+	for r in range(len(dataset[0])):
+		g = grouplist[r]
+		for col in range(ncols):
+			grp_datasets[g][col].append(dataset[col][r])
+	return grp_datasets
+
+
 def treeview_sort_column(tv, col, reverse):
     colvals = [(tv.set(k, col), k) for k in tv.get_children()]
     try:
     	colvals.sort(key=lambda v: float(v[0]), reverse=reverse)
     except ValueError:
     	colvals.sort(reverse=reverse)
     # Rearrange items in sorted positions
@@ -1402,18 +1429,21 @@
 	# This does not grid the table frame in its parent widget.
 	# Returns a tuple of 0: the frame containing the table,  and 1: the table widget itself.
 	nrows = range(len(rowset))
 	ncols = range(len(column_headers))
 	hdrwidths = [len(column_headers[j]) for j in ncols]
 	if len(rowset) > 0:
 		datawidthtbl = [[len(rowset[i][j] if isinstance(rowset[i][j], str) else str(rowset[i][j])) for i in nrows] for j in ncols]
+		#datawidthtbl = [[len(str(rowset[i][j])) for i in nrows] for j in ncols]
 		datawidths = [max(cwidths) for cwidths in datawidthtbl]
+		colwidths = [max(hdrwidths[i], datawidths[i]) for i in ncols]
 	else:
-		datawidths = hdrwidths
-	colwidths = [max(hdrwidths[i], datawidths[i]) for i in ncols]
+		#datawidths = hdrwidths
+		colwidths = hdrwidths
+	#colwidths = [max(hdrwidths[i], datawidths[i]) for i in ncols]
 	# Set the font.
 	ff = tkfont.nametofont("TkFixedFont")
 	tblstyle = ttk.Style()
 	tblstyle.configure('tblstyle', font=ff)
 	charpixels = int(1.3 * ff.measure(u"0"))
 	tableframe = ttk.Frame(master=parent, padding="3 3 3 3")
 	statusframe = ttk.Frame(master=tableframe)
@@ -7257,14 +7287,16 @@
 		self.dlg.rowconfigure(3, weight=0)
 		self.dlg.columnconfigure(0, weight=1)
 		# Data
 		self.dataset = None
 		self.data_labels = None
 		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
 		self.numeric_columns.sort()
+		self.categ_columns = [c[0] for c in self.column_specs if c[1] in ("string", "boolean")]
+		self.categ_columns.sort()
 		self.dnames = ["Variable", " N ", "Min.", "Max.", "Mean", "Median", "Mode", \
 				"Geo. mean", "Std.Dev.", "C.V.", "Sum", "5th %ile", "95th %ile", "Anderson-Darling p", \
 				"Lillefors p", "Rosner's outliers", "Tukey outliers"]
 		self.logdnames = ["Variable", " N ", "Min.", "Max.", "Mean", "Median", "Mode", \
 				"Std.Dev.", "C.V.", "Sum", "5th %ile", "95th %ile", "Anderson-Darling p", "Lillefors p", \
 				"Rosner's outliers", "Tukey outliers"]
 		self.statdata = []
@@ -7307,14 +7339,23 @@
 		frame_panes.add(var_frame, weight=1)
 		# Add multi-select list of variables to the leftmost pane
 		self.column_frame, self.column_table = treeview_table(var_frame, rowset=[[v] for v in self.numeric_columns], \
 				column_headers=['Variable'], select_mode=tk.EXTENDED, nrows=min(10, len(self.numeric_columns)))
 		self.column_frame.grid(row=0, column=0, sticky=tk.NSEW)
 		self.column_table.bind('<ButtonRelease-1>', self.q_recalc)
 
+		# Add an optional 'group by' variable selection
+		self.groupby_var = tk.StringVar(var_frame, "")
+		groupby_lbl = ttk.Label(var_frame, text="Group by:")
+		groupby_lbl.grid(row=1, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.groupby_sel = ttk.Combobox(var_frame, state="readonly", textvariable=self.groupby_var, 
+				values= [''] + self.categ_columns, width=24)
+		self.groupby_sel.grid(row=2, column=0, sticky=tk.W, padx=(12,3), pady=(3,3))
+		self.groupby_sel.bind("<<ComboboxSelected>>", self.q_recalc)
+
 		# Content frame for output.  This contains a tabbed Notebook widget,
 		# with separate pages for statistics of untransformed and log-transformed data.
 		self.content_frame = tk.Frame(frame_panes, borderwidth=3, relief=tk.RIDGE)
 		self.content_frame.grid(row=0, column=1, sticky=tk.NSEW)
 		self.content_frame.rowconfigure(0, weight=1)
 		self.content_frame.columnconfigure(0, weight=1)
 		frame_panes.add(self.content_frame, weight=12)
@@ -7330,15 +7371,15 @@
 		self.log_page.columnconfigure(0, weight=1)
 		self.data_page.grid(row=0, column=0, sticky=tk.NSEW)
 		self.log_page.grid(row=0, column=0, sticky=tk.NSEW)
 		output_pages.add(self.data_page, text="Untransformed")
 		output_pages.add(self.log_page, text="Log-transformed")
 
 		# initialize content frame with headings, no data
-		self.recalc()
+		self.clear_output()
 
 		# Buttons
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=0)
 		btn_frame.columnconfigure(1, weight=1)
@@ -7354,32 +7395,36 @@
 		self.dlg.bind("<Escape>", self.do_close)
 		center_window(self.dlg)
 		raise_window(self.dlg)
 
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#univariate-statistics-dialog", new=2, autoraise=True)
 
-	def q_recalc(self, get_data=True, *args):
-		if self.dataset is None or get_data:
+	def q_recalc(self, *args):
+		if len(self.column_table.selection()) > 0:
 			self.clear_output()
 			self.get_data()
-		if self.dataset is not None and len(self.dataset[0]) > 1:
+		if self.dataset is not None and len(self.dataset[0]) > 0:
 			self.data_btn["state"] = tk.NORMAL
 			self.recalc()
 		else:
 			self.data_btn["state"] = tk.DISABLED
 
 	def get_data(self):
 		# Get the selected data into 'dataset'
 		self.dataset = None
+		self.n_dataset_columns = 0
 		column_list = []
 		for sel_row in self.column_table.selection():
 			datarow = self.column_table.item(sel_row)["values"]
 			column_list.append(datarow[0])
 		if len(column_list) > 0:
+			self.n_dataset_columns = len(column_list)
+			if self.groupby_var.get() != "":
+				column_list.append(self.groupby_var.get())
 			# Get either only the selected data or all data.
 			if self.sel_only_var.get() == "1":
 				dataset = self.parent.get_sel_data(column_list)
 			else:
 				dataset = self.parent.get_all_data(column_list)
 			if dataset is None or len(dataset[0]) == 0:
 				self.dataset = None
@@ -7389,184 +7434,150 @@
 				self.data_labels = column_list
 
 	def show_data(self, *args):
 		if self.dataset is not None:
 			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels[0:len(self.dataset)], \
 					"Data for univariate stats")
 
+	def univar_stats(self, dlist):
+		# Return the univariate statistics for the data values in 'dlist' and for log-transformed versions of those.
+		# The geometric mean is returned only for the untransformed data.
+		#
+		def stats(d, meanlog, do_geomean=False):
+			mean_d = statistics.fmean(d)
+			if len(d) > 1:
+				stdev_d = statistics.stdev(d)
+			else:
+				stdev_d = 0.0
+			dd = [len(d), min(d), max(d), fp_display(mean_d, 4)]
+			if len(d) > 1:
+				dd.extend([fp_display(statistics.median(d), 4), statistics.mode(d)])
+			else:
+				dd.extend([None, None])
+			# Geo. mean
+			if do_geomean:
+				dd.append(fp_display(10**meanlog, 4))
+			if len(d) > 1:
+				# Std. dev.
+				dd.append(fp_display(stdev_d, 4))
+				# Coefficient of variation
+				dd.append(fp_display(stdev_d/mean_d, 4))
+			else:
+				dd.extend([None, None])
+			# Sum
+			dd.append(sum(d))
+			# Percentiles
+			if len(d) > 4:
+				dd.extend([fp_display(np.percentile(d, 5)), fp_display(np.percentile(d, 95))])
+			else:
+				dd.extend(["NC", "NC"])
+			#=== Normality tests
+			if len(d) > 4:
+				da = np.array(d)
+				normstats = []
+				if stdev_d != 0.0:
+					try:
+						adval, adpval = normal_ad(da)
+						normstats.append("%.2E" % adpval)
+					except:
+						normstats.append("NC")
+					try:
+						lfval, lfpval = kstest_normal(da)
+						normstats.append("%.2E" % lfpval)
+					except:
+						normstats.append("NC")
+				else:
+					normstats = ["NC", "NC"]
+				dd.extend(normstats)
+			else:
+				dd.extend([None, None])
+			#=== Outlier evaluation
+			if len(d) > 14:
+				if stdev_d > 0.0:
+					max_outliers = 5 if len(d) < 100 else 10
+					try:
+						dd.append(rosners_test(d, 0.05, max_outliers))
+					except:
+						dd.append("NC")
+				else:
+					dd.append("NC")
+			else:
+				dd.append("NC")
+			if len(d) > 5:
+				dd.append(tukey_outliers(d))
+			else:
+				dd.append("NC")
+			return dd
+		#
+		ds = [float(dv) for dv in dlist if dv is not None and not (type(dv) == type('') and dv.strip()=='')]
+		if len(ds) == 0:
+			return [0], [0]
+		logd = []
+		log_error = False
+		for w in range(len(ds)):
+			try:
+				logd.append(math.log10(ds[w]))
+			except:
+				log_error = True
+				break
+		if len(logd) > 0:
+			meanlog = statistics.fmean(logd)
+		else:
+			meanlog = None
+		normstats = stats(ds, meanlog, do_geomean=True)
+		logstats = stats(logd, meanlog, do_geomean=False)
+		return normstats, logstats
+	
+
 	def recalc(self):
 		# Calculate and display statistics for each selected column.
 		for ctl in self.data_page.winfo_children():
 			ctl.destroy()
 		for ctl in self.log_page.winfo_children():
 			ctl.destroy()
 		self.statdata = []
 		self.logstatdata = []
 		if self.data_labels is not None:
-			for i in range(len(self.data_labels)):
-				d = [float(dv) for dv in self.dataset[i] if dv is not None and not (type(dv) == type('') and dv.strip()=='')]
-				logd = []
-				if len(d) > 0:
-					log_error = False
-					for w in range(len(d)):
-						try:
-							logd.append(math.log10(d[w]))
-						except:
-							log_error = True
-							break
-					if log_error:
-						logd = []
-					if len(logd) > 0:
-						meanlog = statistics.fmean(logd)
-					#=== Descriptive statistics for untransformed data
-					mean_d = statistics.fmean(d)
-					dd = [self.data_labels[i], len(d), min(d), max(d), fp_display(mean_d, 4)]
-					stdev_d = statistics.stdev(d)
-					if len(d) > 1:
-						dd.extend([fp_display(statistics.median(d), 4), statistics.mode(d)])
-					else:
-						dd.extend([None, None])
-					# Geo. mean
-					if len(logd) > 0:
-						dd.append(fp_display(10**meanlog, 4))
-					else:
-						dd.append(None)
-					# Std. dev.
-					if len(d) > 1:
-						dd.append(fp_display(stdev_d, 4))
-					else:
-						dd.append(None)
-					# Coefficient of variation
-					if len(d) > 1:
-						dd.append(fp_display(stdev_d/mean_d, 4))
-					else:
-						dd.append(None)
-					# Sum
-					dd.append(sum(d))
-					# Percentiles
-					if len(d) > 4:
-						dd.extend([fp_display(np.percentile(d, 5)), fp_display(np.percentile(d, 95))])
-					else:
-						dd.extend(["NC", "NC"])
-					#=== Normality tests for untransformed data
-					if len(d) > 4:
-						da = np.array(d)
-						normstats = []
-						if stdev_d != 0.0:
-							try:
-								adval, adpval = normal_ad(da)
-								normstats.append("%.2E" % adpval)
-							except:
-								normstats.append("NC")
-							try:
-								lfval, lfpval = kstest_normal(da)
-								normstats.append("%.2E" % lfpval)
-							except:
-								normstats.append("NC")
-						else:
-							normstats = ["NC", "NC"]
-						dd.extend(normstats)
-					else:
-						dd.extend([None, None])
-					#=== Outlier evaluation for untransformed data
-					if len(d) > 14:
-						max_outliers = 5 if len(d) < 100 else 10
-						try:
-							# May be ZeroDivisionError if sd == 0
-							dd.append(rosners_test(d, 0.05, max_outliers))
-						except:
-							dd.append("NC")
-					else:
-						dd.append(None)
-					if len(d) > 5:
-						dd.append(tukey_outliers(d))
-					else:
-						dd.append("NC")
-					#
-					#=== Descriptive statistics for log-transformed data
-					logdd = [self.data_labels[i], len(logd)]
-					if len(logd) > 0:
-						mean_dd = statistics.fmean(logd)
-						logdd.extend([fp_display(min(logd),4), fp_display(max(logd),4), fp_display(mean_dd, 4)])
-					else:
-						logdd.extend([None, None, None])
-					if len(logd) > 1:
-						logdd.extend([fp_display(statistics.median(logd), 4), statistics.mode(logd)])
-					else:
-						logdd.extend([None, None])
-					if len(logd) > 1:
-						stdevlog = statistics.stdev(logd)
-						logdd.append(fp_display(stdevlog, 4))
-					else:
-						logdd.append(None)
-					# Coefficient of variation
-					if len(logd) > 1:
-						logdd.append(fp_display(stdevlog/mean_dd, 4))
-					else:
-						logdd.append(None)
-					# Sum
-					logdd.append(sum(logd))
-					# Percentiles
-					if len(logd) > 4:
-						logdd.extend([fp_display(np.percentile(logd, 5)), fp_display(np.percentile(logd, 95))])
-					else:
-						logdd.extend(["NC", "NC"])
-					# Normality tests for log-transformed data
-					if len(logd) > 4:
-						logda = np.array(logd)
-						lognormstats = []
-						if stdevlog != 0.0:
-							try:
-								adval, adpval = normal_ad(logda)
-								lognormstats.append("%.2E" % adpval)
-							except:
-								normstats.append("NC")
-							try:
-								lfval, lfpval = kstest_normal(logda)
-								lognormstats.append("%.2E" % lfpval)
-							except:
-								lognormstats.append("NC")
-						else:
-							lognormstats = ["NC", "NC"]
-						logdd.extend(lognormstats)
-					else:
-						logdd.extend([None, None])
-					# Outlier evaluation for log-transformed data
-					if len(logd) > 14:
-						max_outliers = 5 if len(logd) < 100 else 10
-						try:
-							# May be ZeroDivisionError if sd == 0
-							logdd.append(rosners_test(logd, 0.05, max_outliers))
-						except:
-							logdd.append("NC")
-					else:
-						logdd.append(None)
-					if len(logd) > 5:
-						logdd.append(tukey_outliers(logd))
-					else:
-						logdd.append("NC")
-					self.statdata.append(dd)
-					self.logstatdata.append(logdd)
-		#if len(self.statdata) > 0:
-		tframe, tdata = treeview_table(self.data_page, self.statdata, self.dnames)
+			if self.groupby_var.get() == "":
+				for var in range(self.n_dataset_columns):
+					vardata = self.dataset[var]
+					if len(vardata) > 0 and not (len(vardata) == 1 and (vardata[0] is None or vardata[0] == '')):
+						dd, logdd = self.univar_stats(self.dataset[var])
+						self.statdata.append([self.data_labels[var]] + dd)
+						self.logstatdata.append([self.data_labels[var]] + logdd)
+				dnames = self.dnames
+				logdnames = self.logdnames
+			else:
+				datasetdict = subset_by_groups(self.dataset[0:self.n_dataset_columns], self.dataset[self.n_dataset_columns])
+				for grp in datasetdict.keys():
+					ds = datasetdict[grp]
+					for var in range(self.n_dataset_columns):
+						vardata = ds[var]
+						if len(vardata) > 0 and not (len(vardata) == 1 and (vardata[0] is None or vardata[0] == '')):
+							dd, logdd = self.univar_stats(vardata)
+							self.statdata.append([grp, self.data_labels[var]] + dd)
+							self.logstatdata.append([grp, self.data_labels[var]] + logdd)
+				dnames = ["Group"] + self.dnames
+				logdnames = ["Group"] + self.logdnames
+		tframe, tdata = treeview_table(self.data_page, self.statdata, dnames)
 		tframe.grid(row=0, column=0, sticky=tk.NSEW)
-		ltframe, ltdata = treeview_table(self.log_page, self.logstatdata, self.logdnames)
+		ltframe, ltdata = treeview_table(self.log_page, self.logstatdata, logdnames)
 		ltframe.grid(row=0, column=0, sticky=tk.NSEW)
 		self.dlg.bind("<Control-s>", self.save_data)
 		self.dlg.bind("<Control-z>", self.save_logdata)
 
 	def clear_output(self):
 		for ctl in self.data_page.winfo_children():
 			ctl.destroy()
 		for ctl in self.log_page.winfo_children():
 			ctl.destroy()
 		self.dlg.bind("<Control-s>")
 		self.dlg.bind("<Control-z>")
 		self.dataset = None
-		tframe, tdata = treeview_table(self.log_page, [], self.dnames)
+		tframe, tdata = treeview_table(self.data_page, [], self.dnames)
 		tframe.grid(row=0, column=0, sticky=tk.NSEW)
 		ltframe, ltdata = treeview_table(self.log_page, [], self.logdnames)
 		ltframe.grid(row=0, column=0, sticky=tk.NSEW)
 	def save_data(self, *args):
 		export_data_table(self.dnames, self.statdata, sheetname="Stats for untransformed data")
 	def save_logdata(self, *args):
 		export_data_table(self.logdnames, self.logstatdata, sheetname="Stats for log-transformed data")
@@ -8323,23 +8334,35 @@
 		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
 
 		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
 		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
 				onvalue="1", offvalue="0")
 		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 
+		# Dropdown for missing data treatment
 		cleantype_frame = tk.Frame(ctrl_frame)
 		cleantype_frame.grid(row=1, column=0, columnspan=2, sticky=tk.NSEW)
-		self.cleantype_var = tk.StringVar(cleantype_frame, "Variables")
-		ttk.Label(cleantype_frame, text="Remove missing values by").grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
-		self.cleantype_sel = ttk.Combobox(cleantype_frame, state=tk.NORMAL, textvariable=self.cleantype_var, values=["Cases","Variables"], width=10)
+		self.cleantype_var = tk.StringVar(cleantype_frame, "Drop variables")
+		ttk.Label(cleantype_frame, text="Remove missing values by:").grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.cleantype_sel = ttk.Combobox(cleantype_frame, state=tk.NORMAL, textvariable=self.cleantype_var, values=["Drop cases","Drop variables", "Set to zero"], width=14)
 		self.cleantype_sel.bind('<<ComboboxSelected>>', self.q_recalc)
 		self.cleantype_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
 		cleantype_frame.columnconfigure(1, weight=1)
 
+		# Dropdown for standardization
+		stdize_frame = tk.Frame(ctrl_frame)
+		stdize_frame.grid(row=1, column=2, sticky=tk.NSEW)
+		stdize_opts = ["", "Z score by variable", "L1 norm by case"]
+		self.stdize_var = tk.StringVar(stdize_frame, stdize_opts[1])
+		ttk.Label(stdize_frame, text="Standardization:").grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.stdize_sel = ttk.Combobox(stdize_frame, state=tk.NORMAL, textvariable=self.stdize_var, values=stdize_opts, width=20)
+		self.stdize_sel.bind('<<ComboboxSelected>>', self.q_recalc)
+		self.stdize_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		stdize_frame.columnconfigure(1, weight=1)
+
 		# Frame for input selection and output plot
 		self.content_frame = tk.Frame(self.dlg)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
 		self.content_frame.columnconfigure(0, weight=1)
@@ -8497,50 +8520,59 @@
 			self.data_rowids = self.parent.get_all_rowids()
 		if dataset is None or len(dataset[0]) < 6:
 			self.dataset = None
 			self.data_labels = None
 			self.data_btn["state"] = tk.DISABLED
 			self.calc_btn["state"] = tk.DISABLED
 		else:
-			# Remove missing data, either by variables or cases.  This may lead to eliminating the data set.
-			if self.cleantype_var.get() == "Cases":
-				column_indexes = range(len(dataset))
-				clean_data = [[] for _ in dataset]
-				clean_rowids = []
-				for i in range(len(dataset[0])):
-					ok = True
-					for col in column_indexes:
-						if dataset[col][i] is None or dataset[col][i] == '':
-							ok = False
-					if ok:
-						for col in column_indexes:
-							clean_data[col].append(dataset[col][i])
-						clean_rowids.append(self.data_rowids[i])
-				self.data_rowids = clean_rowids
-				dataset = clean_data
-			else:
+			# t-SNE can operate on sparse arrays, so missing values may be converted to zero or removed.
+			if self.cleantype_var.get() == "Set to zero":
+				for col in range(self.n_dataset_columns):
+					for row in range(len(dataset[0])):
+						if dataset[col][row] is None:
+							dataset[col][row] = 0
+			elif self.cleantype_var.get() == "Drop variables":
+				# Remove columns with missing data.  This may remove all columns.
 				badcols = []
 				for col in range(self.n_dataset_columns):
 					if not all(dataset[col]):
 						badcols.append(col)
 				if len(badcols) > 0:
 					badcols.reverse()
 					for bc in badcols:
 						del dataset[bc]
 						del column_list[bc]
 						if self.label_col is not None:
 							self.label_col -= 1
 					if self.groupby_col is not None:
 						self.groupby_col = len(column_list)
 					self.n_dataset_columns = self.n_dataset_columns - len(badcols)
+			elif self.cleantype_var.get() == "Drop rows" and self.n_dataset_columns > 0:
+				# Remove rows with missing data.  This may remove all rows.
+				column_indexes = range(self.n_dataset_columns)
+				clean_data = [[] for _ in dataset]
+				clean_rowids = []
+				for i in range(len(dataset[0])):
+					ok = True
+					for col in column_indexes:
+						if dataset[col][i] is None or dataset[col][i] == '':
+							ok = False
+					if ok:
+						for col in range(len(dataset)):
+							clean_data[col].append(dataset[col][i])
+						clean_rowids.append(self.data_rowids[i])
+				self.data_rowids = clean_rowids
+				dataset = clean_data
+
 			if dataset is not None and len(dataset) > 0 and self.n_dataset_columns > 0:
 				# Convert to floats for numeric data only
 				for i in range(self.n_dataset_columns):
 					if column_list[i] in self.numeric_columns:
 						dataset[i] = [conv_float(v) for v in dataset[i]]
+
 			if dataset is None or self.n_dataset_columns < 3 or len(dataset[0]) < 6:
 				self.dataset = None
 				self.data_labels = None
 				self.data_btn["state"] = tk.DISABLED
 				self.calc_btn["state"] = tk.DISABLED
 				self.loading_dlg.hide()
 				warning("The dataset must have at least 3 variables and 6 cases for t-SNE analysis", {'parent':self.dlg})
@@ -8562,27 +8594,56 @@
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.draw()
 
 	def recalculate(self):
 		self.loading_dlg.display("Calculating t-SNE")
 		self.clear_output()
 		from sklearn.manifold import TSNE
+		from sklearn.preprocessing import Normalizer, StandardScaler
 		self.get_data()
 		if self.dataset is not None and len(self.dataset[0]) > 5:
-			d = np.array(columns_to_rows(self.dataset[0:self.n_dataset_columns]))
+			# Check to see if this is a sparse matrix
+			ds = copy.copy(self.dataset[0:self.n_dataset_columns])
+			is_sparse = False
+			for col in range(len(ds)):
+				if any([x is None for x in ds[col]]):
+					is_sparse = True
+					break
+			if is_sparse:
+				# Replace all None with 0
+				for col in range(len(ds)):
+					ds[col] = [0.0 if x is None else x for x in ds[col]]
+			dsa = np.array(columns_to_rows(ds), dtype=float)
+			if is_sparse:
+				dsa = sparse.csr_matrix(dsa)
+				tsne_init = 'random'
+			else:
+				tsne_init = 'pca'
+			# Maybe transform
+			if self.stdize_var.get() == "L1 norm by case":
+				inp_data = Normalizer(norm='l1').fit_transform(dsa)
+			elif self.stdize_var.get() == "Z score by variable":
+				if is_sparse:
+					inp_data = StandardScaler(with_mean=False).fit_transform(dsa)
+				else:
+					inp_data = StandardScaler().fit_transform(dsa)
+			else:
+				inp_data = dsa
+			# Calculate t-SNE
 			perp = self.perp_var.get()
 			if perp > len(self.dataset[0]) - 1:
 				perp = min(50, math.floor(len(self.dataset[0])/2))
 				self.perp_var.set(perp)
-			tsne = TSNE(n_components=2, perplexity=perp)
-			tsne_result = tsne.fit_transform(d)
+			tsne = TSNE(n_components=2, perplexity=perp, init=tsne_init)
+			tsne_result = tsne.fit_transform(inp_data)
+			# Get data for output table
 			self.tsne_coords = [tsne_result[:,0], tsne_result[:,1]]
 			self.tsne_labels = ["Dimension 1", "Dimension 2"]
 			self.dtable_btn["state"] = tk.NORMAL
-			# Single or grouped scatter plot
+			# Create a single or grouped scatter plot
 			if self.groupby_col is None:
 				splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
 				self.plot_handle_list = []
 				self.plot_label_list = []
 			else:
 				groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
 				cmap = map_colors(groups)
@@ -8637,40 +8698,41 @@
 			self.clust_save_btn["state"] = tk.DISABLED
 			self.loading_dlg.hide()
 
 	def kclusters(self):
 		# Compute and display k-means clusters
 		dlg = OneIntDialog(self.dlg, "k-Means Clusters", "Enter the number of clusters to identify", min_value=2, max_value=min(30, len(self.dataset[0])-1), initial=2)
 		num_clusters = dlg.show()
-		self.loading_dlg.display("Clustering t-SNE output")
-		from sklearn.cluster import KMeans
-		km = KMeans(n_clusters=num_clusters)
-		km.fit(np.array(columns_to_rows([self.tsne_coords[0], self.tsne_coords[1]])))
-		self.kmlabels = ["Cluster "+str(int(lbl)+1) for lbl in km.labels_]
-		self.tsne_coords.append(self.kmlabels)
-		self.tsne_labels.append("k-Means cluster")
-		kgroups = sorted([str(x) for x in list(set(self.kmlabels))])
-		kcmap = map_colors(kgroups)
-		kcolors = [kcmap[str(g)] for g in self.kmlabels]
-		self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], marker="v", s=15, c=kcolors)
-		klbls = [str(k) for k in kcmap.keys()]
-		kcolkey = list(kcmap.values())
-		ksymbs = [matplotlib.lines.Line2D([], [], marker='v', color=kcolkey[i], label=klbls[i], linestyle='None') for i in range(len(klbls))]
-		self.plot_handle_list.extend(ksymbs)
-		self.plot_label_list.extend(klbls)
-		try:
-			self.plot_axes.get_legend().remove()
-		except:
-			pass
-		self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
-		self.plotfig_canvas.draw()
-		# Only allow creation of one set of clusters for each UMAP output.
-		self.cluster_btn["state"] = tk.DISABLED
-		self.clust_save_btn["state"] = tk.NORMAL
-		self.loading_dlg.hide()
+		if num_clusters is not None:
+			self.loading_dlg.display("Clustering t-SNE output")
+			from sklearn.cluster import KMeans
+			km = KMeans(n_clusters=num_clusters)
+			km.fit(np.array(columns_to_rows([self.tsne_coords[0], self.tsne_coords[1]])))
+			self.kmlabels = ["Cluster "+str(int(lbl)+1) for lbl in km.labels_]
+			self.tsne_coords.append(self.kmlabels)
+			self.tsne_labels.append("k-Means cluster")
+			kgroups = sorted([str(x) for x in list(set(self.kmlabels))])
+			kcmap = map_colors(kgroups)
+			kcolors = [kcmap[str(g)] for g in self.kmlabels]
+			self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], marker="v", s=15, c=kcolors)
+			klbls = [str(k) for k in kcmap.keys()]
+			kcolkey = list(kcmap.values())
+			ksymbs = [matplotlib.lines.Line2D([], [], marker='v', color=kcolkey[i], label=klbls[i], linestyle='None') for i in range(len(klbls))]
+			self.plot_handle_list.extend(ksymbs)
+			self.plot_label_list.extend(klbls)
+			try:
+				self.plot_axes.get_legend().remove()
+			except:
+				pass
+			self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
+			self.plotfig_canvas.draw()
+			# Only allow creation of one set of clusters for each t-SNE output.
+			self.cluster_btn["state"] = tk.DISABLED
+			self.clust_save_btn["state"] = tk.NORMAL
+			self.loading_dlg.hide()
 
 	def kcolumn(self):
 		# Save k-means cluster output as a data table column.
 		# Column selection
 		dlg = CustomContentDialog(parent=self.dlg, title="Save Clusters", prompt="Save k-means clusters in a table column.")
 		def ck_col_name(varname, ix, mode):
 			if self.col_var.get() in self.prohibited_columns:
@@ -8796,30 +8858,41 @@
 		# Controls
 		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
 		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
 
 		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
 		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_recalc, variable=self.sel_only_var,
 				onvalue="1", offvalue="0")
-		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(2,2))
 
 		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
 		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
 				onvalue="1", offvalue="0")
-		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(2,2))
 
-		self.compvars_var = tk.StringVar(ctrl_frame, "0")
-		self.compvars_ck = ttk.Checkbutton(ctrl_frame, text="Complete variables only", command=self.q_recalc, variable=self.compvars_var,
-				onvalue="1", offvalue="0")
-		self.compvars_ck.grid(row=1, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		# Dropdown for missing data treatment
+		cleantype_frame = tk.Frame(ctrl_frame)
+		cleantype_frame.grid(row=1, column=0, columnspan=2, sticky=tk.NSEW)
+		self.cleantype_var = tk.StringVar(cleantype_frame, "Drop variables")
+		ttk.Label(cleantype_frame, text="Remove missing values by:").grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.cleantype_sel = ttk.Combobox(cleantype_frame, state=tk.NORMAL, textvariable=self.cleantype_var, values=["Drop cases","Drop variables", "Set to zero"], width=14)
+		self.cleantype_sel.bind('<<ComboboxSelected>>', self.q_recalc)
+		self.cleantype_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		cleantype_frame.columnconfigure(1, weight=1)
 
-		self.compcases_var = tk.StringVar(ctrl_frame, "0")
-		self.compcases_ck = ttk.Checkbutton(ctrl_frame, text="Complete cases only", command=self.q_recalc, variable=self.compcases_var,
-				onvalue="1", offvalue="0")
-		self.compcases_ck.grid(row=1, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		# Dropdown for standardization
+		stdize_frame = tk.Frame(ctrl_frame)
+		stdize_frame.grid(row=1, column=2, columnspan=2, sticky=tk.NSEW)
+		stdize_opts = ["", "Z score by variable", "L1 norm by case"]
+		self.stdize_var = tk.StringVar(stdize_frame, stdize_opts[1])
+		ttk.Label(stdize_frame, text="Standardization:").grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.stdize_sel = ttk.Combobox(stdize_frame, state=tk.NORMAL, textvariable=self.stdize_var, values=stdize_opts, width=20)
+		self.stdize_sel.bind('<<ComboboxSelected>>', self.q_recalc)
+		self.stdize_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(2,2))
+		stdize_frame.columnconfigure(1, weight=1)
 
 		# Frame for input selection and output plot
 		self.content_frame = tk.Frame(self.dlg)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
@@ -8982,15 +9055,20 @@
 			dataset = self.parent.get_sel_data(column_list)
 			self.data_rowids = self.parent.get_sel_rowids()
 		else:
 			dataset = self.parent.get_all_data(column_list)
 			self.data_rowids = self.parent.get_all_rowids()
 		if dataset is not None:
 			# UMAP can operate on sparse arrays, so removal of missing data is optional
-			if self.compvars_var.get() == "1":
+			if self.cleantype_var.get() == "Set to zero":
+				for col in range(self.n_dataset_columns):
+					for row in range(len(dataset[0])):
+						if dataset[col][row] is None:
+							dataset[col][row] = 0
+			elif self.cleantype_var.get() == "Drop variables":
 				# Remove columns with missing data.  This may remove all columns.
 				badcols = []
 				for col in range(self.n_dataset_columns):
 					if not all(dataset[col]):
 						badcols.append(col)
 				if len(badcols) > 0:
 					badcols.reverse()
@@ -8998,15 +9076,15 @@
 						del dataset[bc]
 						del column_list[bc]
 						if self.label_col is not None:
 							self.label_col -= 1
 					if self.groupby_col is not None:
 						self.groupby_col = len(column_list)
 					self.n_dataset_columns = self.n_dataset_columns - len(badcols)
-			if self.compcases_var.get() == "1" and self.n_dataset_columns > 0:
+			elif self.cleantype_var.get() == "Drop rows" and self.n_dataset_columns > 0:
 				# Remove rows with missing data.  This may remove all rows.
 				column_indexes = range(self.n_dataset_columns)
 				clean_data = [[] for _ in dataset]
 				clean_rowids = []
 				for i in range(len(dataset[0])):
 					ok = True
 					for col in column_indexes:
@@ -9014,19 +9092,21 @@
 							ok = False
 					if ok:
 						for col in range(len(dataset)):
 							clean_data[col].append(dataset[col][i])
 						clean_rowids.append(self.data_rowids[i])
 				self.data_rowids = clean_rowids
 				dataset = clean_data
-			if dataset is not None and len(dataset) > 0 and self.n_dataset_columns > 0:
-				# Convert to floats for numeric data only
-				for i in range(self.n_dataset_columns):
-					if column_list[i] in self.numeric_columns:
-						dataset[i] = [conv_float(v) for v in dataset[i]]
+
+		if dataset is not None and len(dataset) > 0 and self.n_dataset_columns > 0:
+			# Convert to floats for numeric data only
+			for i in range(self.n_dataset_columns):
+				if column_list[i] in self.numeric_columns:
+					dataset[i] = [conv_float(v) for v in dataset[i]]
+
 		if dataset is None or self.n_dataset_columns < 3 or len(dataset[0]) < 6:
 			self.dataset = None
 			self.data_labels = None
 			self.data_btn["state"] = tk.DISABLED
 			self.calc_btn["state"] = tk.DISABLED
 			self.loading_dlg.hide()
 			warning("The dataset must have at least 3 variables and 6 cases for UMAP analysis", {'parent':self.dlg})
@@ -9046,41 +9126,44 @@
 		self.plotfig.clear()
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.draw()
 
 	def recalculate(self):
 		self.loading_dlg.display("Calculating UMAP")
 		import umap
-		from sklearn.preprocessing import StandardScaler
+		from sklearn.preprocessing import Normalizer, StandardScaler
 		self.clear_output()
 		self.get_data()
 		if self.dataset is not None and len(self.dataset[0]) > 5:
 			# Check to see if this is a sparse matrix
+			ds = copy.copy(self.dataset[0:self.n_dataset_columns])
 			is_sparse = False
-			for col in range(self.n_dataset_columns):
-				#if any([x is None or x == 0.0 for x in self.dataset[col]]):
-				if any([x is None for x in self.dataset[col]]):
+			for col in range(len(ds)):
+				if any([x is None for x in ds[col]]):
 					is_sparse = True
 					break
-			ds = copy.copy(self.dataset[0:self.n_dataset_columns])
 			if is_sparse:
 				# Replace all None with 0
 				for col in range(len(ds)):
 					ds[col] = [0.0 if x is None else x for x in ds[col]]
 			dsa = np.array(columns_to_rows(ds), dtype=float)
 			if is_sparse:
-				# Convert to a LIL array
-				dsm = sparse.lil_matrix(dsa)
-				# Normalize the variables
-				inp_data = StandardScaler(with_mean=False).fit_transform(dsm)
-			else:
-				# Normalize the variables
-				inp_data = StandardScaler().fit_transform(dsa)
-			reducer = umap.UMAP(n_neighbors=min(self.neighbors_var.get(), len(self.dataset[0])-1), min_dist=self.mindist_var.get(), n_components=2,
-					metric=self.metric_var.get())
+				dsa = sparse.csr_matrix(dsa)
+			# Maybe transform
+			if self.stdize_var.get() == "L1 norm by case":
+				inp_data = Normalizer(norm='l1').fit_transform(dsa)
+			elif self.stdize_var.get() == "Z score by variable":
+				if is_sparse:
+					inp_data = StandardScaler(with_mean=False).fit_transform(dsa)
+				else:
+					inp_data = StandardScaler().fit_transform(dsa)
+			else:
+				inp_data = dsa
+			reducer = umap.UMAP(n_neighbors=min(self.neighbors_var.get(), len(self.dataset[0])-1),
+					min_dist=self.mindist_var.get(), n_components=2, metric=self.metric_var.get())
 			umap_result = reducer.fit_transform(inp_data)
 			self.umap_coords = [umap_result[:,0], umap_result[:,1]]
 			self.umap_labels = ["Dimension 1", "Dimension 2"]
 			self.dtable_btn["state"] = tk.NORMAL
 			# Single or grouped scatter plot
 			if self.groupby_col is None:
 				splot = self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], alpha=self.alpha)
@@ -9140,40 +9223,41 @@
 			self.clust_save_btn["state"] = tk.DISABLED
 			self.loading_dlg.hide()
 
 	def kclusters(self):
 		# Compute and display k-means clusters
 		dlg = OneIntDialog(self.dlg, "k-Means Clusters", "Enter the number of clusters to identify", min_value=2, max_value=min(30, len(self.dataset[0])-1), initial=2)
 		num_clusters = dlg.show()
-		self.loading_dlg.display("Clustering UMAP output")
-		from sklearn.cluster import KMeans
-		km = KMeans(n_clusters=num_clusters)
-		km.fit(np.array(columns_to_rows([self.umap_coords[0], self.umap_coords[1]])))
-		self.kmlabels = ["Cluster "+str(int(lbl)+1) for lbl in km.labels_]
-		self.umap_coords.append(self.kmlabels)
-		self.umap_labels.append("k-Means cluster")
-		kgroups = sorted([str(x) for x in list(set(self.kmlabels))])
-		kcmap = map_colors(kgroups)
-		kcolors = [kcmap[str(g)] for g in self.kmlabels]
-		self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], marker="v", s=15, c=kcolors)
-		klbls = [str(k) for k in kcmap.keys()]
-		kcolkey = list(kcmap.values())
-		ksymbs = [matplotlib.lines.Line2D([], [], marker='v', color=kcolkey[i], label=klbls[i], linestyle='None') for i in range(len(klbls))]
-		self.plot_handle_list.extend(ksymbs)
-		self.plot_label_list.extend(klbls)
-		try:
-			self.plot_axes.get_legend().remove()
-		except:
-			pass
-		self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
-		self.plotfig_canvas.draw()
-		# Only allow creation of one set of clusters for each UMAP output.
-		self.cluster_btn["state"] = tk.DISABLED
-		self.clust_save_btn["state"] = tk.NORMAL
-		self.loading_dlg.hide()
+		if num_clusters is not None:
+			self.loading_dlg.display("Clustering UMAP output")
+			from sklearn.cluster import KMeans
+			km = KMeans(n_clusters=num_clusters)
+			km.fit(np.array(columns_to_rows([self.umap_coords[0], self.umap_coords[1]])))
+			self.kmlabels = ["Cluster "+str(int(lbl)+1) for lbl in km.labels_]
+			self.umap_coords.append(self.kmlabels)
+			self.umap_labels.append("k-Means cluster")
+			kgroups = sorted([str(x) for x in list(set(self.kmlabels))])
+			kcmap = map_colors(kgroups)
+			kcolors = [kcmap[str(g)] for g in self.kmlabels]
+			self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], marker="v", s=15, c=kcolors)
+			klbls = [str(k) for k in kcmap.keys()]
+			kcolkey = list(kcmap.values())
+			ksymbs = [matplotlib.lines.Line2D([], [], marker='v', color=kcolkey[i], label=klbls[i], linestyle='None') for i in range(len(klbls))]
+			self.plot_handle_list.extend(ksymbs)
+			self.plot_label_list.extend(klbls)
+			try:
+				self.plot_axes.get_legend().remove()
+			except:
+				pass
+			self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
+			self.plotfig_canvas.draw()
+			# Only allow creation of one set of clusters for each UMAP output.
+			self.cluster_btn["state"] = tk.DISABLED
+			self.clust_save_btn["state"] = tk.NORMAL
+			self.loading_dlg.hide()
 
 	def kcolumn(self):
 		# Save k-means cluster output as a data table column.
 		# Column selection
 		dlg = CustomContentDialog(parent=self.dlg, title="Save Clusters", prompt="Save k-means clusters in a table column.")
 		def ck_col_name(varname, ix, mode):
 			if self.col_var.get() in self.prohibited_columns:
```

### Comparing `mapdata-3.7.2/mapdata/symbols/24x24/ball24.xbm` & `mapdata-3.8.0/mapdata/symbols/24x24/ball24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/24x24/block24.xbm` & `mapdata-3.8.0/mapdata/symbols/24x24/block24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/24x24/circle24.xbm` & `mapdata-3.8.0/mapdata/symbols/24x24/circle24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/24x24/square24.xbm` & `mapdata-3.8.0/mapdata/symbols/24x24/square24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/28x28/ball28.xbm` & `mapdata-3.8.0/mapdata/symbols/28x28/ball28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/28x28/block28.xbm` & `mapdata-3.8.0/mapdata/symbols/28x28/block28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/28x28/circle28.xbm` & `mapdata-3.8.0/mapdata/symbols/28x28/circle28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata/symbols/28x28/square28.xbm` & `mapdata-3.8.0/mapdata/symbols/28x28/square28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/mapdata.egg-info/PKG-INFO` & `mapdata-3.8.0/mapdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.7.2
+Version: 3.8.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.7.2/mapdata.egg-info/SOURCES.txt` & `mapdata-3.8.0/mapdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.7.2/setup.py` & `mapdata-3.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 symbol_files = glob.glob("mapdata/symbols/16x16/*.xbm") + glob.glob("mapdata/symbols/20x20/*.xbm") + \
 			glob.glob("mapdata/symbols/24x24/*.xbm") + glob.glob("mapdata/symbols/28x28/*.xbm")
 
 setuptools.setup(name='mapdata',
-	version='3.7.2',
+	version='3.8.0',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='cortice@tutanota.com',
     url='https://osdn.net/project/mapdata/',
     packages=['mapdata'],
 	scripts=['mapdata/mapdata.py'],
 	data_files=[('symbols', symbol_files), ('config', ['mapdata/configfile/mapdata.conf'])],
```

