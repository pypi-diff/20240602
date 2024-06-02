# Comparing `tmp/yutto-2.0.0b8.tar.gz` & `tmp/yutto-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yutto-2.0.0b8.tar", max compression
+gzip compressed data, was "yutto-2.0.0b9.tar", max compression
```

## Comparing `yutto-2.0.0b8.tar` & `yutto-2.0.0b9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0    35127 2021-11-01 09:02:52.544502 yutto-2.0.0b8/LICENSE
--rw-r--r--   0        0        0    18780 2022-01-10 09:56:34.149063 yutto-2.0.0b8/README.md
--rw-r--r--   0        0        0     1393 2022-01-10 10:03:39.253750 yutto-2.0.0b8/pyproject.toml
--rw-r--r--   0        0        0      312 2021-11-01 09:02:52.546609 yutto-2.0.0b8/yutto/__init__.py
--rw-r--r--   0        0        0     6671 2021-12-26 16:02:01.773020 yutto-2.0.0b8/yutto/__main__.py
--rw-r--r--   0        0        0      129 2022-01-10 10:03:47.200423 yutto-2.0.0b8/yutto/__version__.py
--rw-r--r--   0        0        0        0 2021-11-01 09:02:52.546864 yutto-2.0.0b8/yutto/api/__init__.py
--rw-r--r--   0        0        0     4031 2022-01-10 08:38:06.158836 yutto-2.0.0b8/yutto/api/acg_video.py
--rw-r--r--   0        0        0     6714 2021-12-16 15:49:23.818435 yutto-2.0.0b8/yutto/api/bangumi.py
--rw-r--r--   0        0        0     1353 2021-11-01 09:02:52.547152 yutto-2.0.0b8/yutto/api/danmaku.py
--rw-r--r--   0        0        0     1883 2022-01-10 08:38:06.159435 yutto-2.0.0b8/yutto/api/info.py
--rw-r--r--   0        0        0     2313 2021-12-15 14:17:30.580165 yutto-2.0.0b8/yutto/api/space.py
--rw-r--r--   0        0        0        0 2021-11-01 09:02:52.547386 yutto-2.0.0b8/yutto/cli/__init__.py
--rw-r--r--   0        0        0    11318 2022-01-10 09:23:08.907675 yutto-2.0.0b8/yutto/cli/batch_get.py
--rw-r--r--   0        0        0     6267 2021-11-01 09:02:52.547624 yutto-2.0.0b8/yutto/cli/checker.py
--rw-r--r--   0        0        0     7941 2022-01-10 09:20:30.694145 yutto-2.0.0b8/yutto/cli/get.py
--rw-r--r--   0        0        0     1680 2021-12-26 15:56:50.891014 yutto-2.0.0b8/yutto/exceptions.py
--rw-r--r--   0        0        0        0 2021-11-01 09:02:52.547906 yutto-2.0.0b8/yutto/media/__init__.py
--rw-r--r--   0        0        0      544 2021-11-01 09:02:52.547994 yutto-2.0.0b8/yutto/media/codec.py
--rw-r--r--   0        0        0     2522 2021-12-21 08:39:41.896438 yutto-2.0.0b8/yutto/media/quality.py
--rw-r--r--   0        0        0        0 2021-11-01 09:02:52.548160 yutto-2.0.0b8/yutto/processor/__init__.py
--rw-r--r--   0        0        0     9677 2022-01-07 17:11:56.419584 yutto-2.0.0b8/yutto/processor/downloader.py
--rw-r--r--   0        0        0     4794 2021-12-21 09:14:37.317452 yutto-2.0.0b8/yutto/processor/filter.py
--rw-r--r--   0        0        0     2279 2022-01-10 09:18:00.951276 yutto-2.0.0b8/yutto/processor/path_resolver.py
--rw-r--r--   0        0        0     4177 2021-12-27 08:40:05.761326 yutto-2.0.0b8/yutto/processor/progressbar.py
--rw-r--r--   0        0        0     3390 2021-11-01 09:02:52.548680 yutto-2.0.0b8/yutto/processor/urlparser.py
--rw-r--r--   0        0        0     2875 2021-11-05 07:40:36.604152 yutto-2.0.0b8/yutto/typing.py
--rw-r--r--   0        0        0        0 2021-11-01 09:02:52.548854 yutto-2.0.0b8/yutto/utils/__init__.py
--rw-r--r--   0        0        0     1168 2021-12-15 13:13:35.747192 yutto-2.0.0b8/yutto/utils/asynclib.py
--rw-r--r--   0        0        0        0 2021-11-01 09:02:52.549044 yutto-2.0.0b8/yutto/utils/console/__init__.py
--rw-r--r--   0        0        0      917 2021-12-26 14:38:24.579229 yutto-2.0.0b8/yutto/utils/console/attributes.py
--rw-r--r--   0        0        0     2696 2021-11-01 09:02:52.549144 yutto-2.0.0b8/yutto/utils/console/colorful.py
--rw-r--r--   0        0        0     1853 2021-11-01 09:02:52.549246 yutto-2.0.0b8/yutto/utils/console/formatter.py
--rw-r--r--   0        0        0     3678 2021-11-01 09:02:52.549340 yutto-2.0.0b8/yutto/utils/console/logger.py
--rw-r--r--   0        0        0      975 2021-11-01 09:02:52.549418 yutto-2.0.0b8/yutto/utils/console/status_bar.py
--rw-r--r--   0        0        0     3238 2021-11-01 09:02:52.549534 yutto-2.0.0b8/yutto/utils/danmaku.py
--rw-r--r--   0        0        0     5990 2021-11-01 09:02:52.549638 yutto-2.0.0b8/yutto/utils/fetcher.py
--rw-r--r--   0        0        0     2408 2021-12-15 13:20:23.685158 yutto-2.0.0b8/yutto/utils/ffmpeg.py
--rw-r--r--   0        0        0     3357 2021-12-15 14:17:47.502135 yutto-2.0.0b8/yutto/utils/file_buffer.py
--rw-r--r--   0        0        0      145 2021-12-15 13:15:12.624167 yutto-2.0.0b8/yutto/utils/functiontools/__init__.py
--rw-r--r--   0        0        0      553 2021-12-15 13:14:21.706636 yutto-2.0.0b8/yutto/utils/functiontools/aobject.py
--rw-r--r--   0        0        0      469 2021-11-01 09:02:52.549994 yutto-2.0.0b8/yutto/utils/functiontools/singleton.py
--rw-r--r--   0        0        0      806 2021-11-01 09:02:52.550074 yutto-2.0.0b8/yutto/utils/functiontools/sync.py
--rw-r--r--   0        0        0      723 2021-11-05 07:41:26.414643 yutto-2.0.0b8/yutto/utils/metadata.py
--rw-r--r--   0        0        0     1456 2021-11-01 09:02:52.550249 yutto-2.0.0b8/yutto/utils/subtitle.py
--rw-r--r--   0        0        0      284 2021-12-15 10:56:15.455409 yutto-2.0.0b8/yutto/utils/time.py
--rw-r--r--   0        0        0    20382 2022-01-10 10:06:40.447959 yutto-2.0.0b8/setup.py
--rw-r--r--   0        0        0    19912 2022-01-10 10:06:40.448749 yutto-2.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0    35127 2021-11-01 09:02:52.544502 yutto-2.0.0b9/LICENSE
+-rw-r--r--   0        0        0    20206 2022-01-24 19:34:53.271257 yutto-2.0.0b9/README.md
+-rw-r--r--   0        0        0     1393 2022-01-24 20:02:49.382951 yutto-2.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0      312 2021-11-01 09:02:52.546609 yutto-2.0.0b9/yutto/__init__.py
+-rw-r--r--   0        0        0     6671 2021-12-26 16:02:01.773020 yutto-2.0.0b9/yutto/__main__.py
+-rw-r--r--   0        0        0      129 2022-01-24 20:03:11.373528 yutto-2.0.0b9/yutto/__version__.py
+-rw-r--r--   0        0        0        0 2021-11-01 09:02:52.546864 yutto-2.0.0b9/yutto/api/__init__.py
+-rw-r--r--   0        0        0     4101 2022-01-24 18:59:36.677499 yutto-2.0.0b9/yutto/api/acg_video.py
+-rw-r--r--   0        0        0     6642 2022-01-24 17:32:51.676970 yutto-2.0.0b9/yutto/api/bangumi.py
+-rw-r--r--   0        0        0     1353 2021-11-01 09:02:52.547152 yutto-2.0.0b9/yutto/api/danmaku.py
+-rw-r--r--   0        0        0     1883 2022-01-10 08:38:06.159435 yutto-2.0.0b9/yutto/api/info.py
+-rw-r--r--   0        0        0     3024 2022-01-14 14:44:10.526479 yutto-2.0.0b9/yutto/api/space.py
+-rw-r--r--   0        0        0        0 2021-11-01 09:02:52.547386 yutto-2.0.0b9/yutto/cli/__init__.py
+-rw-r--r--   0        0        0    13855 2022-01-24 19:11:47.942543 yutto-2.0.0b9/yutto/cli/batch_get.py
+-rw-r--r--   0        0        0     6267 2021-11-01 09:02:52.547624 yutto-2.0.0b9/yutto/cli/checker.py
+-rw-r--r--   0        0        0     7947 2022-01-24 17:47:32.014912 yutto-2.0.0b9/yutto/cli/get.py
+-rw-r--r--   0        0        0     1680 2021-12-26 15:56:50.891014 yutto-2.0.0b9/yutto/exceptions.py
+-rw-r--r--   0        0        0        0 2021-11-01 09:02:52.547906 yutto-2.0.0b9/yutto/media/__init__.py
+-rw-r--r--   0        0        0     1172 2022-01-24 17:30:55.172639 yutto-2.0.0b9/yutto/media/codec.py
+-rw-r--r--   0        0        0     2560 2022-01-24 17:35:01.685124 yutto-2.0.0b9/yutto/media/quality.py
+-rw-r--r--   0        0        0        0 2021-11-01 09:02:52.548160 yutto-2.0.0b9/yutto/processor/__init__.py
+-rw-r--r--   0        0        0     9677 2022-01-07 17:11:56.419584 yutto-2.0.0b9/yutto/processor/downloader.py
+-rw-r--r--   0        0        0     4794 2021-12-21 09:14:37.317452 yutto-2.0.0b9/yutto/processor/filter.py
+-rw-r--r--   0        0        0     2603 2022-01-24 17:53:26.234418 yutto-2.0.0b9/yutto/processor/path_resolver.py
+-rw-r--r--   0        0        0     4177 2021-12-27 08:40:05.761326 yutto-2.0.0b9/yutto/processor/progressbar.py
+-rw-r--r--   0        0        0     3659 2022-01-14 15:00:18.935259 yutto-2.0.0b9/yutto/processor/urlparser.py
+-rw-r--r--   0        0        0     3276 2022-01-24 19:09:54.486060 yutto-2.0.0b9/yutto/typing.py
+-rw-r--r--   0        0        0        0 2021-11-01 09:02:52.548854 yutto-2.0.0b9/yutto/utils/__init__.py
+-rw-r--r--   0        0        0     1168 2021-12-15 13:13:35.747192 yutto-2.0.0b9/yutto/utils/asynclib.py
+-rw-r--r--   0        0        0        0 2021-11-01 09:02:52.549044 yutto-2.0.0b9/yutto/utils/console/__init__.py
+-rw-r--r--   0        0        0      917 2021-12-26 14:38:24.579229 yutto-2.0.0b9/yutto/utils/console/attributes.py
+-rw-r--r--   0        0        0     2696 2021-11-01 09:02:52.549144 yutto-2.0.0b9/yutto/utils/console/colorful.py
+-rw-r--r--   0        0        0     1853 2021-11-01 09:02:52.549246 yutto-2.0.0b9/yutto/utils/console/formatter.py
+-rw-r--r--   0        0        0     4126 2022-01-24 17:51:01.067690 yutto-2.0.0b9/yutto/utils/console/logger.py
+-rw-r--r--   0        0        0      975 2021-11-01 09:02:52.549418 yutto-2.0.0b9/yutto/utils/console/status_bar.py
+-rw-r--r--   0        0        0     3238 2021-11-01 09:02:52.549534 yutto-2.0.0b9/yutto/utils/danmaku.py
+-rw-r--r--   0        0        0     6249 2022-01-24 19:21:43.848193 yutto-2.0.0b9/yutto/utils/fetcher.py
+-rw-r--r--   0        0        0     2408 2021-12-15 13:20:23.685158 yutto-2.0.0b9/yutto/utils/ffmpeg.py
+-rw-r--r--   0        0        0     3357 2021-12-15 14:17:47.502135 yutto-2.0.0b9/yutto/utils/file_buffer.py
+-rw-r--r--   0        0        0      145 2021-12-15 13:15:12.624167 yutto-2.0.0b9/yutto/utils/functiontools/__init__.py
+-rw-r--r--   0        0        0      553 2021-12-15 13:14:21.706636 yutto-2.0.0b9/yutto/utils/functiontools/aobject.py
+-rw-r--r--   0        0        0      469 2021-11-01 09:02:52.549994 yutto-2.0.0b9/yutto/utils/functiontools/singleton.py
+-rw-r--r--   0        0        0      806 2021-11-01 09:02:52.550074 yutto-2.0.0b9/yutto/utils/functiontools/sync.py
+-rw-r--r--   0        0        0      723 2021-11-05 07:41:26.414643 yutto-2.0.0b9/yutto/utils/metadata.py
+-rw-r--r--   0        0        0      667 2022-01-24 17:33:41.957639 yutto-2.0.0b9/yutto/utils/priority.py
+-rw-r--r--   0        0        0     1456 2021-11-01 09:02:52.550249 yutto-2.0.0b9/yutto/utils/subtitle.py
+-rw-r--r--   0        0        0      284 2021-12-15 10:56:15.455409 yutto-2.0.0b9/yutto/utils/time.py
+-rw-r--r--   0        0        0    21815 2022-01-24 20:08:18.551108 yutto-2.0.0b9/setup.py
+-rw-r--r--   0        0        0    21338 2022-01-24 20:08:18.551910 yutto-2.0.0b9/PKG-INFO
```

### Comparing `yutto-2.0.0b8/LICENSE` & `yutto-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/README.md` & `yutto-2.0.0b9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,25 +38,24 @@
 ```
 
 ## 主要功能
 
 ### 已支持的下载类型
 
 <!-- prettier-ignore -->
-|type|batch|path template|
-|-|-|-|
-|投稿视频|:x:|`{title}`|
-|投稿视频|:white_check_mark:|`{title}/{name}`|
-|番剧|:x:|`{name}`|
-|番剧|:white_check_mark:|`{title}/{name}`|
-|用户指定收藏夹|:white_check_mark:|`{username}的收藏夹/{fav_title}/{title}/{name}`|
-|用户全部收藏夹|:white_check_mark:|`{username}的收藏夹/{fav_title}/{title}/{name}`|
-|UP 主个人空间|:white_check_mark:|`{username}的全部投稿视频/{title}/{name}`|
-
-<!-- TODO: 展示更多细节 -->
+|Type|Batch|Example url|Path template|
+|-|-|-|-|
+|投稿视频|:x:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ` <br/> `https://www.bilibili.com/video/av371660125` <br/> `https://www.bilibili.com/video/BV1vZ4y1M7mQ?p=1` <br/> `av371660125` <br/> `BV1vZ4y1M7mQ`|`{title}`|
+|投稿视频|:white_check_mark:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ` <br/> `https://www.bilibili.com/video/av371660125`  <br/> `av371660125` <br/> `BV1vZ4y1M7mQ`|`{title}/{name}`|
+|番剧|:x:|`https://www.bilibili.com/bangumi/play/ep395211` <br/> `ep395211`|`{name}`|
+|番剧|:white_check_mark:|`https://www.bilibili.com/bangumi/play/ep395211` <br/> `https://www.bilibili.com/bangumi/play/ss38221` <br/> `https://www.bilibili.com/bangumi/media/md28233903` <br/> `ep395211` <br/> `ss38221` <br/> `md28233903`|`{title}/{name}`|
+|用户指定收藏夹|:white_check_mark:|`https://space.bilibili.com/100969474/favlist?fid=1306978874`|`{username}的收藏夹/{series_title}/{title}/{name}`|
+|用户全部收藏夹|:white_check_mark:|`https://space.bilibili.com/100969474/favlist`|`{username}的收藏夹/{series_title}/{title}/{name}`|
+|UP 主个人空间|:white_check_mark:|`https://space.bilibili.com/100969474/video`|`{username}的全部投稿视频/{title}/{name}`|
+|视频合集|:white_check_mark:|`https://space.bilibili.com/100969474/channel/seriesdetail?sid=1947439` <br/> `https://www.bilibili.com/medialist/play/100969474?business=space_series&business_id=1947439`|`{series_title}/{title}/{name}`|
 
 ### 基本命令
 
 yutto 的基本命令如下：
 
 ```bash
 yutto <url>
@@ -101,34 +100,37 @@
 -  默认值 `8`
 
 与 bilili 不同的是，yutto 并不是使用多线程实现并行下载，而是使用协程实现的，本参数限制的是最大的并行 Worker 数量。
 
 #### 指定视频清晰度等级
 
 -  参数 `-q` 或 `--video-quality`
--  可选值 `127 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16`
+-  可选值 `127 | 126 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16`
 -  默认值 `127`
 
 清晰度对应关系如下
 
 <!-- prettier-ignore -->
 |code|清晰度|
 |:-:|:-:|
 |127|8K 超高清|
+|126|杜比视界|
 |125|HDR 真彩|
 |120|4K 超清|
 |116|1080P 60帧|
 |112|1080P 高码率|
 |80|1080P 高清|
 |74|720P 60帧|
 |64|720P 高清|
 |32|480P 清晰|
 |16|360P 流畅|
 
-并不是说指定某个清晰度就一定会下载该清晰度的视频，yutto 只会尽可能满足你的要求，如果不存在指定的清晰度，yutto 就会按照默认的清晰度搜索机制进行调节，比如指定清晰度为 `80`，**首先会依次降清晰度搜索** `74`、`64`、`32`、`16`，如果依然找不到合适的则**继续升清晰度搜索** `112`、`116`、`120`、`125`、`127`。
+并不是说指定某个清晰度就一定会下载该清晰度的视频，yutto 只会尽可能满足你的要求，如果不存在指定的清晰度，yutto 就会按照默认的清晰度搜索机制进行调节，比如指定清晰度为 `80`，**首先会依次降清晰度搜索** `74`、`64`、`32`、`16`，如果依然找不到合适的则**继续升清晰度搜索** `112`、`116`、`120`、`125`、`126`、`127`。
+
+值得注意的是，目前杜比视界视频只能简单下载音视频流并合并，合并后并不能达到在线观看的效果。
 
 #### 指定音频码率等级
 
 -  参数 `-aq` 或 `--audio-quality`
 -  可选值 `30280 | 30232 | 30216`
 -  默认值 `30280`
 
@@ -137,28 +139,28 @@
 <!-- prettier-ignore -->
 |code|码率|
 |:-:|:-:|
 |30280|320kbps|
 |30232|128kbps|
 |30216|64kbps|
 
-清晰度自动调节机制与视频清晰度一致，也采用先降后升的匹配机制。
+码率自动调节机制与视频清晰度一致，也采用先降后升的匹配机制。
 
 #### 指定视频编码
 
 -  参数 `--vcodec`
--  下载编码可选值 `"hevc" | "avc"`
+-  下载编码可选值 `"av1" | "hevc" | "avc"`
 -  保存编码可选值 FFmpeg 所有可用的视频编码器
 -  默认值 `"avc:copy"`
 
 该参数略微复杂，前半部分表示在下载时**优先**选择哪一种编码的视频流，后半部分则表示在合并时如何编码视频流，两者使用 `:` 分隔。
 
 值得注意的是，前半的下载编码只是优先下载的编码而已，如果不存在该编码，则仍会像视频清晰度调节机制一样自动选择其余编码。
 
-而后半部分的参数如果设置成非 `copy` 的值则可以确保在下载完成后对其进行重新编码，而且不止支持 `hevc` 与 `avc`，只要你的 FFmpeg 支持的视频编码器，它都可以完成。
+而后半部分的参数如果设置成非 `copy` 的值则可以确保在下载完成后对其进行重新编码，而且不止支持 `av1`、`hevc` 与 `avc`，只要你的 FFmpeg 支持的视频编码器，它都可以完成。
 
 #### 指定音频编码
 
 -  参数 `--acodec`
 -  下载编码可选值 `"mp4a"`
 -  保存编码可选值 FFmpeg 所有可用的音频编码器
 -  默认值 `"mp4a:copy"`
@@ -218,15 +220,15 @@
 
 -  参数 `--tmp-dir`
 -  默认值是“存放根目录”即 `-d, --dir` 的值
 
 #### 存放子路径模板
 
 -  参数 `-tp` 或 `--subpath-template`
--  可选参数变量 `title | id | name | username | fav_title | pubdate` （以后可能会有更多）
+-  可选参数变量 `title | id | name | username | series_title | pubdate` （以后可能会有更多）
 -  默认值 `"{auto}"`
 
 通过配置子路径模板可以灵活地控制视频存放位置。
 
 默认情况是由 yutto 自动控制存放位置的。比如下载单个视频时默认就是直接存放在设定的根目录，不会创建一层容器目录，此时自动选择了 `{name}` 作为模板；而批量下载时则会根据视频层级生成多级目录，比如番剧会是 `{title}/{name}`，首先会在设定根目录里生成一个番剧名的目录，其内才会存放各个番剧剧集视频，这样方便了多个不同番剧的管理。当然，如果你仍希望将番剧直接存放在设定根目录下的话，可以修改该参数值为 `{name}`即可。
 
 另外，该功能语法由 Python format 函数模板语法提供，所以也支持一些高级的用法，比如 `{id:0>3}{name}`。
@@ -235,17 +237,20 @@
 
 <!-- prettier-ignore -->
 |Variable|Description|Scope|
 |-|-|-|
 |title|系列视频总标题（番剧名/投稿视频标题）|全部|
 |id|系列视频单 p 顺序标号|全部|
 |name|系列视频单 p 标题|全部|
-|username|UP 主用户名|个人空间、收藏夹下载|
+|username|UP 主用户名|个人空间、收藏夹、合集下载|
+|series_title|合集标题|收藏夹、视频合集下载|
 |pubdate|投稿日期|仅投稿视频|
 
+> 未来可能会对路径变量及默认路径模板进行调整
+
 #### url 别名文件路径
 
 -  参数 `-af` 或 `--alias-file`
 -  默认值 `None`
 
 指定别名文件路径，别名文件中存放一个别名与其对应的 url，使用空格或者 `=` 分隔，示例如下：
 
@@ -375,14 +380,15 @@
 ```
 
 下面是一些要注意的问题
 
 1. 这里使用的序号是视频的顺序序号，而不是番剧所标注的`第 n 话`，因为有可能会出现 `第 x.5 话` 等等的特殊情况，此时一定要按照顺序自行计数。
 2. 参数值里一定不要加空格
 3. 参数值开头为 `-` 时前面应该使用 `=` 而非空格
+4. 个人空间、合集、收藏夹等批量下载暂不支持选集操作
 
 #### 同时下载附加剧集
 
 -  参数 `-s` 或 `--with-section`
 -  默认值 `False`
 
 </details>
@@ -406,16 +412,16 @@
 
 ### 新增的特性
 
 -  单视频下载与批量下载命令分离（`bilili` 命令与 `yutto --batch` 相类似）
 -  音频/视频编码选择
 -  仅下载音频/视频
 -  存放子路径的自由定制
--  支持 url alias
--  支持 file scheme
+-  支持 url 别名
+-  支持文件列表
 -  更多的批下载支持（现已支持 UP 主全部视频下载，扩展其它批下载支持也很简单）
 -  更加完善的 warning 与 error 提示
 -  支持仅输入 id 即可下载（aid、bvid、episode_id 等）
 -  支持描述文件生成（当前仅番剧）
 
 ## 小技巧
 
@@ -507,14 +513,15 @@
 -  [x] refactor: url 列表能够预线性展开
 -  [x] feat: 添加各种 return code
 -  [x] test: 编写单元测试
 
 ### 2.0.0
 
 -  [ ] feat: 投稿视频描述文件支持
+-  [ ] refactor: 整理路径变量名
 -  [ ] docs: 可爱的 logo（呜呜呜，有谁会做 logo 嘛？）
 -  [ ] docs: 可爱的静态文档（可能需要 VitePress 到 1.0）
 
 ### future
 
 -  [ ] feat: 字幕、弹幕嵌入视频支持（也许？）
 -  [ ] feat: 封面下载支持（也许？）
```

#### html2text {}

```diff
@@ -5,23 +5,45 @@
 å®è£é¢è§ç å¨æ­¤ä¹åè¯·ç¡®ä¿å®è£ Python3.9
 åä»¥ä¸çæ¬ï¼å¹¶éç½®å¥½ FFmpegï¼åç§ [bilili ææ¡£](https://
 bilili.sigure.xyz/guide/getting-started.html)ï¼ å½å yutto å°å¤äº beta
 é¶æ®µï¼æä»»ä½å»ºè®®å°½ç®¡å¨ [Discussions](https://github.com/SigureMo/
 yutto/discussions) æåºï½ï½ï½ ### pip å®è£ ```bash pip install --pre
 yutto ``` ### git clone ```bash git clone https://github.com/SigureMo/yutto.git
 cd yutto/ pip install poetry poetry build pip install ./dist/yutto-*.whl ``` ##
-ä¸»è¦åè½ ### å·²æ¯æçä¸è½½ç±»å |type|batch|path template| |-|-|-
-| |æç¨¿è§é¢|:x:|`{title}`| |æç¨¿è§é¢|:white_check_mark:|`{title}/
-{name}`| |çªå§|:x:|`{name}`| |çªå§|:white_check_mark:|`{title}/{name}`|
-|ç¨æ·æå®æ¶èå¤¹|:white_check_mark:|`{username}çæ¶èå¤¹/{fav_title}/
-{title}/{name}`| |ç¨æ·å¨é¨æ¶èå¤¹|:white_check_mark:|`
-{username}çæ¶èå¤¹/{fav_title}/{title}/{name}`| |UP ä¸»ä¸ªäººç©ºé´|:
-white_check_mark:|`{username}çå¨é¨æç¨¿è§é¢/{title}/{name}`| ###
-åºæ¬å½ä»¤ yutto çåºæ¬å½ä»¤å¦ä¸ï¼ ```bash yutto ``` ä½ å¯ä»¥éè¿
-`yutto -h` æ¥çè¯¦ç»å½ä»¤åæ°ã
+ä¸»è¦åè½ ### å·²æ¯æçä¸è½½ç±»å |Type|Batch|Example url|Path
+template| |-|-|-|-| |æç¨¿è§é¢|:x:|`https://www.bilibili.com/video/
+BV1vZ4y1M7mQ`
+`https://www.bilibili.com/video/av371660125`
+`https://www.bilibili.com/video/BV1vZ4y1M7mQ?p=1`
+`av371660125`
+`BV1vZ4y1M7mQ`|`{title}`| |æç¨¿è§é¢|:white_check_mark:|`https://
+www.bilibili.com/video/BV1vZ4y1M7mQ`
+`https://www.bilibili.com/video/av371660125`
+`av371660125`
+`BV1vZ4y1M7mQ`|`{title}/{name}`| |çªå§|:x:|`https://www.bilibili.com/bangumi/
+play/ep395211`
+`ep395211`|`{name}`| |çªå§|:white_check_mark:|`https://www.bilibili.com/
+bangumi/play/ep395211`
+`https://www.bilibili.com/bangumi/play/ss38221`
+`https://www.bilibili.com/bangumi/media/md28233903`
+`ep395211`
+`ss38221`
+`md28233903`|`{title}/{name}`| |ç¨æ·æå®æ¶èå¤¹|:white_check_mark:
+|`https://space.bilibili.com/100969474/favlist?fid=1306978874`|`
+{username}çæ¶èå¤¹/{series_title}/{title}/{name}`| |ç¨æ·å¨é¨æ¶èå¤¹|:
+white_check_mark:|`https://space.bilibili.com/100969474/favlist`|`
+{username}çæ¶èå¤¹/{series_title}/{title}/{name}`| |UP ä¸»ä¸ªäººç©ºé´|:
+white_check_mark:|`https://space.bilibili.com/100969474/video`|`
+{username}çå¨é¨æç¨¿è§é¢/{title}/{name}`| |è§é¢åé|:
+white_check_mark:|`https://space.bilibili.com/100969474/channel/
+seriesdetail?sid=1947439`
+`https://www.bilibili.com/medialist/play/
+100969474?business=space_series&business_id=1947439`|`{series_title}/{title}/
+{name}`| ### åºæ¬å½ä»¤ yutto çåºæ¬å½ä»¤å¦ä¸ï¼ ```bash yutto ```
+ä½ å¯ä»¥éè¿ `yutto -h` æ¥çè¯¦ç»å½ä»¤åæ°ã
 å¦æä½ éè¦ä¸è½½**åä¸ª**è§é¢ï¼åªéè¦ä½¿ç¨ yutto
 å ä¸è¿ä¸ªè§é¢çå°åå³å¯ãå®æ¯æ av/BV å·ä»¥åç¸åºå¸¦ p=n
 åæ°çæç¨¿è§é¢é¡µé¢ï¼ä¹æ¯æ ep
 å·ï¼episode_idï¼ççªå§é¡µé¢ã æ¯å¦åªéè¦è¿æ ·ä½ å°±å¯ä»¥ä¸è½½
 [ãè»¢ã¹ã©æ¥è¨ã](https://www.bilibili.com/bangumi/play/
 ep395211)ç¬¬ä¸è¯ï¼ ```bash yutto https://www.bilibili.com/bangumi/play/
 ep395211 ``` yutto è¿æ¯æç´æ¥ä½¿ç¨è½å¤å¯ä¸å®ä½èµæºç id
@@ -37,38 +59,39 @@
 åºç¡åæ° > å¤§é¨ååæ°ä¸ bilili éåï¼å¯åè [bilili ç cli
 ææ¡£](https://bilili.nyakku.moe/cli/) yutto
 æ¯æä¸äºåºç¡åæ°ï¼æ è®ºæ¯æ¹éä¸è½½è¿æ¯åè§é¢ä¸è½½é½éç¨ã
 ç¹å»å±å¼è¯¦ç»åæ° #### æå¤§å¹¶è¡ worker æ°é - åæ° `-n` æ `--
 num-workers` - é»è®¤å¼ `8` ä¸ bilili ä¸åçæ¯ï¼yutto
 å¹¶ä¸æ¯ä½¿ç¨å¤çº¿ç¨å®ç°å¹¶è¡ä¸è½½ï¼èæ¯ä½¿ç¨åç¨å®ç°çï¼æ¬åæ°éå¶çæ¯æå¤§çå¹¶è¡
 Worker æ°éã #### æå®è§é¢æ¸æ°åº¦ç­çº§ - åæ° `-q` æ `--video-
-quality` - å¯éå¼ `127 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16` -
-é»è®¤å¼ `127` æ¸æ°åº¦å¯¹åºå³ç³»å¦ä¸ |code|æ¸æ°åº¦| |:-:|:-:| |127|8K
-è¶é«æ¸| |125|HDR çå½©| |120|4K è¶æ¸| |116|1080P 60å¸§| |112|1080P
-é«ç ç| |80|1080P é«æ¸| |74|720P 60å¸§| |64|720P é«æ¸| |32|480P æ¸æ°|
-|16|360P æµç|
+quality` - å¯éå¼ `127 | 126 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 |
+16` - é»è®¤å¼ `127` æ¸æ°åº¦å¯¹åºå³ç³»å¦ä¸ |code|æ¸æ°åº¦| |:-:|:-:
+| |127|8K è¶é«æ¸| |126|ææ¯è§ç| |125|HDR çå½©| |120|4K è¶æ¸|
+|116|1080P 60å¸§| |112|1080P é«ç ç| |80|1080P é«æ¸| |74|720P 60å¸§|
+|64|720P é«æ¸| |32|480P æ¸æ°| |16|360P æµç|
 å¹¶ä¸æ¯è¯´æå®æä¸ªæ¸æ°åº¦å°±ä¸å®ä¼ä¸è½½è¯¥æ¸æ°åº¦çè§é¢ï¼yutto
 åªä¼å°½å¯è½æ»¡è¶³ä½ çè¦æ±ï¼å¦æä¸å­å¨æå®çæ¸æ°åº¦ï¼yutto
 å°±ä¼æç§é»è®¤çæ¸æ°åº¦æç´¢æºå¶è¿è¡è°èï¼æ¯å¦æå®æ¸æ°åº¦ä¸º
 `80`ï¼**é¦åä¼ä¾æ¬¡éæ¸æ°åº¦æç´¢**
 `74`ã`64`ã`32`ã`16`ï¼å¦æä¾ç¶æ¾ä¸å°åéçå**ç»§ç»­åæ¸æ°åº¦æç´¢**
-`112`ã`116`ã`120`ã`125`ã`127`ã #### æå®é³é¢ç çç­çº§ - åæ°
-`-aq` æ `--audio-quality` - å¯éå¼ `30280 | 30232 | 30216` - é»è®¤å¼
-`30280` ç çå¯¹åºå³ç³»å¦ä¸ |code|ç ç| |:-:|:-:| |30280|320kbps|
-|30232|128kbps| |30216|64kbps|
-æ¸æ°åº¦èªå¨è°èæºå¶ä¸è§é¢æ¸æ°åº¦ä¸è´ï¼ä¹éç¨åéååçå¹éæºå¶ã
-#### æå®è§é¢ç¼ç  - åæ° `--vcodec` - ä¸è½½ç¼ç å¯éå¼ `"hevc" |
-"avc"` - ä¿å­ç¼ç å¯éå¼ FFmpeg ææå¯ç¨çè§é¢ç¼ç å¨ -
+`112`ã`116`ã`120`ã`125`ã`126`ã`127`ã
+å¼å¾æ³¨æçæ¯ï¼ç®åææ¯è§çè§é¢åªè½ç®åä¸è½½é³è§é¢æµå¹¶åå¹¶ï¼åå¹¶åå¹¶ä¸è½è¾¾å°å¨çº¿è§ççææã
+#### æå®é³é¢ç çç­çº§ - åæ° `-aq` æ `--audio-quality` - å¯éå¼
+`30280 | 30232 | 30216` - é»è®¤å¼ `30280` ç çå¯¹åºå³ç³»å¦ä¸
+|code|ç ç| |:-:|:-:| |30280|320kbps| |30232|128kbps| |30216|64kbps|
+ç çèªå¨è°èæºå¶ä¸è§é¢æ¸æ°åº¦ä¸è´ï¼ä¹éç¨åéååçå¹éæºå¶ã
+#### æå®è§é¢ç¼ç  - åæ° `--vcodec` - ä¸è½½ç¼ç å¯éå¼ `"av1" |
+"hevc" | "avc"` - ä¿å­ç¼ç å¯éå¼ FFmpeg ææå¯ç¨çè§é¢ç¼ç å¨ -
 é»è®¤å¼ `"avc:copy"`
 è¯¥åæ°ç¥å¾®å¤æï¼ååé¨åè¡¨ç¤ºå¨ä¸è½½æ¶**ä¼å**éæ©åªä¸ç§ç¼ç çè§é¢æµï¼ååé¨ååè¡¨ç¤ºå¨åå¹¶æ¶å¦ä½ç¼ç è§é¢æµï¼ä¸¤èä½¿ç¨
 `:` åéã
 å¼å¾æ³¨æçæ¯ï¼ååçä¸è½½ç¼ç åªæ¯ä¼åä¸è½½çç¼ç èå·²ï¼å¦æä¸å­å¨è¯¥ç¼ç ï¼åä»ä¼åè§é¢æ¸æ°åº¦è°èæºå¶ä¸æ ·èªå¨éæ©å¶ä½ç¼ç ã
 èååé¨åçåæ°å¦æè®¾ç½®æé `copy`
 çå¼åå¯ä»¥ç¡®ä¿å¨ä¸è½½å®æåå¯¹å¶è¿è¡éæ°ç¼ç ï¼èä¸ä¸æ­¢æ¯æ
-`hevc` ä¸ `avc`ï¼åªè¦ä½ ç FFmpeg
+`av1`ã`hevc` ä¸ `avc`ï¼åªè¦ä½ ç FFmpeg
 æ¯æçè§é¢ç¼ç å¨ï¼å®é½å¯ä»¥å®æã #### æå®é³é¢ç¼ç  -
 åæ° `--acodec` - ä¸è½½ç¼ç å¯éå¼ `"mp4a"` - ä¿å­ç¼ç å¯éå¼
 FFmpeg ææå¯ç¨çé³é¢ç¼ç å¨ - é»è®¤å¼ `"mp4a:copy"`
 è¯¦æåè§é¢ç¼ç ã #### ä»ä¸è½½è§é¢æµ - åæ° `--video-only` -
 é»è®¤å¼ `False` #### ä»ä¸è½½é³é¢æµ - åæ° `--audio-only` - é»è®¤å¼
 `False` ä»ä¸è½½å¶ä¸­çé³é¢æµï¼ä¿å­ä¸º `.aac` æä»¶ã
 å¼å¾æ³¨æçæ¯ï¼å¨ä¸éæ©è§é¢æµæ¶ï¼åµå¥å­å¹ãå¼¹å¹åè½å°æ æ³å·¥ä½ã
@@ -89,15 +112,15 @@
 ://url/to/proxy/server>` - é»è®¤å¼ `"auto"`
 è®¾ç½®ä»£çæå¡å¨ï¼é»è®¤æ¯ä»ç¯å¢åéè¯»åï¼`no`
 åä¸ºä¸è®¾ç½®ä»£çï¼è®¾ç½®å¶å® http/https url
 åå°å¶ä½ä¸ºä»£çæå¡å¨ã #### å­æ¾æ ¹ç®å½ - åæ° `-d` æ `--
 dir` - é»è®¤å¼ `"./"` #### ä¸´æ¶æä»¶ç®å½ - åæ° `--tmp-dir` -
 é»è®¤å¼æ¯âå­æ¾æ ¹ç®å½âå³ `-d, --dir` çå¼ ####
 å­æ¾å­è·¯å¾æ¨¡æ¿ - åæ° `-tp` æ `--subpath-template` -
-å¯éåæ°åé `title | id | name | username | fav_title | pubdate`
+å¯éåæ°åé `title | id | name | username | series_title | pubdate`
 ï¼ä»¥åå¯è½ä¼ææ´å¤ï¼ - é»è®¤å¼ `"{auto}"`
 éè¿éç½®å­è·¯å¾æ¨¡æ¿å¯ä»¥çµæ´»å°æ§å¶è§é¢å­æ¾ä½ç½®ã
 é»è®¤æåµæ¯ç± yutto
 èªå¨æ§å¶å­æ¾ä½ç½®çãæ¯å¦ä¸è½½åä¸ªè§é¢æ¶é»è®¤å°±æ¯ç´æ¥å­æ¾å¨è®¾å®çæ ¹ç®å½ï¼ä¸ä¼åå»ºä¸å±å®¹å¨ç®å½ï¼æ­¤æ¶èªå¨éæ©äº
 `{name}`
 ä½ä¸ºæ¨¡æ¿ï¼èæ¹éä¸è½½æ¶åä¼æ ¹æ®è§é¢å±çº§çæå¤çº§ç®å½ï¼æ¯å¦çªå§ä¼æ¯
 `{title}/
@@ -107,17 +130,19 @@
 0>3}{name}`ã
 å¼å¾æ³¨æçæ¯ï¼å¹¶ä¸æ¯ææåéå¨åç§åºåä¸é½ä¼æä¾ï¼æ¯å¦
 `username` åéå½åä»å¨ UP ä¸»å¨é¨æç¨¿è§é¢/
 æ¶èå¤¹ææä¾ï¼å¨å¶å®æåµä¸ä¸åºä½¿ç¨å®ãååéè¯¦ç»ä½ç¨åæè¿°è§ä¸è¡¨ï¼
 |Variable|Description|Scope| |-|-|-| |title|ç³»åè§é¢æ»æ é¢ï¼çªå§å/
 æç¨¿è§é¢æ é¢ï¼|å¨é¨| |id|ç³»åè§é¢å p é¡ºåºæ å·|å¨é¨|
 |name|ç³»åè§é¢å p æ é¢|å¨é¨| |username|UP
-ä¸»ç¨æ·å|ä¸ªäººç©ºé´ãæ¶èå¤¹ä¸è½½|
-|pubdate|æç¨¿æ¥æ|ä»æç¨¿è§é¢| #### url å«åæä»¶è·¯å¾ - åæ° `-
-af` æ `--alias-file` - é»è®¤å¼ `None`
+ä¸»ç¨æ·å|ä¸ªäººç©ºé´ãæ¶èå¤¹ãåéä¸è½½|
+|series_title|åéæ é¢|æ¶èå¤¹ãè§é¢åéä¸è½½|
+|pubdate|æç¨¿æ¥æ|ä»æç¨¿è§é¢| >
+æªæ¥å¯è½ä¼å¯¹è·¯å¾åéåé»è®¤è·¯å¾æ¨¡æ¿è¿è¡è°æ´ #### url
+å«åæä»¶è·¯å¾ - åæ° `-af` æ `--alias-file` - é»è®¤å¼ `None`
 æå®å«åæä»¶è·¯å¾ï¼å«åæä»¶ä¸­å­æ¾ä¸ä¸ªå«åä¸å¶å¯¹åºç
 urlï¼ä½¿ç¨ç©ºæ ¼æè `=` åéï¼ç¤ºä¾å¦ä¸ï¼ ``` rimuru1=https://
 www.bilibili.com/bangumi/play/ss25739/ rimuru2=https://www.bilibili.com/
 bangumi/play/ss36170/ rimuru-nikki=https://www.bilibili.com/bangumi/play/
 ss38221/ ``` æ¯å¦å°ä¸è¿°åå®¹å­å¨å°
 `~/.yutto_alias`ï¼åéè¿ä»¥ä¸å½ä»¤å³å¯è§£æè¯¥æä»¶ï¼ ```bash yutto
 rimuru1 --batch --alias-file='~/.yutto_alias' ``` å½åæ°å¼ä¸º `-
@@ -177,28 +202,29 @@
 p ^~3,10,12~14,16,-4~$ # å¾ææ¾ï¼ä¸é¢çä¾å­å°±æ¯ä¸è½½å 3 è¯ãç¬¬
 10 è¯ãç¬¬ 12 å° 14 è¯ãç¬¬ 16 è¯ä»¥åå 4 è¯ ```
 ä¸é¢æ¯ä¸äºè¦æ³¨æçé®é¢ 1.
 è¿éä½¿ç¨çåºå·æ¯è§é¢çé¡ºåºåºå·ï¼èä¸æ¯çªå§ææ æ³¨ç`ç¬¬
 n è¯`ï¼å ä¸ºæå¯è½ä¼åºç° `ç¬¬ x.5 è¯`
 ç­ç­çç¹æ®æåµï¼æ­¤æ¶ä¸å®è¦æç§é¡ºåºèªè¡è®¡æ°ã 2.
 åæ°å¼éä¸å®ä¸è¦å ç©ºæ ¼ 3. åæ°å¼å¼å¤´ä¸º `-
-` æ¶åé¢åºè¯¥ä½¿ç¨ `=` èéç©ºæ ¼ #### åæ¶ä¸è½½éå å§é - åæ°
-`-s` æ `--with-section` - é»è®¤å¼ `False` ## ä» bilili1.x è¿ç§» ###
-åæ¶çåè½ - `- bilibili` ç®å½ççæ - æ­æ¾åè¡¨çæ -
-æºæ ¼å¼ä¿®æ¹åè½ï¼ä¸åæ¯æ flv
+` æ¶åé¢åºè¯¥ä½¿ç¨ `=` èéç©ºæ ¼ 4.
+ä¸ªäººç©ºé´ãåéãæ¶èå¤¹ç­æ¹éä¸è½½æä¸æ¯æééæä½ ####
+åæ¶ä¸è½½éå å§é - åæ° `-s` æ `--with-section` - é»è®¤å¼ `False`
+## ä» bilili1.x è¿ç§» ### åæ¶çåè½ - `- bilibili` ç®å½ççæ -
+æ­æ¾åè¡¨çæ - æºæ ¼å¼ä¿®æ¹åè½ï¼ä¸åæ¯æ flv
 æºè§é¢ä¸è½½ï¼å¦æä»æè§é¢ä¸æ¯æ dash æºï¼è¯·ç»§ç»­ä½¿ç¨
 bililiï¼ - å¯¹ Python3.8 çæ¯æï¼æä½æ¯æ Python3.9 - ä¸è½½åè¯¢é®
 ### é»è®¤è¡ä¸ºçä¿®æ¹ -
 ä½¿ç¨åç¨èéå¤çº¿ç¨è¿è¡ä¸è½½ï¼åæ¶ä¹ä¸æ¯æ¹éè§£ææ¹éä¸è½½ï¼èæ¯è¾¹è§£æè¾¹ä¸è½½
 - é»è®¤çæå¼¹å¹ä¸º ASS - é»è®¤å¯ç¨ä»å¤éåæºä¸è½½çç¹æ§ -
 ä¸ä»å¯ä»¥æ§å¶æ¯å¦ä½¿ç¨ç³»ç»ä»£çï¼è¿è½éç½®ç¹å®çä»£çæå¡å¨
 ### æ°å¢çç¹æ§ - åè§é¢ä¸è½½ä¸æ¹éä¸è½½å½ä»¤åç¦»ï¼`bilili`
 å½ä»¤ä¸ `yutto --batch` ç¸ç±»ä¼¼ï¼ - é³é¢/è§é¢ç¼ç éæ© -
-ä»ä¸è½½é³é¢/è§é¢ - å­æ¾å­è·¯å¾çèªç±å®å¶ - æ¯æ url alias -
-æ¯æ file scheme - æ´å¤çæ¹ä¸è½½æ¯æï¼ç°å·²æ¯æ UP
+ä»ä¸è½½é³é¢/è§é¢ - å­æ¾å­è·¯å¾çèªç±å®å¶ - æ¯æ url å«å -
+æ¯ææä»¶åè¡¨ - æ´å¤çæ¹ä¸è½½æ¯æï¼ç°å·²æ¯æ UP
 ä¸»å¨é¨è§é¢ä¸è½½ï¼æ©å±å¶å®æ¹ä¸è½½æ¯æä¹å¾ç®åï¼ -
 æ´å å®åç warning ä¸ error æç¤º - æ¯æä»è¾å¥ id
 å³å¯ä¸è½½ï¼aidãbvidãepisode_id ç­ï¼ -
 æ¯ææè¿°æä»¶çæï¼å½åä»çªå§ï¼ ## å°æå·§ ### ä½¿ç¨ uvloop
 æååç¨æç å¬è¯´ uvloop
 å¯ä»¥æé«åç¨æçï¼å¦æä½ çç³»ç»é Windows
 çè¯ï¼å¯ä»¥è¯ä¸ä¸å®è£ uvloopï¼ ```bash pip install uvloop ```
@@ -232,16 +258,16 @@
 www.bilibili.com/bangumi/play/ep395211?t=24) ### yutto ä¼å¾å¿«æ¿ä»£ bilili
 å ç­æåä¸ä¼ï¼bilili å¹¶ä¸ä¼æ¶å¤±ï¼å¨ä¸æ®µæ¶é´å bilili
 ä»ä¼åçº éæ§ç»´æ¤ï¼åªæ¯ä¸ä¼æä¾æ°ç¹æ§äºã yutto
 ç°å¨ä¹è¿ä¸æ¯éå¸¸ç¨³å®ï¼éè¦ç¨³å®çä½éªçè¯è¯·ç»§ç»­ä½¿ç¨
 bilili ï½ ## Roadmap ### 2.0.0-beta - [x] feat: æ¯æ bare name (bare id,
 bare path) - [x] refactor: url åè¡¨è½å¤é¢çº¿æ§å±å¼ - [x] feat:
 æ·»å åç§ return code - [x] test: ç¼åååæµè¯ ### 2.0.0 - [ ] feat:
-æç¨¿è§é¢æè¿°æä»¶æ¯æ - [ ] docs: å¯ç±ç
-logoï¼åååï¼æè°ä¼å logo åï¼ï¼ - [ ] docs:
+æç¨¿è§é¢æè¿°æä»¶æ¯æ - [ ] refactor: æ´çè·¯å¾åéå - [ ]
+docs: å¯ç±ç logoï¼åååï¼æè°ä¼å logo åï¼ï¼ - [ ] docs:
 å¯ç±çéæææ¡£ï¼å¯è½éè¦ VitePress å° 1.0ï¼ ### future - [ ]
 feat: å­å¹ãå¼¹å¹åµå¥è§é¢æ¯æï¼ä¹è®¸ï¼ï¼ - [ ] feat:
 å°é¢ä¸è½½æ¯æï¼ä¹è®¸ï¼ï¼ - [ ] refactor:
 ä»¥æä»¶å½¢å¼æ¯ææ´å¤é³è§é¢å¤çæ¹é¢çåè½ï¼æ¯å¦ç±»ä¼¼
 autosub çå·¥å·ï¼ä¹è®¸ï¼ï¼ - [ ] feat: æ´å¤æ¹ä¸è½½æ¯æ - [ ] feat:
 ä»¥åæ´å å¯ç±ï½ ## åè - åºæ¬ç»æï¼
 github.com/SigureMo/bilili> - åç¨ä¸è½½ï¼
```

### Comparing `yutto-2.0.0b8/pyproject.toml` & `yutto-2.0.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yutto"
-version = "2.0.0-beta.8"
+version = "2.0.0-beta.9"
 description = "🧊 一个可爱且任性的 B 站视频下载器"
 authors = ["Nyakku Shigure <sigure.qaq@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/SigureMo/yutto"
 repository = "https://github.com/SigureMo/yutto"
 keywords = ["python", "bilibili", "video", "downloader", "danmaku"]
```

### Comparing `yutto-2.0.0b8/yutto/__main__.py` & `yutto-2.0.0b9/yutto/__main__.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/api/acg_video.py` & `yutto-2.0.0b9/yutto/api/acg_video.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import re
-from typing import Literal, TypedDict
+from typing import TypedDict
 
 from aiohttp import ClientSession
 
 from yutto.api.info import get_video_info
 from yutto.exceptions import NoAccessPermissionError, UnSupportedTypeError
-from yutto.media.codec import VideoCodec
+from yutto.media.codec import audio_codec_map, video_codec_map
 from yutto.typing import AudioUrlMeta, AvId, CId, MultiLangSubtitle, VideoUrlMeta
 from yutto.utils.fetcher import Fetcher
 
 
 class AcgVideoListItem(TypedDict):
     id: int
     name: str
@@ -39,44 +39,44 @@
         for i, item in enumerate(res_json["data"])
     ]
 
 
 async def get_acg_video_playurl(
     session: ClientSession, avid: AvId, cid: CId
 ) -> tuple[list[VideoUrlMeta], list[AudioUrlMeta]]:
-    play_api = "https://api.bilibili.com/x/player/playurl?avid={aid}&bvid={bvid}&cid={cid}&qn=127&type=&otype=json&fnver=0&fnval=2000&fourk=1&eightk=1"
-    codecid_map: dict[Literal[7, 12], VideoCodec] = {7: "avc", 12: "hevc"}
+    # 4048 = 16(useDash) | 64(useHDR) | 128(use4K) | 256(useDolby) | 512(useXXX) | 1024(use8K) | 2048(useAV1)
+    play_api = "https://api.bilibili.com/x/player/playurl?avid={aid}&bvid={bvid}&cid={cid}&qn=127&type=&otype=json&fnver=0&fnval=4048&fourk=1"
 
     async with session.get(play_api.format(**avid.to_dict(), cid=cid), proxy=Fetcher.proxy) as resp:
         if not resp.ok:
             raise NoAccessPermissionError("无法下载该视频（cid: {cid}）".format(cid=cid))
         resp_json = await resp.json()
         if resp_json.get("data") is None:
             raise NoAccessPermissionError("无法下载该视频（cid: {cid}），原因：{msg}".format(cid=cid, msg=resp_json.get("message")))
         if resp_json["data"].get("dash") is None:
             raise UnSupportedTypeError("该视频（cid: {cid}）尚不支持 DASH 格式".format(cid=cid))
         return (
             [
                 {
                     "url": video["base_url"],
                     "mirrors": video["backup_url"] if video["backup_url"] is not None else [],
-                    "codec": codecid_map[video["codecid"]],
+                    "codec": video_codec_map[video["codecid"]],
                     "width": video["width"],
                     "height": video["height"],
                     "quality": video["id"],
                 }
                 for video in resp_json["data"]["dash"]["video"]
             ]
             if resp_json["data"]["dash"]["video"]
             else [],
             [
                 {
                     "url": audio["base_url"],
                     "mirrors": audio["backup_url"] if audio["backup_url"] is not None else [],
-                    "codec": "mp4a",
+                    "codec": audio_codec_map[audio["codecid"]],
                     "width": 0,
                     "height": 0,
                     "quality": audio["id"],
                 }
                 for audio in resp_json["data"]["dash"]["audio"]
             ]
             if resp_json["data"]["dash"]["audio"]
```

### Comparing `yutto-2.0.0b8/yutto/api/bangumi.py` & `yutto-2.0.0b9/yutto/api/bangumi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 import re
-from typing import Any, Literal, TypedDict
+from typing import Any, TypedDict
 
 from aiohttp import ClientSession
 
 from yutto.exceptions import NoAccessPermissionError, UnSupportedTypeError
-from yutto.media.codec import VideoCodec
-from yutto.typing import (
-    AudioUrlMeta,
-    AvId,
-    BvId,
-    CId,
-    EpisodeId,
-    MediaId,
-    MultiLangSubtitle,
-    SeasonId,
-    VideoUrlMeta,
-)
+from yutto.media.codec import audio_codec_map, video_codec_map
+from yutto.typing import AudioUrlMeta, AvId, BvId, CId, EpisodeId, MediaId, MultiLangSubtitle, SeasonId, VideoUrlMeta
 from yutto.utils.console.logger import Logger
 from yutto.utils.fetcher import Fetcher
 from yutto.utils.metadata import MetaData
 from yutto.utils.time import get_time_str_by_now, get_time_str_by_stamp
 
 
 class BangumiListItem(TypedDict):
@@ -94,15 +84,14 @@
     ]
 
 
 async def get_bangumi_playurl(
     session: ClientSession, avid: AvId, episode_id: EpisodeId, cid: CId
 ) -> tuple[list[VideoUrlMeta], list[AudioUrlMeta]]:
     play_api = "https://api.bilibili.com/pgc/player/web/playurl?avid={aid}&bvid={bvid}&ep_id={episode_id}&cid={cid}&qn=127&fnver=0&fnval=16&fourk=1"
-    codecid_map: dict[Literal[7, 12], VideoCodec] = {7: "avc", 12: "hevc"}
 
     async with session.get(
         play_api.format(**avid.to_dict(), cid=cid, episode_id=episode_id), proxy=Fetcher.proxy
     ) as resp:
         if not resp.ok:
             raise NoAccessPermissionError("无法下载该视频（cid: {cid}）".format(cid=cid))
         resp_json = await resp.json()
@@ -113,26 +102,26 @@
         if resp_json["result"]["is_preview"] == 1:
             Logger.warning("视频（cid: {cid}）是预览视频".format(cid=cid))
         return (
             [
                 {
                     "url": video["base_url"],
                     "mirrors": video["backup_url"] if video["backup_url"] is not None else [],
-                    "codec": codecid_map[video["codecid"]],
+                    "codec": video_codec_map[video["codecid"]],
                     "width": video["width"],
                     "height": video["height"],
                     "quality": video["id"],
                 }
                 for video in resp_json["result"]["dash"]["video"]
             ],
             [
                 {
                     "url": audio["base_url"],
                     "mirrors": audio["backup_url"] if audio["backup_url"] is not None else [],
-                    "codec": "mp4a",
+                    "codec": audio_codec_map[audio["codecid"]],
                     "width": 0,
                     "height": 0,
                     "quality": audio["id"],
                 }
                 for audio in resp_json["result"]["dash"]["audio"]
             ],
         )
```

### Comparing `yutto-2.0.0b8/yutto/api/danmaku.py` & `yutto-2.0.0b9/yutto/api/danmaku.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/api/info.py` & `yutto-2.0.0b9/yutto/api/info.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/api/space.py` & `yutto-2.0.0b9/yutto/api/space.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 
 from aiohttp import ClientSession
 
-from yutto.typing import AvId, BvId, FavouriteMetaData, FId, MId
+from yutto.typing import AvId, BvId, FavouriteMetaData, FId, MId, SeriesId
 from yutto.utils.fetcher import Fetcher
 
 
 async def get_uploader_space_all_videos_avids(session: ClientSession, mid: MId) -> list[AvId]:
     space_videos_api = (
         "https://api.bilibili.com/x/space/arc/search?mid={mid}&ps={ps}&tid=0&pn={pn}&order=pubdate&jsonp=jsonp"
     )
@@ -47,7 +47,21 @@
 
 async def get_all_favourites(session: ClientSession, mid: MId) -> list[FavouriteMetaData]:
     api = "https://api.bilibili.com/x/v3/fav/folder/created/list-all?up_mid={mid}"
     json_data = await Fetcher.fetch_json(session, api.format(mid=mid))
     if not json_data["data"]:
         return []
     return [FavouriteMetaData(title=data["title"], fid=FId(str(data["id"]))) for data in json_data["data"]["list"]]
+
+
+async def get_medialist_avids(session: ClientSession, series_id: SeriesId) -> list[AvId]:
+    api = "https://api.bilibili.com/x/v2/medialist/resource/list?type=5&otype=2&biz_id={series_id}"
+    json_data = await Fetcher.fetch_json(session, api.format(series_id=series_id))
+    if not json_data["data"]:
+        return []
+    return [BvId(video_info["bv_id"]) for video_info in json_data["data"]["media_list"]]
+
+
+async def get_medialist_title(session: ClientSession, series_id: SeriesId) -> str:
+    api = "https://api.bilibili.com/x/v1/medialist/info?type=5&biz_id={series_id}"
+    json_data = await Fetcher.fetch_json(session, api.format(series_id=series_id))
+    return json_data["data"]["title"]
```

### Comparing `yutto-2.0.0b8/yutto/cli/batch_get.py` & `yutto-2.0.0b9/yutto/cli/batch_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import argparse
 import sys
 
 import aiohttp
 
-from yutto.api.acg_video import get_acg_video_list, get_acg_video_title, get_acg_video_pubdate
+from yutto.api.acg_video import get_acg_video_list, get_acg_video_pubdate, get_acg_video_title
 from yutto.api.bangumi import (
     get_bangumi_list,
     get_bangumi_title,
     get_season_id_by_episode_id,
     get_season_id_by_media_id,
 )
 from yutto.api.space import (
     get_all_favourites,
     get_favourite_avids,
     get_favourite_info,
+    get_medialist_avids,
+    get_medialist_title,
     get_uploader_name,
     get_uploader_space_all_videos_avids,
 )
 from yutto.cli.get import fetch_acg_video_data, fetch_bangumi_data
 from yutto.exceptions import ErrorCode, HttpStatusError, NoAccessPermissionError, NotFoundError, UnSupportedTypeError
 from yutto.processor.downloader import process_video_download
 from yutto.processor.filter import parse_episodes
@@ -25,17 +27,19 @@
     regexp_acg_video_av,
     regexp_acg_video_bv,
     regexp_bangumi_ep,
     regexp_bangumi_md,
     regexp_bangumi_ss,
     regexp_favourite,
     regexp_favourite_all,
+    regexp_medialist,
+    regexp_series,
     regexp_space_all,
 )
-from yutto.typing import AId, BvId, EpisodeData, EpisodeId, FId, MediaId, MId, SeasonId
+from yutto.typing import AId, BvId, EpisodeData, EpisodeId, FId, MediaId, MId, SeasonId, SeriesId
 from yutto.utils.console.logger import Badge, Logger
 from yutto.utils.fetcher import Fetcher
 from yutto.utils.functiontools import sync
 
 
 @sync
 async def run(args: argparse.Namespace):
@@ -124,29 +128,31 @@
                 acg_video_item
                 for avid in await get_favourite_avids(session, fid)
                 for acg_video_item in await get_acg_video_list(session, avid)
             ]
             for i, acg_video_item in enumerate(acg_video_list):
                 Logger.status.set("正在努力解析第 {}/{} 个视频".format(i + 1, len(acg_video_list)))
                 try:
+                    # 在使用 SESSDATA 时，如果不去事先 touch 一下视频链接的话，是无法获取 episode_data 的
+                    await Fetcher.touch_url(session, acg_video_item["avid"].to_url())
                     title = await get_acg_video_title(session, acg_video_item["avid"])
                     pubdate = await get_acg_video_pubdate(session, acg_video_item["avid"])
                     episode_data = await fetch_acg_video_data(
                         session,
                         acg_video_item["avid"],
                         i + 1,
                         acg_video_item,
                         args,
                         {
                             "title": title,
                             "username": username,
-                            "fav_title": favourite_info["title"],
+                            "series_title": favourite_info["title"],
                             "pubdate": pubdate,
                         },
-                        "{username}的收藏夹/{fav_title}/{title}/{name}",
+                        "{username}的收藏夹/{series_title}/{title}/{name}",
                     )
                 except (NoAccessPermissionError, HttpStatusError, UnSupportedTypeError, NotFoundError) as e:
                     Logger.error(e.message)
                     continue
                 download_list.append(episode_data)
 
         # 匹配为用户全部收藏
@@ -158,27 +164,66 @@
             acg_video_list = [
                 (acg_video_item, fav["title"])
                 for fav in await get_all_favourites(session, mid)
                 for avid in await get_favourite_avids(session, fav["fid"])
                 for acg_video_item in await get_acg_video_list(session, avid)
             ]
 
-            for i, (acg_video_item, fav_title) in enumerate(acg_video_list):
+            for i, (acg_video_item, series_title) in enumerate(acg_video_list):
                 Logger.status.set("正在努力解析第 {}/{} 个视频".format(i + 1, len(acg_video_list)))
                 pubdate = await get_acg_video_pubdate(session, acg_video_item["avid"])
                 try:
+                    await Fetcher.touch_url(session, acg_video_item["avid"].to_url())
                     title = await get_acg_video_title(session, acg_video_item["avid"])
                     episode_data = await fetch_acg_video_data(
                         session,
                         acg_video_item["avid"],
                         i + 1,
                         acg_video_item,
                         args,
-                        {"title": title, "username": username, "fav_title": fav_title, "pubdate": pubdate},
-                        "{username}的收藏夹/{fav_title}/{title}/{name}",
+                        {"title": title, "username": username, "series_title": series_title, "pubdate": pubdate},
+                        "{username}的收藏夹/{series_title}/{title}/{name}",
+                    )
+                except (NoAccessPermissionError, HttpStatusError, UnSupportedTypeError, NotFoundError) as e:
+                    Logger.error(e.message)
+                    continue
+                download_list.append(episode_data)
+
+        # 匹配为视频合集
+        elif (match_obj := regexp_medialist.match(url)) or (match_obj := regexp_series.match(url)):
+            mid = MId(match_obj.group("mid"))
+            series_id = SeriesId(match_obj.group("series_id"))
+            username = await get_uploader_name(session, mid)
+            series_title = await get_medialist_title(session, series_id)
+            Logger.custom(series_title, Badge("视频合集", fore="black", back="cyan"))
+
+            acg_video_list = [
+                acg_video_item
+                for avid in await get_medialist_avids(session, series_id)
+                for acg_video_item in await get_acg_video_list(session, avid)
+            ]
+            for i, acg_video_item in enumerate(acg_video_list):
+                Logger.status.set("正在努力解析第 {}/{} 个视频".format(i + 1, len(acg_video_list)))
+                try:
+                    await Fetcher.touch_url(session, acg_video_item["avid"].to_url())
+                    title = await get_acg_video_title(session, acg_video_item["avid"])
+                    pubdate = await get_acg_video_pubdate(session, acg_video_item["avid"])
+                    episode_data = await fetch_acg_video_data(
+                        session,
+                        acg_video_item["avid"],
+                        i + 1,
+                        acg_video_item,
+                        args,
+                        {
+                            "series_title": series_title,
+                            "username": username,  # 虽然默认模板的用不上，但这里可以提供一下
+                            "title": title,
+                            "pubdate": pubdate,
+                        },
+                        "{series_title}/{title}/{name}",
                     )
                 except (NoAccessPermissionError, HttpStatusError, UnSupportedTypeError, NotFoundError) as e:
                     Logger.error(e.message)
                     continue
                 download_list.append(episode_data)
 
         # 匹配为 UP 主个人空间
@@ -192,14 +237,15 @@
                 for avid in await get_uploader_space_all_videos_avids(session, mid)
                 for acg_video_item in await get_acg_video_list(session, avid)
             ]
 
             for i, acg_video_item in enumerate(acg_video_list):
                 Logger.status.set("正在努力解析第 {}/{} 个视频".format(i + 1, len(acg_video_list)))
                 try:
+                    await Fetcher.touch_url(session, acg_video_item["avid"].to_url())
                     title = await get_acg_video_title(session, acg_video_item["avid"])
                     pubdate = await get_acg_video_pubdate(session, acg_video_item["avid"])
                     episode_data = await fetch_acg_video_data(
                         session,
                         acg_video_item["avid"],
                         i + 1,
                         acg_video_item,
```

### Comparing `yutto-2.0.0b8/yutto/cli/checker.py` & `yutto-2.0.0b9/yutto/cli/checker.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/cli/get.py` & `yutto-2.0.0b9/yutto/cli/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     danmaku = await get_danmaku(session, cid, args.danmaku_format) if not args.no_danmaku else EmptyDanmakuData
     metadata = bangumi_info["metadata"] if args.with_metadata else None
     subpath_variables_base: PathTemplateVariableDict = {
         "id": id,
         "name": name,
         "title": UNKNOWN,
         "username": UNKNOWN,
-        "fav_title": UNKNOWN,
+        "series_title": UNKNOWN,
         "pubdate": UNKNOWN,
     }
     subpath_variables_base.update(subpath_variables)
     subpath = resolve_path_template(args.subpath_template, auto_subpath_template, subpath_variables_base)
     output_dir, filename = os.path.split(os.path.join(args.dir, subpath))
     return EpisodeData(
         videos=videos,
@@ -106,15 +106,15 @@
         Logger.warning("目前仅支持番剧 metadata 生成")
     metadata = None
     subpath_variables_base: PathTemplateVariableDict = {
         "id": id,
         "name": name,
         "title": UNKNOWN,
         "username": UNKNOWN,
-        "fav_title": UNKNOWN,
+        "series_title": UNKNOWN,
         "pubdate": UNKNOWN,
     }
     subpath_variables_base.update(subpath_variables)
     subpath = resolve_path_template(args.subpath_template, auto_subpath_template, subpath_variables_base)
     output_dir, filename = os.path.split(os.path.join(args.dir, subpath))
     return EpisodeData(
         videos=videos,
```

### Comparing `yutto-2.0.0b8/yutto/exceptions.py` & `yutto-2.0.0b9/yutto/exceptions.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/processor/downloader.py` & `yutto-2.0.0b9/yutto/processor/downloader.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/processor/filter.py` & `yutto-2.0.0b9/yutto/processor/filter.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/processor/path_resolver.py` & `yutto-2.0.0b9/yutto/processor/path_resolver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from html import unescape
 from typing import Literal, Union
 
 from yutto.utils.console.logger import Logger
 
 path_template_variables = ["title", "id", "name", "username"]
-PathTemplateVariable = Literal["title", "id", "name", "username", "fav_title", "pubdate"]
+PathTemplateVariable = Literal["title", "id", "name", "username", "series_title", "pubdate"]
 PathTemplateVariableDict = dict[PathTemplateVariable, Union[int, str]]
 UNKNOWN: str = "unknown_variable"
 
 _count: int = 0
 
 
 def repair_filename(filename: str) -> str:
@@ -46,14 +46,18 @@
         _count += 1
     return filename
 
 
 def resolve_path_template(
     path_template: str, auto_path_template: str, subpath_variables: PathTemplateVariableDict
 ) -> str:
+    # fav_title 已经被 series_title 取代
+    if "{fav_title}" in path_template:
+        Logger.deprecated_warning("路径变量 fav_title 已经被废除，已自动使用 series_title 替代（2.0.0 后将会彻底废除 fav_title）")
+        path_template = path_template.replace("{fav_title}", "{series_title}")
     # 保证所有传进来的值都满足路径要求
     for key, value in subpath_variables.items():
         # 只对字符串值修改，int 型不修改以适配高级模板
         if isinstance(value, str):
             if f"{{{key}}}" in path_template and value == UNKNOWN:
                 Logger.warning("使用了未知的变量，可能导致产生错误的下载路径")
             subpath_variables[key] = repair_filename(value)
```

### Comparing `yutto-2.0.0b8/yutto/processor/progressbar.py` & `yutto-2.0.0b9/yutto/processor/progressbar.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/processor/urlparser.py` & `yutto-2.0.0b9/yutto/processor/urlparser.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 regexp_acg_video_bv = re.compile(r"https?://www\.bilibili\.com/video/(?P<bvid>(bv|BV)\w+)(\?p=(?P<page>\d+))?")
 regexp_bangumi_md = re.compile(r"https?://www\.bilibili\.com/bangumi/media/md(?P<media_id>\d+)")
 regexp_bangumi_ep = re.compile(r"https?://www\.bilibili\.com/bangumi/play/ep(?P<episode_id>\d+)")
 regexp_bangumi_ss = re.compile(r"https?://www\.bilibili\.com/bangumi/play/ss(?P<season_id>\d+)")
 regexp_space_all = re.compile(r"https?://space\.bilibili\.com/(?P<mid>\d+)(/video)?")
 regexp_favourite_all = re.compile(r"https?://space\.bilibili\.com/(?P<mid>\d+)/favlist")
 regexp_favourite = re.compile(r"https?://space\.bilibili\.com/(?P<mid>\d+)/favlist\?fid=(?P<fid>\d+)")
+regexp_medialist = re.compile(
+    r"https?://www\.bilibili\.com/medialist/play/(?P<mid>\d+)\?business=space_series&business_id=(?P<series_id>\d+)"
+)
+regexp_series = re.compile(r"https?://space\.bilibili\.com/(?P<mid>\d+)/channel/seriesdetail\?sid=(?P<series_id>\d+)")
 
 regexp_acg_video_av_bare = re.compile(r"av(?P<aid>\d+)(\?p=(?P<page>\d+))?")
 regexp_acg_video_bv_bare = re.compile(r"(?P<bvid>(bv|BV)\w+)(\?p=(?P<page>\d+))?")
 regexp_bangumi_md_bare = re.compile(r"md(?P<media_id>\d+)")
 regexp_bangumi_ep_bare = re.compile(r"ep(?P<episode_id>\d+)")
 regexp_bangumi_ss_bare = re.compile(r"ss(?P<season_id>\d+)")
```

### Comparing `yutto-2.0.0b8/yutto/typing.py` & `yutto-2.0.0b9/yutto/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,31 +22,40 @@
 
 class AvId(BilibiliId):
     """AID 与 BVID 的统一，大多数 API 只需要其中一种即可正常工作"""
 
     def to_dict(self) -> dict[str, str]:
         raise NotImplementedError("请不要直接使用 AvId")
 
+    def to_url(self) -> str:
+        raise NotImplementedError("请不要直接使用 AvId")
+
 
 class AId(AvId):
     """AID"""
 
     def to_dict(self):
         return {"aid": self.value, "bvid": ""}
 
+    def to_url(self) -> str:
+        return f"https://www.bilibili.com/video/av{self.value}"
+
 
 class BvId(AvId):
     """BVID"""
 
     def to_dict(self):
         return {
             "aid": "",
             "bvid": self.value,
         }
 
+    def to_url(self) -> str:
+        return f"https://www.bilibili.com/video/{self.value}"
+
 
 class CId(BilibiliId):
     """视频 ID"""
 
     def to_dict(self):
         return {"cid": self.value}
 
@@ -82,14 +91,21 @@
 class FId(BilibiliId):
     """收藏夹 ID"""
 
     def to_dict(self):
         return {"fid": self.value}
 
 
+class SeriesId(BilibiliId):
+    """视频合集 ID"""
+
+    def to_dict(self):
+        return {"series_id": self.value}
+
+
 class VideoUrlMeta(TypedDict):
     url: str
     mirrors: list[str]
     codec: VideoCodec
     width: int
     height: int
     quality: VideoQuality
```

### Comparing `yutto-2.0.0b8/yutto/utils/asynclib.py` & `yutto-2.0.0b9/yutto/utils/asynclib.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/console/attributes.py` & `yutto-2.0.0b9/yutto/utils/console/attributes.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/console/colorful.py` & `yutto-2.0.0b9/yutto/utils/console/colorful.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/console/formatter.py` & `yutto-2.0.0b9/yutto/utils/console/formatter.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/console/logger.py` & `yutto-2.0.0b9/yutto/utils/console/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def __add__(self, other: str) -> str:
         return str(self) + other
 
 
 WARNING_BADGE = Badge("WARN", fore="yellow")
 ERROR_BADGE = Badge("ERROR", fore="red", style=["bold"])
 INFO_BADGE = Badge("INFO", fore="bright_blue")
+DEPRECATED_BADGE = Badge("DEPRECATED", fore="black", back="yellow")
 DEBUG_BADGE = Badge("DEBUG", fore="green")
 
 
 class Logger:
     status = StatusBar
 
     @classmethod
@@ -67,14 +68,18 @@
         Logger.custom(string, ERROR_BADGE, *print_args, **print_kwargs)
 
     @classmethod
     def info(cls, string: Any, *print_args: Any, **print_kwargs: Any):
         Logger.custom(string, INFO_BADGE, *print_args, **print_kwargs)
 
     @classmethod
+    def deprecated_warning(cls, string: Any, *print_args: Any, **print_kwargs: Any):
+        Logger.custom(string, DEPRECATED_BADGE, *print_args, **print_kwargs)
+
+    @classmethod
     def debug(cls, string: Any, *print_args: Any, **print_kwargs: Any):
         if not _logger_debug:
             return
         Logger.custom(string, DEBUG_BADGE, *print_args, **print_kwargs)
 
     @classmethod
     def custom_multiline(cls, string: Any, badge: Badge, *print_args: Any, **print_kwargs: Any):
@@ -94,14 +99,18 @@
         Logger.custom_multiline(string, ERROR_BADGE, *print_args, **print_kwargs)
 
     @classmethod
     def info_multiline(cls, string: Any, *print_args: Any, **print_kwargs: Any):
         Logger.custom_multiline(string, INFO_BADGE, *print_args, **print_kwargs)
 
     @classmethod
+    def deprecated_warning_multiline(cls, string: Any, *print_args: Any, **print_kwargs: Any):
+        Logger.custom_multiline(string, DEPRECATED_BADGE, *print_args, **print_kwargs)
+
+    @classmethod
     def debug_multiline(cls, string: Any, *print_args: Any, **print_kwargs: Any):
         if not _logger_debug:
             return
         Logger.custom_multiline(string, INFO_BADGE, *print_args, **print_kwargs)
 
     @classmethod
     def print(cls, string: Any, *print_args: Any, **print_kwargs: Any):
```

### Comparing `yutto-2.0.0b8/yutto/utils/console/status_bar.py` & `yutto-2.0.0b9/yutto/utils/console/status_bar.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/danmaku.py` & `yutto-2.0.0b9/yutto/utils/danmaku.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/fetcher.py` & `yutto-2.0.0b9/yutto/utils/fetcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
     def __call__(self, connect_once: Callable[..., Coroutine[Any, Any, T]]) -> Callable[..., Coroutine[Any, Any, T]]:
         async def connect_n_times(*args: Any, **kwargs: Any) -> T:
             retry = self.max_retry + 1
             while retry:
                 try:
                     return await connect_once(*args, **kwargs)
-                except asyncio.TimeoutError as e:
-                    Logger.warning("抓取超时，正在重试")
+                except asyncio.TimeoutError:
+                    Logger.warning(f"抓取超时，正在重试，剩余 {retry - 1} 次")
                 finally:
                     retry -= 1
             raise MaxRetryError("超出最大重试次数！")
 
         return connect_n_times
 
 
 class Fetcher:
     proxy: Optional[str] = None
     trust_env: bool = True
     headers: dict[str, str] = {
-        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.54 Safari/537.36",
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/97.0.4692.71 Safari/537.36",
         "Referer": "https://www.bilibili.com",
     }
     cookies = {}
 
     @classmethod
     def set_proxy(cls, proxy: Union[Literal["no", "auto"], str]):
         if proxy == "auto":
@@ -100,14 +100,24 @@
         ) as resp:
             if resp.status == 206:
                 return int(resp.headers["Content-Range"].split("/")[-1])
             else:
                 return None
 
     @classmethod
+    @MaxRetry(2)
+    async def touch_url(cls, session: ClientSession, url: str):
+        async with session.get(
+            url,
+            proxy=Fetcher.proxy,
+            ssl=False,
+        ) as resp:
+            resp.close()
+
+    @classmethod
     async def download_file_with_offset(
         cls,
         session: ClientSession,
         url: str,
         mirrors: list[str],
         file_buffer: AsyncFileBuffer,
         offset: int,
@@ -146,16 +156,16 @@
                     else:
                         chunk = await resp.read()
                         await file_buffer.write(chunk, offset + block_offset)
                         block_offset += len(chunk)
                 # TODO: 是否需要校验总大小
                 done = True
 
-            except asyncio.TimeoutError as e:
-                Logger.warning("文件 {} 下载超时，尝试重新连接...".format(file_buffer.file_path))
-
             except (
                 aiohttp.client_exceptions.ClientPayloadError,
                 aiohttp.client_exceptions.ServerDisconnectedError,
-            ) as e:
+            ):
                 await asyncio.sleep(0.5)
                 Logger.warning("文件 {} 下载出错，尝试重新连接...".format(file_buffer.file_path))
+
+            except asyncio.TimeoutError:
+                Logger.warning("文件 {} 下载超时，尝试重新连接...".format(file_buffer.file_path))
```

### Comparing `yutto-2.0.0b8/yutto/utils/ffmpeg.py` & `yutto-2.0.0b9/yutto/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/file_buffer.py` & `yutto-2.0.0b9/yutto/utils/file_buffer.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/functiontools/aobject.py` & `yutto-2.0.0b9/yutto/utils/functiontools/aobject.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/functiontools/sync.py` & `yutto-2.0.0b9/yutto/utils/functiontools/sync.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/metadata.py` & `yutto-2.0.0b9/yutto/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/yutto/utils/subtitle.py` & `yutto-2.0.0b9/yutto/utils/subtitle.py`

 * *Files identical despite different names*

### Comparing `yutto-2.0.0b8/setup.py` & `yutto-2.0.0b9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 {'uvloop': ['uvloop==0.16.0']}
 
 entry_points = \
 {'console_scripts': ['yutto = yutto.__main__:main']}
 
 setup_kwargs = {
     'name': 'yutto',
-    'version': '2.0.0b8',
+    'version': '2.0.0b9',
     'description': '🧊 一个可爱且任性的 B 站视频下载器',
-    'long_description': '# yutto<sup>2.0.0-beta</sup>\n\n<p align="center">\n   <a href="https://python.org/" target="_blank"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/yutto?logo=python&style=flat-square"></a>\n   <a href="https://pypi.org/project/yutto/" target="_blank"><img src="https://img.shields.io/pypi/v/yutto?style=flat-square" alt="pypi"></a>\n   <a href="https://pypi.org/project/yutto/" target="_blank"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/yutto?style=flat-square"></a>\n   <a href="LICENSE"><img alt="LICENSE" src="https://img.shields.io/github/license/SigureMo/yutto?style=flat-square"></a>\n   <a href="https://github.com/psf/black"><img alt="black" src="https://img.shields.io/badge/code%20style-black-000000?style=flat-square"></a>\n   <a href="https://gitmoji.dev"><img src="https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67?style=flat-square" alt="Gitmoji"></a>\n</p>\n\nyutto，一个可爱且任性的 B 站下载器（CLI）\n\n## 版本号为什么是 2.0\n\n因为 yutto 是 bilili 的後輩呀～\n\n## 安装预览版\n\n在此之前请确保安装 Python3.9 及以上版本，并配置好 FFmpeg（参照 [bilili 文档](https://bilili.sigure.xyz/guide/getting-started.html)）\n\n当前 yutto 尚处于 beta 阶段，有任何建议尽管在 [Discussions](https://github.com/SigureMo/yutto/discussions) 提出～～～\n\n### pip 安装\n\n```bash\npip install --pre yutto\n```\n\n### git clone\n\n```bash\ngit clone https://github.com/SigureMo/yutto.git\ncd yutto/\npip install poetry\npoetry build\npip install ./dist/yutto-*.whl\n```\n\n## 主要功能\n\n### 已支持的下载类型\n\n<!-- prettier-ignore -->\n|type|batch|path template|\n|-|-|-|\n|投稿视频|:x:|`{title}`|\n|投稿视频|:white_check_mark:|`{title}/{name}`|\n|番剧|:x:|`{name}`|\n|番剧|:white_check_mark:|`{title}/{name}`|\n|用户指定收藏夹|:white_check_mark:|`{username}的收藏夹/{fav_title}/{title}/{name}`|\n|用户全部收藏夹|:white_check_mark:|`{username}的收藏夹/{fav_title}/{title}/{name}`|\n|UP 主个人空间|:white_check_mark:|`{username}的全部投稿视频/{title}/{name}`|\n\n<!-- TODO: 展示更多细节 -->\n\n### 基本命令\n\nyutto 的基本命令如下：\n\n```bash\nyutto <url>\n```\n\n你可以通过 `yutto -h` 查看详细命令参数。\n\n如果你需要下载**单个**视频，只需要使用 yutto 加上这个视频的地址即可。它支持 av/BV 号以及相应带 p=n 参数的投稿视频页面，也支持 ep 号（episode_id）的番剧页面。\n\n比如只需要这样你就可以下载[《転スラ日記》](https://www.bilibili.com/bangumi/play/ep395211)第一话：\n\n```bash\nyutto https://www.bilibili.com/bangumi/play/ep395211\n```\n\nyutto 还支持直接使用能够唯一定位资源的 id 来作为 `<url>`，刚刚的功能与下面的简化后的命令功能是完全一样的\n\n```bash\nyutto ep395211\n```\n\n不过有时你可能想要批量下载很多剧集，因此 yutto 提供了用于批量下载的参数 `-b/--batch`，它不仅支持前面所说的单个视频所在页面地址（会解析该单个视频所在的系列视频），还支持一些明确用于表示系列视频的地址，比如 md 页面（media_id）、ss 页面（season_id）。\n\n比如像下面这样就可以下载《転スラ日記》所有已更新的剧集：\n\n```bash\nyutto --batch https://www.bilibili.com/bangumi/play/ep395211\n```\n\n### 基础参数\n\n> 大部分参数与 bilili 重合，可参考 [bilili 的 cli 文档](https://bilili.nyakku.moe/cli/)\n\nyutto 支持一些基础参数，无论是批量下载还是单视频下载都适用。\n\n<details>\n<summary>点击展开详细参数</summary>\n\n#### 最大并行 worker 数量\n\n-  参数 `-n` 或 `--num-workers`\n-  默认值 `8`\n\n与 bilili 不同的是，yutto 并不是使用多线程实现并行下载，而是使用协程实现的，本参数限制的是最大的并行 Worker 数量。\n\n#### 指定视频清晰度等级\n\n-  参数 `-q` 或 `--video-quality`\n-  可选值 `127 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16`\n-  默认值 `127`\n\n清晰度对应关系如下\n\n<!-- prettier-ignore -->\n|code|清晰度|\n|:-:|:-:|\n|127|8K 超高清|\n|125|HDR 真彩|\n|120|4K 超清|\n|116|1080P 60帧|\n|112|1080P 高码率|\n|80|1080P 高清|\n|74|720P 60帧|\n|64|720P 高清|\n|32|480P 清晰|\n|16|360P 流畅|\n\n并不是说指定某个清晰度就一定会下载该清晰度的视频，yutto 只会尽可能满足你的要求，如果不存在指定的清晰度，yutto 就会按照默认的清晰度搜索机制进行调节，比如指定清晰度为 `80`，**首先会依次降清晰度搜索** `74`、`64`、`32`、`16`，如果依然找不到合适的则**继续升清晰度搜索** `112`、`116`、`120`、`125`、`127`。\n\n#### 指定音频码率等级\n\n-  参数 `-aq` 或 `--audio-quality`\n-  可选值 `30280 | 30232 | 30216`\n-  默认值 `30280`\n\n码率对应关系如下\n\n<!-- prettier-ignore -->\n|code|码率|\n|:-:|:-:|\n|30280|320kbps|\n|30232|128kbps|\n|30216|64kbps|\n\n清晰度自动调节机制与视频清晰度一致，也采用先降后升的匹配机制。\n\n#### 指定视频编码\n\n-  参数 `--vcodec`\n-  下载编码可选值 `"hevc" | "avc"`\n-  保存编码可选值 FFmpeg 所有可用的视频编码器\n-  默认值 `"avc:copy"`\n\n该参数略微复杂，前半部分表示在下载时**优先**选择哪一种编码的视频流，后半部分则表示在合并时如何编码视频流，两者使用 `:` 分隔。\n\n值得注意的是，前半的下载编码只是优先下载的编码而已，如果不存在该编码，则仍会像视频清晰度调节机制一样自动选择其余编码。\n\n而后半部分的参数如果设置成非 `copy` 的值则可以确保在下载完成后对其进行重新编码，而且不止支持 `hevc` 与 `avc`，只要你的 FFmpeg 支持的视频编码器，它都可以完成。\n\n#### 指定音频编码\n\n-  参数 `--acodec`\n-  下载编码可选值 `"mp4a"`\n-  保存编码可选值 FFmpeg 所有可用的音频编码器\n-  默认值 `"mp4a:copy"`\n\n详情同视频编码。\n\n#### 仅下载视频流\n\n-  参数 `--video-only`\n-  默认值 `False`\n\n#### 仅下载音频流\n\n-  参数 `--audio-only`\n-  默认值 `False`\n\n仅下载其中的音频流，保存为 `.aac` 文件。\n\n值得注意的是，在不选择视频流时，嵌入字幕、弹幕功能将无法工作。\n\n#### 弹幕格式选择\n\n-  参数 `-df` 或 `--danmaku-format`\n-  可选值 `"ass" | "xml" | "protobuf"`\n-  默认值 `"ass"`\n\nB 站提供了 `xml` 与 `protobuf` 两种弹幕数据接口，yutto 会自动下载 `xml` 格式弹幕并转换为 `ass` 格式，如果你不喜欢 yutto 自动转换的效果，可以选择输出格式为 `xml` 或 `protobuf`，手动通过一些工具进行转换，比如 yutto 和 bilili 所使用的 [biliass](https://github.com/ShigureLab/biliass)，或者使用 [us-danmaku](https://tiansh.github.io/us-danmaku/bilibili/) 进行在线转换。\n\n如果你不想下载弹幕，只需要使用参数 `--no-danmaku` 即可。\n\n#### 下载块大小\n\n-  参数 `-bs` 或 `--block-size`\n-  默认值 `0.5`\n\n以 MiB 为单位，为分块下载时各块大小，不建议更改。\n\n#### 强制覆盖已下载文件\n\n-  参数 `-w` 或 `--overwrite`\n-  默认值 `False`\n\n#### 代理设置\n\n-  参数 `-x` 或 `--proxy`\n-  可选值 `"auto" | "no" | <https?://url/to/proxy/server>`\n-  默认值 `"auto"`\n\n设置代理服务器，默认是从环境变量读取，`no` 则为不设置代理，设置其它 http/https url 则将其作为代理服务器。\n\n#### 存放根目录\n\n-  参数 `-d` 或 `--dir`\n-  默认值 `"./"`\n\n#### 临时文件目录\n\n-  参数 `--tmp-dir`\n-  默认值是“存放根目录”即 `-d, --dir` 的值\n\n#### 存放子路径模板\n\n-  参数 `-tp` 或 `--subpath-template`\n-  可选参数变量 `title | id | name | username | fav_title | pubdate` （以后可能会有更多）\n-  默认值 `"{auto}"`\n\n通过配置子路径模板可以灵活地控制视频存放位置。\n\n默认情况是由 yutto 自动控制存放位置的。比如下载单个视频时默认就是直接存放在设定的根目录，不会创建一层容器目录，此时自动选择了 `{name}` 作为模板；而批量下载时则会根据视频层级生成多级目录，比如番剧会是 `{title}/{name}`，首先会在设定根目录里生成一个番剧名的目录，其内才会存放各个番剧剧集视频，这样方便了多个不同番剧的管理。当然，如果你仍希望将番剧直接存放在设定根目录下的话，可以修改该参数值为 `{name}`即可。\n\n另外，该功能语法由 Python format 函数模板语法提供，所以也支持一些高级的用法，比如 `{id:0>3}{name}`。\n\n值得注意的是，并不是所有变量在各种场合下都会提供，比如 `username` 变量当前仅在 UP 主全部投稿视频/收藏夹才提供，在其它情况下不应使用它。各变量详细作用域描述见下表：\n\n<!-- prettier-ignore -->\n|Variable|Description|Scope|\n|-|-|-|\n|title|系列视频总标题（番剧名/投稿视频标题）|全部|\n|id|系列视频单 p 顺序标号|全部|\n|name|系列视频单 p 标题|全部|\n|username|UP 主用户名|个人空间、收藏夹下载|\n|pubdate|投稿日期|仅投稿视频|\n\n#### url 别名文件路径\n\n-  参数 `-af` 或 `--alias-file`\n-  默认值 `None`\n\n指定别名文件路径，别名文件中存放一个别名与其对应的 url，使用空格或者 `=` 分隔，示例如下：\n\n```\nrimuru1=https://www.bilibili.com/bangumi/play/ss25739/\nrimuru2=https://www.bilibili.com/bangumi/play/ss36170/\nrimuru-nikki=https://www.bilibili.com/bangumi/play/ss38221/\n```\n\n比如将上述内容存储到 `~/.yutto_alias`，则通过以下命令即可解析该文件：\n\n```bash\nyutto rimuru1 --batch --alias-file=\'~/.yutto_alias\'\n```\n\n当参数值为 `-` 时，会从标准输入中读取：\n\n```bash\ncat ~/.yutto_alias | yutto rimuru-nikki --batch --alias-file -\n```\n\n#### Cookies 设置\n\n-  参数 `-c` 或 `--sessdata`\n-  默认值 `""`\n\n设置 Cookies 后你才可以下载更高清晰度以及更多的剧集，当你传入你的大会员 `SESSDATA` 时（当然前提是你是大会员），你就可以下载大会员可访问的资源咯。\n\n<details><summary> SESSDATA 获取方式 </summary>\n\n这里用 Chrome 作为示例，其它浏览器请尝试类似方法。\n\n首先，用你的帐号登录 B 站，然后随便打开一个 B 站网页，比如[首页](https://www.bilibili.com/)。\n\n按 F12 打开开发者工具，切换到 Network 栏，刷新页面，此时第一个加载的资源应该就是当前页面的 html，选中该资源，在右侧 「Request Headers」 中找到 「cookie」，在其中找到类似于 `SESSDATA=d8bc7493%2C2843925707%2C08c3e*81;` 的一串字符串，复制这里的 `d8bc7493%2C2843925707%2C08c3e*81`，这就是你需要的 `SESSDATA`。\n\n</details>\n\n另外，由于 SESSDATA 中可能有特殊符号，所以传入时你可能需要使用双引号来包裹\n\n```bash\nyutto <url> -c "d8bc7493%2C2843925707%2C08c3e*81"\n```\n\n当然，示例里的 SESSDATA 是无效的，请使用自己的 SESSDATA。\n\n#### 不下载弹幕\n\n-  参数 `--no-danmaku`\n-  默认值 `False`\n\n#### 不下载字幕\n\n-  参数 `--no-subtitle`\n-  默认值 `False`\n\n#### 不显示颜色\n\n-  参数 `--no-color`\n-  默认值 `False`\n\n#### 启用 Debug 模式\n\n-  参数 `--debug`\n-  默认值 `False`\n\n#### 生成媒体元数据文件\n\n-  参数 `--with-metadata`\n-  默认值 `False`\n\n</details>\n\n### 批量参数\n\n有些参数是只有批量下载时才可以使用的\n\n<details>\n<summary>点击展开详细参数</summary>\n\n#### 启用批量下载\n\n-  参数 `-b` 或 `--batch`\n-  默认值 `False`\n\n只需要 `yutto --batch <url>` 即可启用批量下载功能。\n\n#### 选集\n\n-  参数 `-p` 或 `--episodes`\n-  默认值 `^~$`\n\n-  参数 `-p` 或 `--episodes`\n-  默认值 `^~$`（也即全选）\n\n也就是选集咯，其语法是这样的\n\n-  `<p1>` 单独下某一剧集\n   -  支持负数来选择倒数第几话\n   -  此外还可以使用 `^` 与 `$` 来分别代表 `1` 与 `-1`\n-  `<p_start>~<p_end>` 使用 `~` 可以连续选取\n-  `<p1>,<p2>,<p3>,...,<pn>` 使用 `,` 可以不连续选取\n\nemmm，直接看的话大概并不能知道我在说什么，所以我们通过几个小例子来了解其语法\n\n```bash\n# 假设要下载一个具有 24 话的番剧\n# 如果我们只想下载第 3 话，只需要这样\nyutto <url> -b -p 3\n# 那如果我想下载第 5 话到第 7 话呢，使用 `~` 可以连续选中\nyutto <url> -b -p 5~7\n# 那我想下载第 12 话和第 17 话又要怎么办？此时只需要 `,` 就可以将多个不连续的选集一起选中\nyutto <url> -b -p 12,17\n# 那我突然又想将刚才那些都选中了呢？还是使用 `,` 呀，将它们连在一起即可\nyutto <url> -b -p 3,5~7,12,17\n# 嗯，你已经把基本用法都了解过了，很简单吧～\n# 下面是一些语法糖，不了解也完全不会影响任何功能哒～\n# 那如果我只知道我想下载倒数第 3 话，而不想算倒数第三话是第几话应该怎么办？\n# 此时可以用负数哒～不过要注意的是，开头如果是 `-` 的话前面应该使用 `=`\nyutto <url> -b -p=-3\n# 那么如果想下载最后一话你可能会想到 `-p=-1` 对吧？不过我内置了两个符号分别代表第一话（^）和最后一话（$）\n# 像下面这样就可以直接下载最后一话啦～\nyutto <url> -b -p $\n# 所有语法都了解完啦，我们看一个稍微复杂的例子\nyutto <url> -b -p ^~3,10,12~14,16,-4~$\n# 很明显，上面的例子就是下载前 3 话、第 10 话、第 12 到 14 话、第 16 话以及后 4 话\n```\n\n下面是一些要注意的问题\n\n1. 这里使用的序号是视频的顺序序号，而不是番剧所标注的`第 n 话`，因为有可能会出现 `第 x.5 话` 等等的特殊情况，此时一定要按照顺序自行计数。\n2. 参数值里一定不要加空格\n3. 参数值开头为 `-` 时前面应该使用 `=` 而非空格\n\n#### 同时下载附加剧集\n\n-  参数 `-s` 或 `--with-section`\n-  默认值 `False`\n\n</details>\n\n## 从 bilili1.x 迁移\n\n### 取消的功能\n\n-  `- bilibili` 目录的生成\n-  播放列表生成\n-  源格式修改功能（不再支持 flv 源视频下载，如果仍有视频不支持 dash 源，请继续使用 bilili）\n-  对 Python3.8 的支持，最低支持 Python3.9\n-  下载前询问\n\n### 默认行为的修改\n\n-  使用协程而非多线程进行下载，同时也不是批量解析批量下载，而是边解析边下载\n-  默认生成弹幕为 ASS\n-  默认启用从多镜像源下载的特性\n-  不仅可以控制是否使用系统代理，还能配置特定的代理服务器\n\n### 新增的特性\n\n-  单视频下载与批量下载命令分离（`bilili` 命令与 `yutto --batch` 相类似）\n-  音频/视频编码选择\n-  仅下载音频/视频\n-  存放子路径的自由定制\n-  支持 url alias\n-  支持 file scheme\n-  更多的批下载支持（现已支持 UP 主全部视频下载，扩展其它批下载支持也很简单）\n-  更加完善的 warning 与 error 提示\n-  支持仅输入 id 即可下载（aid、bvid、episode_id 等）\n-  支持描述文件生成（当前仅番剧）\n\n## 小技巧\n\n### 使用 uvloop 提升协程效率\n\n听说 uvloop 可以提高协程效率，如果你的系统非 Windows 的话，可以试一下安装 uvloop：\n\n```bash\npip install uvloop\n```\n\n现在再运行就会发现不会弹出「没有安装 uvloop 的」 warning 了，至于具体提升多少我也不太清楚啦，没有测过\n\n### 使用 url alias\n\nyutto 新增的 url alias 可以让你下载正在追的番剧时不必每次都打开浏览器复制 url，只需要将追番列表存储在一个文件中，并为这些 url 起一个别名即可\n\n```\nrimuru-nikki=https://www.bilibili.com/bangumi/play/ss38221/\n```\n\n之后下载最新话只需要\n\n```\nyutto --batch rimuru-nikki --alias-file=/path/to/alias-file\n```\n\n### 使用文件列表\n\n现在 url 不仅支持 http/https 链接与裸 id，还支持使用文件路径与 file scheme 来用于表示文件列表，文件列表以行分隔，每行写一次命令的参数，该参数会覆盖掉主程序中所使用的参数，示例如下：\n\n首先将下面的文件存储到一个地方\n\n```\nhttps://www.bilibili.com/bangumi/play/ss38221/ --batch -p $\nhttps://www.bilibili.com/bangumi/play/ss38260/ --batch -p $\n```\n\n然后运行\n\n```\nyutto file:///path/to/list\n```\n\n即可分别下载这两个番剧的最新一话\n\n或者直接使用相对或者绝对路径也是可以的\n\n```\nyutto ./path/to/list\n```\n\n值得注意的是，在文件列表各项里的参数优先级是高于命令里的优先级的，比如文件中使用：\n\n```\nrimuru1 --batch -p $ --no-danmaku --vcodec="hevc:copy"\nrimuru2 --batch -p $\n```\n\n而命令中则使用\n\n```\nyutto file:///path/to/list --vcodec="avc:copy"\n```\n\n最终下载的 rimuru1 会是 "hevc:copy"，而 rimuru2 则会是 "avc:copy"\n\n另外，文件列表也是支持 alias 的，你完全可以为该列表起一个别名，一个比较特别的用例是将你所有追番的内容放在一个文件里，然后为该文件起一个别名（比如 `subscription`），这样只需要 `yutto subscription --alias-file path/to/alias/file` 就可以达到追番效果啦～\n\n最后，列表也是支持嵌套的哦（虽然没什么用 2333）\n\n## FAQ\n\n### 名字的由来\n\n[《転スラ日記》第一话 00:24](https://www.bilibili.com/bangumi/play/ep395211?t=24)\n\n### yutto 会很快替代 bilili 吗\n\n短期内不会，bilili 并不会消失，在一段时间内 bilili 仍会做纠错性维护，只是不会提供新特性了。\n\nyutto 现在也还不是非常稳定，需要稳定的体验的话请继续使用 bilili ～\n\n## Roadmap\n\n### 2.0.0-beta\n\n-  [x] feat: 支持 bare name (bare id, bare path)\n-  [x] refactor: url 列表能够预线性展开\n-  [x] feat: 添加各种 return code\n-  [x] test: 编写单元测试\n\n### 2.0.0\n\n-  [ ] feat: 投稿视频描述文件支持\n-  [ ] docs: 可爱的 logo（呜呜呜，有谁会做 logo 嘛？）\n-  [ ] docs: 可爱的静态文档（可能需要 VitePress 到 1.0）\n\n### future\n\n-  [ ] feat: 字幕、弹幕嵌入视频支持（也许？）\n-  [ ] feat: 封面下载支持（也许？）\n-  [ ] refactor: 以插件形式支持更多音视频处理方面的功能，比如类似 autosub 的工具（也许？）\n-  [ ] feat: 更多批下载支持\n-  [ ] feat: 以及更加可爱～\n\n## 参考\n\n-  基本结构：<https://github.com/SigureMo/bilili>\n-  协程下载：<https://github.com/changmenseng/AsyncBilibiliDownloader>\n-  弹幕转换：<https://github.com/ShigureLab/biliass>\n-  样式设计：<https://github.com/willmcgugan/rich>\n\n## 参与贡献\n\n请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)\n',
+    'long_description': '# yutto<sup>2.0.0-beta</sup>\n\n<p align="center">\n   <a href="https://python.org/" target="_blank"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/yutto?logo=python&style=flat-square"></a>\n   <a href="https://pypi.org/project/yutto/" target="_blank"><img src="https://img.shields.io/pypi/v/yutto?style=flat-square" alt="pypi"></a>\n   <a href="https://pypi.org/project/yutto/" target="_blank"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/yutto?style=flat-square"></a>\n   <a href="LICENSE"><img alt="LICENSE" src="https://img.shields.io/github/license/SigureMo/yutto?style=flat-square"></a>\n   <a href="https://github.com/psf/black"><img alt="black" src="https://img.shields.io/badge/code%20style-black-000000?style=flat-square"></a>\n   <a href="https://gitmoji.dev"><img src="https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67?style=flat-square" alt="Gitmoji"></a>\n</p>\n\nyutto，一个可爱且任性的 B 站下载器（CLI）\n\n## 版本号为什么是 2.0\n\n因为 yutto 是 bilili 的後輩呀～\n\n## 安装预览版\n\n在此之前请确保安装 Python3.9 及以上版本，并配置好 FFmpeg（参照 [bilili 文档](https://bilili.sigure.xyz/guide/getting-started.html)）\n\n当前 yutto 尚处于 beta 阶段，有任何建议尽管在 [Discussions](https://github.com/SigureMo/yutto/discussions) 提出～～～\n\n### pip 安装\n\n```bash\npip install --pre yutto\n```\n\n### git clone\n\n```bash\ngit clone https://github.com/SigureMo/yutto.git\ncd yutto/\npip install poetry\npoetry build\npip install ./dist/yutto-*.whl\n```\n\n## 主要功能\n\n### 已支持的下载类型\n\n<!-- prettier-ignore -->\n|Type|Batch|Example url|Path template|\n|-|-|-|-|\n|投稿视频|:x:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ` <br/> `https://www.bilibili.com/video/av371660125` <br/> `https://www.bilibili.com/video/BV1vZ4y1M7mQ?p=1` <br/> `av371660125` <br/> `BV1vZ4y1M7mQ`|`{title}`|\n|投稿视频|:white_check_mark:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ` <br/> `https://www.bilibili.com/video/av371660125`  <br/> `av371660125` <br/> `BV1vZ4y1M7mQ`|`{title}/{name}`|\n|番剧|:x:|`https://www.bilibili.com/bangumi/play/ep395211` <br/> `ep395211`|`{name}`|\n|番剧|:white_check_mark:|`https://www.bilibili.com/bangumi/play/ep395211` <br/> `https://www.bilibili.com/bangumi/play/ss38221` <br/> `https://www.bilibili.com/bangumi/media/md28233903` <br/> `ep395211` <br/> `ss38221` <br/> `md28233903`|`{title}/{name}`|\n|用户指定收藏夹|:white_check_mark:|`https://space.bilibili.com/100969474/favlist?fid=1306978874`|`{username}的收藏夹/{series_title}/{title}/{name}`|\n|用户全部收藏夹|:white_check_mark:|`https://space.bilibili.com/100969474/favlist`|`{username}的收藏夹/{series_title}/{title}/{name}`|\n|UP 主个人空间|:white_check_mark:|`https://space.bilibili.com/100969474/video`|`{username}的全部投稿视频/{title}/{name}`|\n|视频合集|:white_check_mark:|`https://space.bilibili.com/100969474/channel/seriesdetail?sid=1947439` <br/> `https://www.bilibili.com/medialist/play/100969474?business=space_series&business_id=1947439`|`{series_title}/{title}/{name}`|\n\n### 基本命令\n\nyutto 的基本命令如下：\n\n```bash\nyutto <url>\n```\n\n你可以通过 `yutto -h` 查看详细命令参数。\n\n如果你需要下载**单个**视频，只需要使用 yutto 加上这个视频的地址即可。它支持 av/BV 号以及相应带 p=n 参数的投稿视频页面，也支持 ep 号（episode_id）的番剧页面。\n\n比如只需要这样你就可以下载[《転スラ日記》](https://www.bilibili.com/bangumi/play/ep395211)第一话：\n\n```bash\nyutto https://www.bilibili.com/bangumi/play/ep395211\n```\n\nyutto 还支持直接使用能够唯一定位资源的 id 来作为 `<url>`，刚刚的功能与下面的简化后的命令功能是完全一样的\n\n```bash\nyutto ep395211\n```\n\n不过有时你可能想要批量下载很多剧集，因此 yutto 提供了用于批量下载的参数 `-b/--batch`，它不仅支持前面所说的单个视频所在页面地址（会解析该单个视频所在的系列视频），还支持一些明确用于表示系列视频的地址，比如 md 页面（media_id）、ss 页面（season_id）。\n\n比如像下面这样就可以下载《転スラ日記》所有已更新的剧集：\n\n```bash\nyutto --batch https://www.bilibili.com/bangumi/play/ep395211\n```\n\n### 基础参数\n\n> 大部分参数与 bilili 重合，可参考 [bilili 的 cli 文档](https://bilili.nyakku.moe/cli/)\n\nyutto 支持一些基础参数，无论是批量下载还是单视频下载都适用。\n\n<details>\n<summary>点击展开详细参数</summary>\n\n#### 最大并行 worker 数量\n\n-  参数 `-n` 或 `--num-workers`\n-  默认值 `8`\n\n与 bilili 不同的是，yutto 并不是使用多线程实现并行下载，而是使用协程实现的，本参数限制的是最大的并行 Worker 数量。\n\n#### 指定视频清晰度等级\n\n-  参数 `-q` 或 `--video-quality`\n-  可选值 `127 | 126 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16`\n-  默认值 `127`\n\n清晰度对应关系如下\n\n<!-- prettier-ignore -->\n|code|清晰度|\n|:-:|:-:|\n|127|8K 超高清|\n|126|杜比视界|\n|125|HDR 真彩|\n|120|4K 超清|\n|116|1080P 60帧|\n|112|1080P 高码率|\n|80|1080P 高清|\n|74|720P 60帧|\n|64|720P 高清|\n|32|480P 清晰|\n|16|360P 流畅|\n\n并不是说指定某个清晰度就一定会下载该清晰度的视频，yutto 只会尽可能满足你的要求，如果不存在指定的清晰度，yutto 就会按照默认的清晰度搜索机制进行调节，比如指定清晰度为 `80`，**首先会依次降清晰度搜索** `74`、`64`、`32`、`16`，如果依然找不到合适的则**继续升清晰度搜索** `112`、`116`、`120`、`125`、`126`、`127`。\n\n值得注意的是，目前杜比视界视频只能简单下载音视频流并合并，合并后并不能达到在线观看的效果。\n\n#### 指定音频码率等级\n\n-  参数 `-aq` 或 `--audio-quality`\n-  可选值 `30280 | 30232 | 30216`\n-  默认值 `30280`\n\n码率对应关系如下\n\n<!-- prettier-ignore -->\n|code|码率|\n|:-:|:-:|\n|30280|320kbps|\n|30232|128kbps|\n|30216|64kbps|\n\n码率自动调节机制与视频清晰度一致，也采用先降后升的匹配机制。\n\n#### 指定视频编码\n\n-  参数 `--vcodec`\n-  下载编码可选值 `"av1" | "hevc" | "avc"`\n-  保存编码可选值 FFmpeg 所有可用的视频编码器\n-  默认值 `"avc:copy"`\n\n该参数略微复杂，前半部分表示在下载时**优先**选择哪一种编码的视频流，后半部分则表示在合并时如何编码视频流，两者使用 `:` 分隔。\n\n值得注意的是，前半的下载编码只是优先下载的编码而已，如果不存在该编码，则仍会像视频清晰度调节机制一样自动选择其余编码。\n\n而后半部分的参数如果设置成非 `copy` 的值则可以确保在下载完成后对其进行重新编码，而且不止支持 `av1`、`hevc` 与 `avc`，只要你的 FFmpeg 支持的视频编码器，它都可以完成。\n\n#### 指定音频编码\n\n-  参数 `--acodec`\n-  下载编码可选值 `"mp4a"`\n-  保存编码可选值 FFmpeg 所有可用的音频编码器\n-  默认值 `"mp4a:copy"`\n\n详情同视频编码。\n\n#### 仅下载视频流\n\n-  参数 `--video-only`\n-  默认值 `False`\n\n#### 仅下载音频流\n\n-  参数 `--audio-only`\n-  默认值 `False`\n\n仅下载其中的音频流，保存为 `.aac` 文件。\n\n值得注意的是，在不选择视频流时，嵌入字幕、弹幕功能将无法工作。\n\n#### 弹幕格式选择\n\n-  参数 `-df` 或 `--danmaku-format`\n-  可选值 `"ass" | "xml" | "protobuf"`\n-  默认值 `"ass"`\n\nB 站提供了 `xml` 与 `protobuf` 两种弹幕数据接口，yutto 会自动下载 `xml` 格式弹幕并转换为 `ass` 格式，如果你不喜欢 yutto 自动转换的效果，可以选择输出格式为 `xml` 或 `protobuf`，手动通过一些工具进行转换，比如 yutto 和 bilili 所使用的 [biliass](https://github.com/ShigureLab/biliass)，或者使用 [us-danmaku](https://tiansh.github.io/us-danmaku/bilibili/) 进行在线转换。\n\n如果你不想下载弹幕，只需要使用参数 `--no-danmaku` 即可。\n\n#### 下载块大小\n\n-  参数 `-bs` 或 `--block-size`\n-  默认值 `0.5`\n\n以 MiB 为单位，为分块下载时各块大小，不建议更改。\n\n#### 强制覆盖已下载文件\n\n-  参数 `-w` 或 `--overwrite`\n-  默认值 `False`\n\n#### 代理设置\n\n-  参数 `-x` 或 `--proxy`\n-  可选值 `"auto" | "no" | <https?://url/to/proxy/server>`\n-  默认值 `"auto"`\n\n设置代理服务器，默认是从环境变量读取，`no` 则为不设置代理，设置其它 http/https url 则将其作为代理服务器。\n\n#### 存放根目录\n\n-  参数 `-d` 或 `--dir`\n-  默认值 `"./"`\n\n#### 临时文件目录\n\n-  参数 `--tmp-dir`\n-  默认值是“存放根目录”即 `-d, --dir` 的值\n\n#### 存放子路径模板\n\n-  参数 `-tp` 或 `--subpath-template`\n-  可选参数变量 `title | id | name | username | series_title | pubdate` （以后可能会有更多）\n-  默认值 `"{auto}"`\n\n通过配置子路径模板可以灵活地控制视频存放位置。\n\n默认情况是由 yutto 自动控制存放位置的。比如下载单个视频时默认就是直接存放在设定的根目录，不会创建一层容器目录，此时自动选择了 `{name}` 作为模板；而批量下载时则会根据视频层级生成多级目录，比如番剧会是 `{title}/{name}`，首先会在设定根目录里生成一个番剧名的目录，其内才会存放各个番剧剧集视频，这样方便了多个不同番剧的管理。当然，如果你仍希望将番剧直接存放在设定根目录下的话，可以修改该参数值为 `{name}`即可。\n\n另外，该功能语法由 Python format 函数模板语法提供，所以也支持一些高级的用法，比如 `{id:0>3}{name}`。\n\n值得注意的是，并不是所有变量在各种场合下都会提供，比如 `username` 变量当前仅在 UP 主全部投稿视频/收藏夹才提供，在其它情况下不应使用它。各变量详细作用域描述见下表：\n\n<!-- prettier-ignore -->\n|Variable|Description|Scope|\n|-|-|-|\n|title|系列视频总标题（番剧名/投稿视频标题）|全部|\n|id|系列视频单 p 顺序标号|全部|\n|name|系列视频单 p 标题|全部|\n|username|UP 主用户名|个人空间、收藏夹、合集下载|\n|series_title|合集标题|收藏夹、视频合集下载|\n|pubdate|投稿日期|仅投稿视频|\n\n> 未来可能会对路径变量及默认路径模板进行调整\n\n#### url 别名文件路径\n\n-  参数 `-af` 或 `--alias-file`\n-  默认值 `None`\n\n指定别名文件路径，别名文件中存放一个别名与其对应的 url，使用空格或者 `=` 分隔，示例如下：\n\n```\nrimuru1=https://www.bilibili.com/bangumi/play/ss25739/\nrimuru2=https://www.bilibili.com/bangumi/play/ss36170/\nrimuru-nikki=https://www.bilibili.com/bangumi/play/ss38221/\n```\n\n比如将上述内容存储到 `~/.yutto_alias`，则通过以下命令即可解析该文件：\n\n```bash\nyutto rimuru1 --batch --alias-file=\'~/.yutto_alias\'\n```\n\n当参数值为 `-` 时，会从标准输入中读取：\n\n```bash\ncat ~/.yutto_alias | yutto rimuru-nikki --batch --alias-file -\n```\n\n#### Cookies 设置\n\n-  参数 `-c` 或 `--sessdata`\n-  默认值 `""`\n\n设置 Cookies 后你才可以下载更高清晰度以及更多的剧集，当你传入你的大会员 `SESSDATA` 时（当然前提是你是大会员），你就可以下载大会员可访问的资源咯。\n\n<details><summary> SESSDATA 获取方式 </summary>\n\n这里用 Chrome 作为示例，其它浏览器请尝试类似方法。\n\n首先，用你的帐号登录 B 站，然后随便打开一个 B 站网页，比如[首页](https://www.bilibili.com/)。\n\n按 F12 打开开发者工具，切换到 Network 栏，刷新页面，此时第一个加载的资源应该就是当前页面的 html，选中该资源，在右侧 「Request Headers」 中找到 「cookie」，在其中找到类似于 `SESSDATA=d8bc7493%2C2843925707%2C08c3e*81;` 的一串字符串，复制这里的 `d8bc7493%2C2843925707%2C08c3e*81`，这就是你需要的 `SESSDATA`。\n\n</details>\n\n另外，由于 SESSDATA 中可能有特殊符号，所以传入时你可能需要使用双引号来包裹\n\n```bash\nyutto <url> -c "d8bc7493%2C2843925707%2C08c3e*81"\n```\n\n当然，示例里的 SESSDATA 是无效的，请使用自己的 SESSDATA。\n\n#### 不下载弹幕\n\n-  参数 `--no-danmaku`\n-  默认值 `False`\n\n#### 不下载字幕\n\n-  参数 `--no-subtitle`\n-  默认值 `False`\n\n#### 不显示颜色\n\n-  参数 `--no-color`\n-  默认值 `False`\n\n#### 启用 Debug 模式\n\n-  参数 `--debug`\n-  默认值 `False`\n\n#### 生成媒体元数据文件\n\n-  参数 `--with-metadata`\n-  默认值 `False`\n\n</details>\n\n### 批量参数\n\n有些参数是只有批量下载时才可以使用的\n\n<details>\n<summary>点击展开详细参数</summary>\n\n#### 启用批量下载\n\n-  参数 `-b` 或 `--batch`\n-  默认值 `False`\n\n只需要 `yutto --batch <url>` 即可启用批量下载功能。\n\n#### 选集\n\n-  参数 `-p` 或 `--episodes`\n-  默认值 `^~$`\n\n-  参数 `-p` 或 `--episodes`\n-  默认值 `^~$`（也即全选）\n\n也就是选集咯，其语法是这样的\n\n-  `<p1>` 单独下某一剧集\n   -  支持负数来选择倒数第几话\n   -  此外还可以使用 `^` 与 `$` 来分别代表 `1` 与 `-1`\n-  `<p_start>~<p_end>` 使用 `~` 可以连续选取\n-  `<p1>,<p2>,<p3>,...,<pn>` 使用 `,` 可以不连续选取\n\nemmm，直接看的话大概并不能知道我在说什么，所以我们通过几个小例子来了解其语法\n\n```bash\n# 假设要下载一个具有 24 话的番剧\n# 如果我们只想下载第 3 话，只需要这样\nyutto <url> -b -p 3\n# 那如果我想下载第 5 话到第 7 话呢，使用 `~` 可以连续选中\nyutto <url> -b -p 5~7\n# 那我想下载第 12 话和第 17 话又要怎么办？此时只需要 `,` 就可以将多个不连续的选集一起选中\nyutto <url> -b -p 12,17\n# 那我突然又想将刚才那些都选中了呢？还是使用 `,` 呀，将它们连在一起即可\nyutto <url> -b -p 3,5~7,12,17\n# 嗯，你已经把基本用法都了解过了，很简单吧～\n# 下面是一些语法糖，不了解也完全不会影响任何功能哒～\n# 那如果我只知道我想下载倒数第 3 话，而不想算倒数第三话是第几话应该怎么办？\n# 此时可以用负数哒～不过要注意的是，开头如果是 `-` 的话前面应该使用 `=`\nyutto <url> -b -p=-3\n# 那么如果想下载最后一话你可能会想到 `-p=-1` 对吧？不过我内置了两个符号分别代表第一话（^）和最后一话（$）\n# 像下面这样就可以直接下载最后一话啦～\nyutto <url> -b -p $\n# 所有语法都了解完啦，我们看一个稍微复杂的例子\nyutto <url> -b -p ^~3,10,12~14,16,-4~$\n# 很明显，上面的例子就是下载前 3 话、第 10 话、第 12 到 14 话、第 16 话以及后 4 话\n```\n\n下面是一些要注意的问题\n\n1. 这里使用的序号是视频的顺序序号，而不是番剧所标注的`第 n 话`，因为有可能会出现 `第 x.5 话` 等等的特殊情况，此时一定要按照顺序自行计数。\n2. 参数值里一定不要加空格\n3. 参数值开头为 `-` 时前面应该使用 `=` 而非空格\n4. 个人空间、合集、收藏夹等批量下载暂不支持选集操作\n\n#### 同时下载附加剧集\n\n-  参数 `-s` 或 `--with-section`\n-  默认值 `False`\n\n</details>\n\n## 从 bilili1.x 迁移\n\n### 取消的功能\n\n-  `- bilibili` 目录的生成\n-  播放列表生成\n-  源格式修改功能（不再支持 flv 源视频下载，如果仍有视频不支持 dash 源，请继续使用 bilili）\n-  对 Python3.8 的支持，最低支持 Python3.9\n-  下载前询问\n\n### 默认行为的修改\n\n-  使用协程而非多线程进行下载，同时也不是批量解析批量下载，而是边解析边下载\n-  默认生成弹幕为 ASS\n-  默认启用从多镜像源下载的特性\n-  不仅可以控制是否使用系统代理，还能配置特定的代理服务器\n\n### 新增的特性\n\n-  单视频下载与批量下载命令分离（`bilili` 命令与 `yutto --batch` 相类似）\n-  音频/视频编码选择\n-  仅下载音频/视频\n-  存放子路径的自由定制\n-  支持 url 别名\n-  支持文件列表\n-  更多的批下载支持（现已支持 UP 主全部视频下载，扩展其它批下载支持也很简单）\n-  更加完善的 warning 与 error 提示\n-  支持仅输入 id 即可下载（aid、bvid、episode_id 等）\n-  支持描述文件生成（当前仅番剧）\n\n## 小技巧\n\n### 使用 uvloop 提升协程效率\n\n听说 uvloop 可以提高协程效率，如果你的系统非 Windows 的话，可以试一下安装 uvloop：\n\n```bash\npip install uvloop\n```\n\n现在再运行就会发现不会弹出「没有安装 uvloop 的」 warning 了，至于具体提升多少我也不太清楚啦，没有测过\n\n### 使用 url alias\n\nyutto 新增的 url alias 可以让你下载正在追的番剧时不必每次都打开浏览器复制 url，只需要将追番列表存储在一个文件中，并为这些 url 起一个别名即可\n\n```\nrimuru-nikki=https://www.bilibili.com/bangumi/play/ss38221/\n```\n\n之后下载最新话只需要\n\n```\nyutto --batch rimuru-nikki --alias-file=/path/to/alias-file\n```\n\n### 使用文件列表\n\n现在 url 不仅支持 http/https 链接与裸 id，还支持使用文件路径与 file scheme 来用于表示文件列表，文件列表以行分隔，每行写一次命令的参数，该参数会覆盖掉主程序中所使用的参数，示例如下：\n\n首先将下面的文件存储到一个地方\n\n```\nhttps://www.bilibili.com/bangumi/play/ss38221/ --batch -p $\nhttps://www.bilibili.com/bangumi/play/ss38260/ --batch -p $\n```\n\n然后运行\n\n```\nyutto file:///path/to/list\n```\n\n即可分别下载这两个番剧的最新一话\n\n或者直接使用相对或者绝对路径也是可以的\n\n```\nyutto ./path/to/list\n```\n\n值得注意的是，在文件列表各项里的参数优先级是高于命令里的优先级的，比如文件中使用：\n\n```\nrimuru1 --batch -p $ --no-danmaku --vcodec="hevc:copy"\nrimuru2 --batch -p $\n```\n\n而命令中则使用\n\n```\nyutto file:///path/to/list --vcodec="avc:copy"\n```\n\n最终下载的 rimuru1 会是 "hevc:copy"，而 rimuru2 则会是 "avc:copy"\n\n另外，文件列表也是支持 alias 的，你完全可以为该列表起一个别名，一个比较特别的用例是将你所有追番的内容放在一个文件里，然后为该文件起一个别名（比如 `subscription`），这样只需要 `yutto subscription --alias-file path/to/alias/file` 就可以达到追番效果啦～\n\n最后，列表也是支持嵌套的哦（虽然没什么用 2333）\n\n## FAQ\n\n### 名字的由来\n\n[《転スラ日記》第一话 00:24](https://www.bilibili.com/bangumi/play/ep395211?t=24)\n\n### yutto 会很快替代 bilili 吗\n\n短期内不会，bilili 并不会消失，在一段时间内 bilili 仍会做纠错性维护，只是不会提供新特性了。\n\nyutto 现在也还不是非常稳定，需要稳定的体验的话请继续使用 bilili ～\n\n## Roadmap\n\n### 2.0.0-beta\n\n-  [x] feat: 支持 bare name (bare id, bare path)\n-  [x] refactor: url 列表能够预线性展开\n-  [x] feat: 添加各种 return code\n-  [x] test: 编写单元测试\n\n### 2.0.0\n\n-  [ ] feat: 投稿视频描述文件支持\n-  [ ] refactor: 整理路径变量名\n-  [ ] docs: 可爱的 logo（呜呜呜，有谁会做 logo 嘛？）\n-  [ ] docs: 可爱的静态文档（可能需要 VitePress 到 1.0）\n\n### future\n\n-  [ ] feat: 字幕、弹幕嵌入视频支持（也许？）\n-  [ ] feat: 封面下载支持（也许？）\n-  [ ] refactor: 以插件形式支持更多音视频处理方面的功能，比如类似 autosub 的工具（也许？）\n-  [ ] feat: 更多批下载支持\n-  [ ] feat: 以及更加可爱～\n\n## 参考\n\n-  基本结构：<https://github.com/SigureMo/bilili>\n-  协程下载：<https://github.com/changmenseng/AsyncBilibiliDownloader>\n-  弹幕转换：<https://github.com/ShigureLab/biliass>\n-  样式设计：<https://github.com/willmcgugan/rich>\n\n## 参与贡献\n\n请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)\n',
     'author': 'Nyakku Shigure',
     'author_email': 'sigure.qaq@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/SigureMo/yutto',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,37 +1,58 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['yutto',
 'yutto.api', 'yutto.cli', 'yutto.media', 'yutto.processor', 'yutto.utils',
 'yutto.utils.console', 'yutto.utils.functiontools'] package_data = \ {'':
 ['*']} install_requires = \ ['aiofiles>=0.7,<0.9', 'aiohttp>=3.7.4,<4.0.0',
 'biliass==1.3.4', 'dicttoxml>=1.7.4,<2.0.0'] extras_require = \ {'uvloop':
 ['uvloop==0.16.0']} entry_points = \ {'console_scripts': ['yutto =
-yutto.__main__:main']} setup_kwargs = { 'name': 'yutto', 'version': '2.0.0b8',
+yutto.__main__:main']} setup_kwargs = { 'name': 'yutto', 'version': '2.0.0b9',
 'description': 'ð§ ä¸ä¸ªå¯ç±ä¸ä»»æ§ç B ç«è§é¢ä¸è½½å¨',
 'long_description': '# yutto2.0.0-beta\n\n
     \n _[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]\n _[_p_y_p_i_]\n _[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]\n _[_L_I_C_E_N_S_E_]\n
                              _[_b_l_a_c_k_]\n _[_G_i_t_m_o_j_i_]\n
 \n\nyuttoï¼ä¸ä¸ªå¯ç±ä¸ä»»æ§ç B ç«ä¸è½½å¨ï¼CLIï¼\n\n##
 çæ¬å·ä¸ºä»ä¹æ¯ 2.0\n\nå ä¸º yutto æ¯ bilili çå¾è¼©åï½\n\n##
 å®è£é¢è§ç\n\nå¨æ­¤ä¹åè¯·ç¡®ä¿å®è£ Python3.9
 åä»¥ä¸çæ¬ï¼å¹¶éç½®å¥½ FFmpegï¼åç§ [bilili ææ¡£](https://
 bilili.sigure.xyz/guide/getting-started.html)ï¼\n\nå½å yutto å°å¤äº beta
 é¶æ®µï¼æä»»ä½å»ºè®®å°½ç®¡å¨ [Discussions](https://github.com/SigureMo/
 yutto/discussions) æåºï½ï½ï½\n\n### pip å®è£\n\n```bash\npip install --
 pre yutto\n```\n\n### git clone\n\n```bash\ngit clone https://github.com/
 SigureMo/yutto.git\ncd yutto/\npip install poetry\npoetry build\npip install ./
 dist/yutto-*.whl\n```\n\n## ä¸»è¦åè½\n\n###
-å·²æ¯æçä¸è½½ç±»å\n\n\n|type|batch|path template|\n|-|-|-
-|\n|æç¨¿è§é¢|:x:|`{title}`|\n|æç¨¿è§é¢|:white_check_mark:|`{title}/
-{name}`|\n|çªå§|:x:|`{name}`|\n|çªå§|:white_check_mark:|`{title}/
-{name}`|\n|ç¨æ·æå®æ¶èå¤¹|:white_check_mark:|`{username}çæ¶èå¤¹/
-{fav_title}/{title}/{name}`|\n|ç¨æ·å¨é¨æ¶èå¤¹|:white_check_mark:|`
-{username}çæ¶èå¤¹/{fav_title}/{title}/{name}`|\n|UP ä¸»ä¸ªäººç©ºé´|:
-white_check_mark:|`{username}çå¨é¨æç¨¿è§é¢/{title}/{name}`|\n\n\n\n###
-åºæ¬å½ä»¤\n\nyutto çåºæ¬å½ä»¤å¦ä¸ï¼\n\n```bash\nyutto
-\n```\n\nä½ å¯ä»¥éè¿ `yutto -h`
+å·²æ¯æçä¸è½½ç±»å\n\n\n|Type|Batch|Example url|Path template|\n|-|-|-|-
+|\n|æç¨¿è§é¢|:x:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ`
+`https://www.bilibili.com/video/av371660125`
+`https://www.bilibili.com/video/BV1vZ4y1M7mQ?p=1`
+`av371660125`
+`BV1vZ4y1M7mQ`|`{title}`|\n|æç¨¿è§é¢|:white_check_mark:|`https://
+www.bilibili.com/video/BV1vZ4y1M7mQ`
+`https://www.bilibili.com/video/av371660125`
+`av371660125`
+`BV1vZ4y1M7mQ`|`{title}/{name}`|\n|çªå§|:x:|`https://www.bilibili.com/
+bangumi/play/ep395211`
+`ep395211`|`{name}`|\n|çªå§|:white_check_mark:|`https://www.bilibili.com/
+bangumi/play/ep395211`
+`https://www.bilibili.com/bangumi/play/ss38221`
+`https://www.bilibili.com/bangumi/media/md28233903`
+`ep395211`
+`ss38221`
+`md28233903`|`{title}/{name}`|\n|ç¨æ·æå®æ¶èå¤¹|:white_check_mark:
+|`https://space.bilibili.com/100969474/favlist?fid=1306978874`|`
+{username}çæ¶èå¤¹/{series_title}/{title}/
+{name}`|\n|ç¨æ·å¨é¨æ¶èå¤¹|:white_check_mark:|`https://
+space.bilibili.com/100969474/favlist`|`{username}çæ¶èå¤¹/{series_title}/
+{title}/{name}`|\n|UP ä¸»ä¸ªäººç©ºé´|:white_check_mark:|`https://
+space.bilibili.com/100969474/video`|`{username}çå¨é¨æç¨¿è§é¢/{title}/
+{name}`|\n|è§é¢åé|:white_check_mark:|`https://space.bilibili.com/
+100969474/channel/seriesdetail?sid=1947439`
+`https://www.bilibili.com/medialist/play/
+100969474?business=space_series&business_id=1947439`|`{series_title}/{title}/
+{name}`|\n\n### åºæ¬å½ä»¤\n\nyutto
+çåºæ¬å½ä»¤å¦ä¸ï¼\n\n```bash\nyutto \n```\n\nä½ å¯ä»¥éè¿ `yutto -h`
 æ¥çè¯¦ç»å½ä»¤åæ°ã\n\nå¦æä½ éè¦ä¸è½½**åä¸ª**è§é¢ï¼åªéè¦ä½¿ç¨
 yutto å ä¸è¿ä¸ªè§é¢çå°åå³å¯ãå®æ¯æ av/BV å·ä»¥åç¸åºå¸¦
 p=n åæ°çæç¨¿è§é¢é¡µé¢ï¼ä¹æ¯æ ep
 å·ï¼episode_idï¼ççªå§é¡µé¢ã\n\næ¯å¦åªéè¦è¿æ ·ä½ å°±å¯ä»¥ä¸è½½
 [ãè»¢ã¹ã©æ¥è¨ã](https://www.bilibili.com/bangumi/play/
 ep395211)ç¬¬ä¸è¯ï¼\n\n```bash\nyutto https://www.bilibili.com/bangumi/play/
 ep395211\n```\n\nyutto è¿æ¯æç´æ¥ä½¿ç¨è½å¤å¯ä¸å®ä½èµæºç id
@@ -46,38 +67,40 @@
 åºç¡åæ°\n\n> å¤§é¨ååæ°ä¸ bilili éåï¼å¯åè [bilili ç cli
 ææ¡£](https://bilili.nyakku.moe/cli/)\n\nyutto
 æ¯æä¸äºåºç¡åæ°ï¼æ è®ºæ¯æ¹éä¸è½½è¿æ¯åè§é¢ä¸è½½é½éç¨ã\n\n\nç¹å»å±å¼è¯¦ç»åæ°\n\n####
 æå¤§å¹¶è¡ worker æ°é\n\n- åæ° `-n` æ `--num-workers`\n- é»è®¤å¼
 `8`\n\nä¸ bilili ä¸åçæ¯ï¼yutto
 å¹¶ä¸æ¯ä½¿ç¨å¤çº¿ç¨å®ç°å¹¶è¡ä¸è½½ï¼èæ¯ä½¿ç¨åç¨å®ç°çï¼æ¬åæ°éå¶çæ¯æå¤§çå¹¶è¡
 Worker æ°éã\n\n#### æå®è§é¢æ¸æ°åº¦ç­çº§\n\n- åæ° `-q` æ `--
-video-quality`\n- å¯éå¼ `127 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 |
-16`\n- é»è®¤å¼ `127`\n\næ¸æ°åº¦å¯¹åºå³ç³»å¦ä¸\n\n\n|code|æ¸æ°åº¦|\n|:
--:|:-:|\n|127|8K è¶é«æ¸|\n|125|HDR çå½©|\n|120|4K è¶æ¸|\n|116|1080P
+video-quality`\n- å¯éå¼ `127 | 126 | 125 | 120 | 116 | 112 | 80 | 74 | 64 |
+32 | 16`\n- é»è®¤å¼
+`127`\n\næ¸æ°åº¦å¯¹åºå³ç³»å¦ä¸\n\n\n|code|æ¸æ°åº¦|\n|:-:|:-:|\n|127|8K
+è¶é«æ¸|\n|126|ææ¯è§ç|\n|125|HDR çå½©|\n|120|4K è¶æ¸|\n|116|1080P
 60å¸§|\n|112|1080P é«ç ç|\n|80|1080P é«æ¸|\n|74|720P 60å¸§|\n|64|720P
 é«æ¸|\n|32|480P æ¸æ°|\n|16|360P
 æµç|\n\nå¹¶ä¸æ¯è¯´æå®æä¸ªæ¸æ°åº¦å°±ä¸å®ä¼ä¸è½½è¯¥æ¸æ°åº¦çè§é¢ï¼yutto
 åªä¼å°½å¯è½æ»¡è¶³ä½ çè¦æ±ï¼å¦æä¸å­å¨æå®çæ¸æ°åº¦ï¼yutto
 å°±ä¼æç§é»è®¤çæ¸æ°åº¦æç´¢æºå¶è¿è¡è°èï¼æ¯å¦æå®æ¸æ°åº¦ä¸º
 `80`ï¼**é¦åä¼ä¾æ¬¡éæ¸æ°åº¦æç´¢**
 `74`ã`64`ã`32`ã`16`ï¼å¦æä¾ç¶æ¾ä¸å°åéçå**ç»§ç»­åæ¸æ°åº¦æç´¢**
-`112`ã`116`ã`120`ã`125`ã`127`ã\n\n#### æå®é³é¢ç çç­çº§\n\n-
-åæ° `-aq` æ `--audio-quality`\n- å¯éå¼ `30280 | 30232 | 30216`\n-
-é»è®¤å¼ `30280`\n\nç çå¯¹åºå³ç³»å¦ä¸\n\n\n|code|ç ç|\n|:-:|:-:
-|\n|30280|320kbps|\n|30232|128kbps|\n|30216|64kbps|\n\næ¸æ°åº¦èªå¨è°èæºå¶ä¸è§é¢æ¸æ°åº¦ä¸è´ï¼ä¹éç¨åéååçå¹éæºå¶ã\n\n####
-æå®è§é¢ç¼ç \n\n- åæ° `--vcodec`\n- ä¸è½½ç¼ç å¯éå¼ `"hevc" |
-"avc"`\n- ä¿å­ç¼ç å¯éå¼ FFmpeg ææå¯ç¨çè§é¢ç¼ç å¨\n-
-é»è®¤å¼ `"avc:
+`112`ã`116`ã`120`ã`125`ã`126`ã`127`ã\n\nå¼å¾æ³¨æçæ¯ï¼ç®åææ¯è§çè§é¢åªè½ç®åä¸è½½é³è§é¢æµå¹¶åå¹¶ï¼åå¹¶åå¹¶ä¸è½è¾¾å°å¨çº¿è§ççææã\n\n####
+æå®é³é¢ç çç­çº§\n\n- åæ° `-aq` æ `--audio-quality`\n- å¯éå¼
+`30280 | 30232 | 30216`\n- é»è®¤å¼
+`30280`\n\nç çå¯¹åºå³ç³»å¦ä¸\n\n\n|code|ç ç|\n|:-:|:-:
+|\n|30280|320kbps|\n|30232|128kbps|\n|30216|64kbps|\n\nç çèªå¨è°èæºå¶ä¸è§é¢æ¸æ°åº¦ä¸è´ï¼ä¹éç¨åéååçå¹éæºå¶ã\n\n####
+æå®è§é¢ç¼ç \n\n- åæ° `--vcodec`\n- ä¸è½½ç¼ç å¯éå¼ `"av1" |
+"hevc" | "avc"`\n- ä¿å­ç¼ç å¯éå¼ FFmpeg
+ææå¯ç¨çè§é¢ç¼ç å¨\n- é»è®¤å¼ `"avc:
 copy"`\n\nè¯¥åæ°ç¥å¾®å¤æï¼ååé¨åè¡¨ç¤ºå¨ä¸è½½æ¶**ä¼å**éæ©åªä¸ç§ç¼ç çè§é¢æµï¼ååé¨ååè¡¨ç¤ºå¨åå¹¶æ¶å¦ä½ç¼ç è§é¢æµï¼ä¸¤èä½¿ç¨
 `:
 `
 åéã\n\nå¼å¾æ³¨æçæ¯ï¼ååçä¸è½½ç¼ç åªæ¯ä¼åä¸è½½çç¼ç èå·²ï¼å¦æä¸å­å¨è¯¥ç¼ç ï¼åä»ä¼åè§é¢æ¸æ°åº¦è°èæºå¶ä¸æ ·èªå¨éæ©å¶ä½ç¼ç ã\n\nèååé¨åçåæ°å¦æè®¾ç½®æé
 `copy`
 çå¼åå¯ä»¥ç¡®ä¿å¨ä¸è½½å®æåå¯¹å¶è¿è¡éæ°ç¼ç ï¼èä¸ä¸æ­¢æ¯æ
-`hevc` ä¸ `avc`ï¼åªè¦ä½ ç FFmpeg
+`av1`ã`hevc` ä¸ `avc`ï¼åªè¦ä½ ç FFmpeg
 æ¯æçè§é¢ç¼ç å¨ï¼å®é½å¯ä»¥å®æã\n\n####
 æå®é³é¢ç¼ç \n\n- åæ° `--acodec`\n- ä¸è½½ç¼ç å¯éå¼ `"mp4a"`\n-
 ä¿å­ç¼ç å¯éå¼ FFmpeg ææå¯ç¨çé³é¢ç¼ç å¨\n- é»è®¤å¼
 `"mp4a:copy"`\n\nè¯¦æåè§é¢ç¼ç ã\n\n#### ä»ä¸è½½è§é¢æµ\n\n-
 åæ° `--video-only`\n- é»è®¤å¼ `False`\n\n#### ä»ä¸è½½é³é¢æµ\n\n-
 åæ° `--audio-only`\n- é»è®¤å¼
 `False`\n\nä»ä¸è½½å¶ä¸­çé³é¢æµï¼ä¿å­ä¸º `.aac`
@@ -100,15 +123,15 @@
 ://url/to/proxy/server>`\n- é»è®¤å¼
 `"auto"`\n\nè®¾ç½®ä»£çæå¡å¨ï¼é»è®¤æ¯ä»ç¯å¢åéè¯»åï¼`no`
 åä¸ºä¸è®¾ç½®ä»£çï¼è®¾ç½®å¶å® http/https url
 åå°å¶ä½ä¸ºä»£çæå¡å¨ã\n\n#### å­æ¾æ ¹ç®å½\n\n- åæ° `-d` æ
 `--dir`\n- é»è®¤å¼ `"./"`\n\n#### ä¸´æ¶æä»¶ç®å½\n\n- åæ° `--tmp-
 dir`\n- é»è®¤å¼æ¯âå­æ¾æ ¹ç®å½âå³ `-d, --dir` çå¼\n\n####
 å­æ¾å­è·¯å¾æ¨¡æ¿\n\n- åæ° `-tp` æ `--subpath-template`\n-
-å¯éåæ°åé `title | id | name | username | fav_title | pubdate`
+å¯éåæ°åé `title | id | name | username | series_title | pubdate`
 ï¼ä»¥åå¯è½ä¼ææ´å¤ï¼\n- é»è®¤å¼ `"
 {auto}"`\n\néè¿éç½®å­è·¯å¾æ¨¡æ¿å¯ä»¥çµæ´»å°æ§å¶è§é¢å­æ¾ä½ç½®ã\n\né»è®¤æåµæ¯ç±
 yutto
 èªå¨æ§å¶å­æ¾ä½ç½®çãæ¯å¦ä¸è½½åä¸ªè§é¢æ¶é»è®¤å°±æ¯ç´æ¥å­æ¾å¨è®¾å®çæ ¹ç®å½ï¼ä¸ä¼åå»ºä¸å±å®¹å¨ç®å½ï¼æ­¤æ¶èªå¨éæ©äº
 `{name}`
 ä½ä¸ºæ¨¡æ¿ï¼èæ¹éä¸è½½æ¶åä¼æ ¹æ®è§é¢å±çº§çæå¤çº§ç®å½ï¼æ¯å¦çªå§ä¼æ¯
 `{title}/
@@ -118,16 +141,17 @@
 0>3}
 {name}`ã\n\nå¼å¾æ³¨æçæ¯ï¼å¹¶ä¸æ¯ææåéå¨åç§åºåä¸é½ä¼æä¾ï¼æ¯å¦
 `username` åéå½åä»å¨ UP ä¸»å¨é¨æç¨¿è§é¢/
 æ¶èå¤¹ææä¾ï¼å¨å¶å®æåµä¸ä¸åºä½¿ç¨å®ãååéè¯¦ç»ä½ç¨åæè¿°è§ä¸è¡¨ï¼\n\n\n|Variable|Description|Scope|\n|-
 |-|-|\n|title|ç³»åè§é¢æ»æ é¢ï¼çªå§å/
 æç¨¿è§é¢æ é¢ï¼|å¨é¨|\n|id|ç³»åè§é¢å p
 é¡ºåºæ å·|å¨é¨|\n|name|ç³»åè§é¢å p æ é¢|å¨é¨|\n|username|UP
-ä¸»ç¨æ·å|ä¸ªäººç©ºé´ãæ¶èå¤¹ä¸è½½|\n|pubdate|æç¨¿æ¥æ|ä»æç¨¿è§é¢|\n\n####
-url å«åæä»¶è·¯å¾\n\n- åæ° `-af` æ `--alias-file`\n- é»è®¤å¼
+ä¸»ç¨æ·å|ä¸ªäººç©ºé´ãæ¶èå¤¹ãåéä¸è½½|\n|series_title|åéæ é¢|æ¶èå¤¹ãè§é¢åéä¸è½½|\n|pubdate|æç¨¿æ¥æ|ä»æç¨¿è§é¢|\n\n>
+æªæ¥å¯è½ä¼å¯¹è·¯å¾åéåé»è®¤è·¯å¾æ¨¡æ¿è¿è¡è°æ´\n\n#### url
+å«åæä»¶è·¯å¾\n\n- åæ° `-af` æ `--alias-file`\n- é»è®¤å¼
 `None`\n\næå®å«åæä»¶è·¯å¾ï¼å«åæä»¶ä¸­å­æ¾ä¸ä¸ªå«åä¸å¶å¯¹åºç
 urlï¼ä½¿ç¨ç©ºæ ¼æè `=` åéï¼ç¤ºä¾å¦ä¸ï¼\n\n```\nrimuru1=https://
 www.bilibili.com/bangumi/play/ss25739/\nrimuru2=https://www.bilibili.com/
 bangumi/play/ss36170/\nrimuru-nikki=https://www.bilibili.com/bangumi/play/
 ss38221/\n```\n\næ¯å¦å°ä¸è¿°åå®¹å­å¨å°
 `~/.yutto_alias`ï¼åéè¿ä»¥ä¸å½ä»¤å³å¯è§£æè¯¥æä»¶ï¼\n\n```bash\nyutto
 rimuru1 --batch --alias-file=\'~/.yutto_alias\'\n```\n\nå½åæ°å¼ä¸º `-
@@ -186,28 +210,29 @@
 p ^~3,10,12~14,16,-4~$\n# å¾ææ¾ï¼ä¸é¢çä¾å­å°±æ¯ä¸è½½å 3
 è¯ãç¬¬ 10 è¯ãç¬¬ 12 å° 14 è¯ãç¬¬ 16 è¯ä»¥åå 4
 è¯\n```\n\nä¸é¢æ¯ä¸äºè¦æ³¨æçé®é¢\n\n1.
 è¿éä½¿ç¨çåºå·æ¯è§é¢çé¡ºåºåºå·ï¼èä¸æ¯çªå§ææ æ³¨ç`ç¬¬
 n è¯`ï¼å ä¸ºæå¯è½ä¼åºç° `ç¬¬ x.5 è¯`
 ç­ç­çç¹æ®æåµï¼æ­¤æ¶ä¸å®è¦æç§é¡ºåºèªè¡è®¡æ°ã\n2.
 åæ°å¼éä¸å®ä¸è¦å ç©ºæ ¼\n3. åæ°å¼å¼å¤´ä¸º `-
-` æ¶åé¢åºè¯¥ä½¿ç¨ `=` èéç©ºæ ¼\n\n#### åæ¶ä¸è½½éå å§é\n\n-
-åæ° `-s` æ `--with-section`\n- é»è®¤å¼ `False`\n\n\n\n## ä» bilili1.x
-è¿ç§»\n\n### åæ¶çåè½\n\n- `- bilibili` ç®å½ççæ\n-
-æ­æ¾åè¡¨çæ\n- æºæ ¼å¼ä¿®æ¹åè½ï¼ä¸åæ¯æ flv
-æºè§é¢ä¸è½½ï¼å¦æä»æè§é¢ä¸æ¯æ dash æºï¼è¯·ç»§ç»­ä½¿ç¨
+` æ¶åé¢åºè¯¥ä½¿ç¨ `=` èéç©ºæ ¼\n4.
+ä¸ªäººç©ºé´ãåéãæ¶èå¤¹ç­æ¹éä¸è½½æä¸æ¯æééæä½\n\n####
+åæ¶ä¸è½½éå å§é\n\n- åæ° `-s` æ `--with-section`\n- é»è®¤å¼
+`False`\n\n\n\n## ä» bilili1.x è¿ç§»\n\n### åæ¶çåè½\n\n- `- bilibili`
+ç®å½ççæ\n- æ­æ¾åè¡¨çæ\n- æºæ ¼å¼ä¿®æ¹åè½ï¼ä¸åæ¯æ
+flv æºè§é¢ä¸è½½ï¼å¦æä»æè§é¢ä¸æ¯æ dash æºï¼è¯·ç»§ç»­ä½¿ç¨
 bililiï¼\n- å¯¹ Python3.8 çæ¯æï¼æä½æ¯æ Python3.9\n-
 ä¸è½½åè¯¢é®\n\n### é»è®¤è¡ä¸ºçä¿®æ¹\n\n-
 ä½¿ç¨åç¨èéå¤çº¿ç¨è¿è¡ä¸è½½ï¼åæ¶ä¹ä¸æ¯æ¹éè§£ææ¹éä¸è½½ï¼èæ¯è¾¹è§£æè¾¹ä¸è½½\n-
 é»è®¤çæå¼¹å¹ä¸º ASS\n- é»è®¤å¯ç¨ä»å¤éåæºä¸è½½çç¹æ§\n-
 ä¸ä»å¯ä»¥æ§å¶æ¯å¦ä½¿ç¨ç³»ç»ä»£çï¼è¿è½éç½®ç¹å®çä»£çæå¡å¨\n\n###
 æ°å¢çç¹æ§\n\n- åè§é¢ä¸è½½ä¸æ¹éä¸è½½å½ä»¤åç¦»ï¼`bilili`
 å½ä»¤ä¸ `yutto --batch` ç¸ç±»ä¼¼ï¼\n- é³é¢/è§é¢ç¼ç éæ©\n-
-ä»ä¸è½½é³é¢/è§é¢\n- å­æ¾å­è·¯å¾çèªç±å®å¶\n- æ¯æ url alias\n-
-æ¯æ file scheme\n- æ´å¤çæ¹ä¸è½½æ¯æï¼ç°å·²æ¯æ UP
+ä»ä¸è½½é³é¢/è§é¢\n- å­æ¾å­è·¯å¾çèªç±å®å¶\n- æ¯æ url
+å«å\n- æ¯ææä»¶åè¡¨\n- æ´å¤çæ¹ä¸è½½æ¯æï¼ç°å·²æ¯æ UP
 ä¸»å¨é¨è§é¢ä¸è½½ï¼æ©å±å¶å®æ¹ä¸è½½æ¯æä¹å¾ç®åï¼\n-
 æ´å å®åç warning ä¸ error æç¤º\n- æ¯æä»è¾å¥ id
 å³å¯ä¸è½½ï¼aidãbvidãepisode_id ç­ï¼\n-
 æ¯ææè¿°æä»¶çæï¼å½åä»çªå§ï¼\n\n## å°æå·§\n\n### ä½¿ç¨
 uvloop æååç¨æç\n\nå¬è¯´ uvloop
 å¯ä»¥æé«åç¨æçï¼å¦æä½ çç³»ç»é Windows
 çè¯ï¼å¯ä»¥è¯ä¸ä¸å®è£ uvloopï¼\n\n```bash\npip install
@@ -242,18 +267,19 @@
 ä¼å¾å¿«æ¿ä»£ bilili å\n\nç­æåä¸ä¼ï¼bilili
 å¹¶ä¸ä¼æ¶å¤±ï¼å¨ä¸æ®µæ¶é´å bilili
 ä»ä¼åçº éæ§ç»´æ¤ï¼åªæ¯ä¸ä¼æä¾æ°ç¹æ§äºã\n\nyutto
 ç°å¨ä¹è¿ä¸æ¯éå¸¸ç¨³å®ï¼éè¦ç¨³å®çä½éªçè¯è¯·ç»§ç»­ä½¿ç¨
 bilili ï½\n\n## Roadmap\n\n### 2.0.0-beta\n\n- [x] feat: æ¯æ bare name
 (bare id, bare path)\n- [x] refactor: url åè¡¨è½å¤é¢çº¿æ§å±å¼\n- [x]
 feat: æ·»å åç§ return code\n- [x] test: ç¼åååæµè¯\n\n###
-2.0.0\n\n- [ ] feat: æç¨¿è§é¢æè¿°æä»¶æ¯æ\n- [ ] docs: å¯ç±ç
-logoï¼åååï¼æè°ä¼å logo åï¼ï¼\n- [ ] docs:
-å¯ç±çéæææ¡£ï¼å¯è½éè¦ VitePress å° 1.0ï¼\n\n### future\n\n-
-[ ] feat: å­å¹ãå¼¹å¹åµå¥è§é¢æ¯æï¼ä¹è®¸ï¼ï¼\n- [ ] feat:
+2.0.0\n\n- [ ] feat: æç¨¿è§é¢æè¿°æä»¶æ¯æ\n- [ ] refactor:
+æ´çè·¯å¾åéå\n- [ ] docs: å¯ç±ç logoï¼åååï¼æè°ä¼å
+logo åï¼ï¼\n- [ ] docs: å¯ç±çéæææ¡£ï¼å¯è½éè¦ VitePress å°
+1.0ï¼\n\n### future\n\n- [ ] feat:
+å­å¹ãå¼¹å¹åµå¥è§é¢æ¯æï¼ä¹è®¸ï¼ï¼\n- [ ] feat:
 å°é¢ä¸è½½æ¯æï¼ä¹è®¸ï¼ï¼\n- [ ] refactor:
 ä»¥æä»¶å½¢å¼æ¯ææ´å¤é³è§é¢å¤çæ¹é¢çåè½ï¼æ¯å¦ç±»ä¼¼
 autosub çå·¥å·ï¼ä¹è®¸ï¼ï¼\n- [ ] feat: æ´å¤æ¹ä¸è½½æ¯æ\n- [ ]
 feat: ä»¥åæ´å å¯ç±ï½\n\n## åè\n\n- åºæ¬ç»æï¼
 github.com/SigureMo/bilili>\n- åç¨ä¸è½½ï¼
 github.com/changmenseng/AsyncBilibiliDownloader>\n- å¼¹å¹è½¬æ¢ï¼
 github.com/ShigureLab/biliass>\n- æ ·å¼è®¾è®¡ï¼
```

### Comparing `yutto-2.0.0b8/PKG-INFO` & `yutto-2.0.0b9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yutto
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: 🧊 一个可爱且任性的 B 站视频下载器
 Home-page: https://github.com/SigureMo/yutto
 License: GPL-3.0
 Keywords: python,bilibili,video,downloader,danmaku
 Author: Nyakku Shigure
 Author-email: sigure.qaq@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
@@ -66,25 +66,24 @@
 ```
 
 ## 主要功能
 
 ### 已支持的下载类型
 
 <!-- prettier-ignore -->
-|type|batch|path template|
-|-|-|-|
-|投稿视频|:x:|`{title}`|
-|投稿视频|:white_check_mark:|`{title}/{name}`|
-|番剧|:x:|`{name}`|
-|番剧|:white_check_mark:|`{title}/{name}`|
-|用户指定收藏夹|:white_check_mark:|`{username}的收藏夹/{fav_title}/{title}/{name}`|
-|用户全部收藏夹|:white_check_mark:|`{username}的收藏夹/{fav_title}/{title}/{name}`|
-|UP 主个人空间|:white_check_mark:|`{username}的全部投稿视频/{title}/{name}`|
-
-<!-- TODO: 展示更多细节 -->
+|Type|Batch|Example url|Path template|
+|-|-|-|-|
+|投稿视频|:x:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ` <br/> `https://www.bilibili.com/video/av371660125` <br/> `https://www.bilibili.com/video/BV1vZ4y1M7mQ?p=1` <br/> `av371660125` <br/> `BV1vZ4y1M7mQ`|`{title}`|
+|投稿视频|:white_check_mark:|`https://www.bilibili.com/video/BV1vZ4y1M7mQ` <br/> `https://www.bilibili.com/video/av371660125`  <br/> `av371660125` <br/> `BV1vZ4y1M7mQ`|`{title}/{name}`|
+|番剧|:x:|`https://www.bilibili.com/bangumi/play/ep395211` <br/> `ep395211`|`{name}`|
+|番剧|:white_check_mark:|`https://www.bilibili.com/bangumi/play/ep395211` <br/> `https://www.bilibili.com/bangumi/play/ss38221` <br/> `https://www.bilibili.com/bangumi/media/md28233903` <br/> `ep395211` <br/> `ss38221` <br/> `md28233903`|`{title}/{name}`|
+|用户指定收藏夹|:white_check_mark:|`https://space.bilibili.com/100969474/favlist?fid=1306978874`|`{username}的收藏夹/{series_title}/{title}/{name}`|
+|用户全部收藏夹|:white_check_mark:|`https://space.bilibili.com/100969474/favlist`|`{username}的收藏夹/{series_title}/{title}/{name}`|
+|UP 主个人空间|:white_check_mark:|`https://space.bilibili.com/100969474/video`|`{username}的全部投稿视频/{title}/{name}`|
+|视频合集|:white_check_mark:|`https://space.bilibili.com/100969474/channel/seriesdetail?sid=1947439` <br/> `https://www.bilibili.com/medialist/play/100969474?business=space_series&business_id=1947439`|`{series_title}/{title}/{name}`|
 
 ### 基本命令
 
 yutto 的基本命令如下：
 
 ```bash
 yutto <url>
@@ -129,34 +128,37 @@
 -  默认值 `8`
 
 与 bilili 不同的是，yutto 并不是使用多线程实现并行下载，而是使用协程实现的，本参数限制的是最大的并行 Worker 数量。
 
 #### 指定视频清晰度等级
 
 -  参数 `-q` 或 `--video-quality`
--  可选值 `127 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16`
+-  可选值 `127 | 126 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16`
 -  默认值 `127`
 
 清晰度对应关系如下
 
 <!-- prettier-ignore -->
 |code|清晰度|
 |:-:|:-:|
 |127|8K 超高清|
+|126|杜比视界|
 |125|HDR 真彩|
 |120|4K 超清|
 |116|1080P 60帧|
 |112|1080P 高码率|
 |80|1080P 高清|
 |74|720P 60帧|
 |64|720P 高清|
 |32|480P 清晰|
 |16|360P 流畅|
 
-并不是说指定某个清晰度就一定会下载该清晰度的视频，yutto 只会尽可能满足你的要求，如果不存在指定的清晰度，yutto 就会按照默认的清晰度搜索机制进行调节，比如指定清晰度为 `80`，**首先会依次降清晰度搜索** `74`、`64`、`32`、`16`，如果依然找不到合适的则**继续升清晰度搜索** `112`、`116`、`120`、`125`、`127`。
+并不是说指定某个清晰度就一定会下载该清晰度的视频，yutto 只会尽可能满足你的要求，如果不存在指定的清晰度，yutto 就会按照默认的清晰度搜索机制进行调节，比如指定清晰度为 `80`，**首先会依次降清晰度搜索** `74`、`64`、`32`、`16`，如果依然找不到合适的则**继续升清晰度搜索** `112`、`116`、`120`、`125`、`126`、`127`。
+
+值得注意的是，目前杜比视界视频只能简单下载音视频流并合并，合并后并不能达到在线观看的效果。
 
 #### 指定音频码率等级
 
 -  参数 `-aq` 或 `--audio-quality`
 -  可选值 `30280 | 30232 | 30216`
 -  默认值 `30280`
 
@@ -165,28 +167,28 @@
 <!-- prettier-ignore -->
 |code|码率|
 |:-:|:-:|
 |30280|320kbps|
 |30232|128kbps|
 |30216|64kbps|
 
-清晰度自动调节机制与视频清晰度一致，也采用先降后升的匹配机制。
+码率自动调节机制与视频清晰度一致，也采用先降后升的匹配机制。
 
 #### 指定视频编码
 
 -  参数 `--vcodec`
--  下载编码可选值 `"hevc" | "avc"`
+-  下载编码可选值 `"av1" | "hevc" | "avc"`
 -  保存编码可选值 FFmpeg 所有可用的视频编码器
 -  默认值 `"avc:copy"`
 
 该参数略微复杂，前半部分表示在下载时**优先**选择哪一种编码的视频流，后半部分则表示在合并时如何编码视频流，两者使用 `:` 分隔。
 
 值得注意的是，前半的下载编码只是优先下载的编码而已，如果不存在该编码，则仍会像视频清晰度调节机制一样自动选择其余编码。
 
-而后半部分的参数如果设置成非 `copy` 的值则可以确保在下载完成后对其进行重新编码，而且不止支持 `hevc` 与 `avc`，只要你的 FFmpeg 支持的视频编码器，它都可以完成。
+而后半部分的参数如果设置成非 `copy` 的值则可以确保在下载完成后对其进行重新编码，而且不止支持 `av1`、`hevc` 与 `avc`，只要你的 FFmpeg 支持的视频编码器，它都可以完成。
 
 #### 指定音频编码
 
 -  参数 `--acodec`
 -  下载编码可选值 `"mp4a"`
 -  保存编码可选值 FFmpeg 所有可用的音频编码器
 -  默认值 `"mp4a:copy"`
@@ -246,15 +248,15 @@
 
 -  参数 `--tmp-dir`
 -  默认值是“存放根目录”即 `-d, --dir` 的值
 
 #### 存放子路径模板
 
 -  参数 `-tp` 或 `--subpath-template`
--  可选参数变量 `title | id | name | username | fav_title | pubdate` （以后可能会有更多）
+-  可选参数变量 `title | id | name | username | series_title | pubdate` （以后可能会有更多）
 -  默认值 `"{auto}"`
 
 通过配置子路径模板可以灵活地控制视频存放位置。
 
 默认情况是由 yutto 自动控制存放位置的。比如下载单个视频时默认就是直接存放在设定的根目录，不会创建一层容器目录，此时自动选择了 `{name}` 作为模板；而批量下载时则会根据视频层级生成多级目录，比如番剧会是 `{title}/{name}`，首先会在设定根目录里生成一个番剧名的目录，其内才会存放各个番剧剧集视频，这样方便了多个不同番剧的管理。当然，如果你仍希望将番剧直接存放在设定根目录下的话，可以修改该参数值为 `{name}`即可。
 
 另外，该功能语法由 Python format 函数模板语法提供，所以也支持一些高级的用法，比如 `{id:0>3}{name}`。
@@ -263,17 +265,20 @@
 
 <!-- prettier-ignore -->
 |Variable|Description|Scope|
 |-|-|-|
 |title|系列视频总标题（番剧名/投稿视频标题）|全部|
 |id|系列视频单 p 顺序标号|全部|
 |name|系列视频单 p 标题|全部|
-|username|UP 主用户名|个人空间、收藏夹下载|
+|username|UP 主用户名|个人空间、收藏夹、合集下载|
+|series_title|合集标题|收藏夹、视频合集下载|
 |pubdate|投稿日期|仅投稿视频|
 
+> 未来可能会对路径变量及默认路径模板进行调整
+
 #### url 别名文件路径
 
 -  参数 `-af` 或 `--alias-file`
 -  默认值 `None`
 
 指定别名文件路径，别名文件中存放一个别名与其对应的 url，使用空格或者 `=` 分隔，示例如下：
 
@@ -403,14 +408,15 @@
 ```
 
 下面是一些要注意的问题
 
 1. 这里使用的序号是视频的顺序序号，而不是番剧所标注的`第 n 话`，因为有可能会出现 `第 x.5 话` 等等的特殊情况，此时一定要按照顺序自行计数。
 2. 参数值里一定不要加空格
 3. 参数值开头为 `-` 时前面应该使用 `=` 而非空格
+4. 个人空间、合集、收藏夹等批量下载暂不支持选集操作
 
 #### 同时下载附加剧集
 
 -  参数 `-s` 或 `--with-section`
 -  默认值 `False`
 
 </details>
@@ -434,16 +440,16 @@
 
 ### 新增的特性
 
 -  单视频下载与批量下载命令分离（`bilili` 命令与 `yutto --batch` 相类似）
 -  音频/视频编码选择
 -  仅下载音频/视频
 -  存放子路径的自由定制
--  支持 url alias
--  支持 file scheme
+-  支持 url 别名
+-  支持文件列表
 -  更多的批下载支持（现已支持 UP 主全部视频下载，扩展其它批下载支持也很简单）
 -  更加完善的 warning 与 error 提示
 -  支持仅输入 id 即可下载（aid、bvid、episode_id 等）
 -  支持描述文件生成（当前仅番剧）
 
 ## 小技巧
 
@@ -535,14 +541,15 @@
 -  [x] refactor: url 列表能够预线性展开
 -  [x] feat: 添加各种 return code
 -  [x] test: 编写单元测试
 
 ### 2.0.0
 
 -  [ ] feat: 投稿视频描述文件支持
+-  [ ] refactor: 整理路径变量名
 -  [ ] docs: 可爱的 logo（呜呜呜，有谁会做 logo 嘛？）
 -  [ ] docs: 可爱的静态文档（可能需要 VitePress 到 1.0）
 
 ### future
 
 -  [ ] feat: 字幕、弹幕嵌入视频支持（也许？）
 -  [ ] feat: 封面下载支持（也许？）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yutto Version: 2.0.0b8 Summary: ð§
+Metadata-Version: 2.1 Name: yutto Version: 2.0.0b9 Summary: ð§
 ä¸ä¸ªå¯ç±ä¸ä»»æ§ç B ç«è§é¢ä¸è½½å¨ Home-page: https://github.com/
 SigureMo/yutto License: GPL-3.0 Keywords:
 python,bilibili,video,downloader,danmaku Author: Nyakku Shigure Author-email:
 sigure.qaq@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: Environment ::
 Console Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -20,23 +20,45 @@
 å®è£é¢è§ç å¨æ­¤ä¹åè¯·ç¡®ä¿å®è£ Python3.9
 åä»¥ä¸çæ¬ï¼å¹¶éç½®å¥½ FFmpegï¼åç§ [bilili ææ¡£](https://
 bilili.sigure.xyz/guide/getting-started.html)ï¼ å½å yutto å°å¤äº beta
 é¶æ®µï¼æä»»ä½å»ºè®®å°½ç®¡å¨ [Discussions](https://github.com/SigureMo/
 yutto/discussions) æåºï½ï½ï½ ### pip å®è£ ```bash pip install --pre
 yutto ``` ### git clone ```bash git clone https://github.com/SigureMo/yutto.git
 cd yutto/ pip install poetry poetry build pip install ./dist/yutto-*.whl ``` ##
-ä¸»è¦åè½ ### å·²æ¯æçä¸è½½ç±»å |type|batch|path template| |-|-|-
-| |æç¨¿è§é¢|:x:|`{title}`| |æç¨¿è§é¢|:white_check_mark:|`{title}/
-{name}`| |çªå§|:x:|`{name}`| |çªå§|:white_check_mark:|`{title}/{name}`|
-|ç¨æ·æå®æ¶èå¤¹|:white_check_mark:|`{username}çæ¶èå¤¹/{fav_title}/
-{title}/{name}`| |ç¨æ·å¨é¨æ¶èå¤¹|:white_check_mark:|`
-{username}çæ¶èå¤¹/{fav_title}/{title}/{name}`| |UP ä¸»ä¸ªäººç©ºé´|:
-white_check_mark:|`{username}çå¨é¨æç¨¿è§é¢/{title}/{name}`| ###
-åºæ¬å½ä»¤ yutto çåºæ¬å½ä»¤å¦ä¸ï¼ ```bash yutto ``` ä½ å¯ä»¥éè¿
-`yutto -h` æ¥çè¯¦ç»å½ä»¤åæ°ã
+ä¸»è¦åè½ ### å·²æ¯æçä¸è½½ç±»å |Type|Batch|Example url|Path
+template| |-|-|-|-| |æç¨¿è§é¢|:x:|`https://www.bilibili.com/video/
+BV1vZ4y1M7mQ`
+`https://www.bilibili.com/video/av371660125`
+`https://www.bilibili.com/video/BV1vZ4y1M7mQ?p=1`
+`av371660125`
+`BV1vZ4y1M7mQ`|`{title}`| |æç¨¿è§é¢|:white_check_mark:|`https://
+www.bilibili.com/video/BV1vZ4y1M7mQ`
+`https://www.bilibili.com/video/av371660125`
+`av371660125`
+`BV1vZ4y1M7mQ`|`{title}/{name}`| |çªå§|:x:|`https://www.bilibili.com/bangumi/
+play/ep395211`
+`ep395211`|`{name}`| |çªå§|:white_check_mark:|`https://www.bilibili.com/
+bangumi/play/ep395211`
+`https://www.bilibili.com/bangumi/play/ss38221`
+`https://www.bilibili.com/bangumi/media/md28233903`
+`ep395211`
+`ss38221`
+`md28233903`|`{title}/{name}`| |ç¨æ·æå®æ¶èå¤¹|:white_check_mark:
+|`https://space.bilibili.com/100969474/favlist?fid=1306978874`|`
+{username}çæ¶èå¤¹/{series_title}/{title}/{name}`| |ç¨æ·å¨é¨æ¶èå¤¹|:
+white_check_mark:|`https://space.bilibili.com/100969474/favlist`|`
+{username}çæ¶èå¤¹/{series_title}/{title}/{name}`| |UP ä¸»ä¸ªäººç©ºé´|:
+white_check_mark:|`https://space.bilibili.com/100969474/video`|`
+{username}çå¨é¨æç¨¿è§é¢/{title}/{name}`| |è§é¢åé|:
+white_check_mark:|`https://space.bilibili.com/100969474/channel/
+seriesdetail?sid=1947439`
+`https://www.bilibili.com/medialist/play/
+100969474?business=space_series&business_id=1947439`|`{series_title}/{title}/
+{name}`| ### åºæ¬å½ä»¤ yutto çåºæ¬å½ä»¤å¦ä¸ï¼ ```bash yutto ```
+ä½ å¯ä»¥éè¿ `yutto -h` æ¥çè¯¦ç»å½ä»¤åæ°ã
 å¦æä½ éè¦ä¸è½½**åä¸ª**è§é¢ï¼åªéè¦ä½¿ç¨ yutto
 å ä¸è¿ä¸ªè§é¢çå°åå³å¯ãå®æ¯æ av/BV å·ä»¥åç¸åºå¸¦ p=n
 åæ°çæç¨¿è§é¢é¡µé¢ï¼ä¹æ¯æ ep
 å·ï¼episode_idï¼ççªå§é¡µé¢ã æ¯å¦åªéè¦è¿æ ·ä½ å°±å¯ä»¥ä¸è½½
 [ãè»¢ã¹ã©æ¥è¨ã](https://www.bilibili.com/bangumi/play/
 ep395211)ç¬¬ä¸è¯ï¼ ```bash yutto https://www.bilibili.com/bangumi/play/
 ep395211 ``` yutto è¿æ¯æç´æ¥ä½¿ç¨è½å¤å¯ä¸å®ä½èµæºç id
@@ -52,38 +74,39 @@
 åºç¡åæ° > å¤§é¨ååæ°ä¸ bilili éåï¼å¯åè [bilili ç cli
 ææ¡£](https://bilili.nyakku.moe/cli/) yutto
 æ¯æä¸äºåºç¡åæ°ï¼æ è®ºæ¯æ¹éä¸è½½è¿æ¯åè§é¢ä¸è½½é½éç¨ã
 ç¹å»å±å¼è¯¦ç»åæ° #### æå¤§å¹¶è¡ worker æ°é - åæ° `-n` æ `--
 num-workers` - é»è®¤å¼ `8` ä¸ bilili ä¸åçæ¯ï¼yutto
 å¹¶ä¸æ¯ä½¿ç¨å¤çº¿ç¨å®ç°å¹¶è¡ä¸è½½ï¼èæ¯ä½¿ç¨åç¨å®ç°çï¼æ¬åæ°éå¶çæ¯æå¤§çå¹¶è¡
 Worker æ°éã #### æå®è§é¢æ¸æ°åº¦ç­çº§ - åæ° `-q` æ `--video-
-quality` - å¯éå¼ `127 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 | 16` -
-é»è®¤å¼ `127` æ¸æ°åº¦å¯¹åºå³ç³»å¦ä¸ |code|æ¸æ°åº¦| |:-:|:-:| |127|8K
-è¶é«æ¸| |125|HDR çå½©| |120|4K è¶æ¸| |116|1080P 60å¸§| |112|1080P
-é«ç ç| |80|1080P é«æ¸| |74|720P 60å¸§| |64|720P é«æ¸| |32|480P æ¸æ°|
-|16|360P æµç|
+quality` - å¯éå¼ `127 | 126 | 125 | 120 | 116 | 112 | 80 | 74 | 64 | 32 |
+16` - é»è®¤å¼ `127` æ¸æ°åº¦å¯¹åºå³ç³»å¦ä¸ |code|æ¸æ°åº¦| |:-:|:-:
+| |127|8K è¶é«æ¸| |126|ææ¯è§ç| |125|HDR çå½©| |120|4K è¶æ¸|
+|116|1080P 60å¸§| |112|1080P é«ç ç| |80|1080P é«æ¸| |74|720P 60å¸§|
+|64|720P é«æ¸| |32|480P æ¸æ°| |16|360P æµç|
 å¹¶ä¸æ¯è¯´æå®æä¸ªæ¸æ°åº¦å°±ä¸å®ä¼ä¸è½½è¯¥æ¸æ°åº¦çè§é¢ï¼yutto
 åªä¼å°½å¯è½æ»¡è¶³ä½ çè¦æ±ï¼å¦æä¸å­å¨æå®çæ¸æ°åº¦ï¼yutto
 å°±ä¼æç§é»è®¤çæ¸æ°åº¦æç´¢æºå¶è¿è¡è°èï¼æ¯å¦æå®æ¸æ°åº¦ä¸º
 `80`ï¼**é¦åä¼ä¾æ¬¡éæ¸æ°åº¦æç´¢**
 `74`ã`64`ã`32`ã`16`ï¼å¦æä¾ç¶æ¾ä¸å°åéçå**ç»§ç»­åæ¸æ°åº¦æç´¢**
-`112`ã`116`ã`120`ã`125`ã`127`ã #### æå®é³é¢ç çç­çº§ - åæ°
-`-aq` æ `--audio-quality` - å¯éå¼ `30280 | 30232 | 30216` - é»è®¤å¼
-`30280` ç çå¯¹åºå³ç³»å¦ä¸ |code|ç ç| |:-:|:-:| |30280|320kbps|
-|30232|128kbps| |30216|64kbps|
-æ¸æ°åº¦èªå¨è°èæºå¶ä¸è§é¢æ¸æ°åº¦ä¸è´ï¼ä¹éç¨åéååçå¹éæºå¶ã
-#### æå®è§é¢ç¼ç  - åæ° `--vcodec` - ä¸è½½ç¼ç å¯éå¼ `"hevc" |
-"avc"` - ä¿å­ç¼ç å¯éå¼ FFmpeg ææå¯ç¨çè§é¢ç¼ç å¨ -
+`112`ã`116`ã`120`ã`125`ã`126`ã`127`ã
+å¼å¾æ³¨æçæ¯ï¼ç®åææ¯è§çè§é¢åªè½ç®åä¸è½½é³è§é¢æµå¹¶åå¹¶ï¼åå¹¶åå¹¶ä¸è½è¾¾å°å¨çº¿è§ççææã
+#### æå®é³é¢ç çç­çº§ - åæ° `-aq` æ `--audio-quality` - å¯éå¼
+`30280 | 30232 | 30216` - é»è®¤å¼ `30280` ç çå¯¹åºå³ç³»å¦ä¸
+|code|ç ç| |:-:|:-:| |30280|320kbps| |30232|128kbps| |30216|64kbps|
+ç çèªå¨è°èæºå¶ä¸è§é¢æ¸æ°åº¦ä¸è´ï¼ä¹éç¨åéååçå¹éæºå¶ã
+#### æå®è§é¢ç¼ç  - åæ° `--vcodec` - ä¸è½½ç¼ç å¯éå¼ `"av1" |
+"hevc" | "avc"` - ä¿å­ç¼ç å¯éå¼ FFmpeg ææå¯ç¨çè§é¢ç¼ç å¨ -
 é»è®¤å¼ `"avc:copy"`
 è¯¥åæ°ç¥å¾®å¤æï¼ååé¨åè¡¨ç¤ºå¨ä¸è½½æ¶**ä¼å**éæ©åªä¸ç§ç¼ç çè§é¢æµï¼ååé¨ååè¡¨ç¤ºå¨åå¹¶æ¶å¦ä½ç¼ç è§é¢æµï¼ä¸¤èä½¿ç¨
 `:` åéã
 å¼å¾æ³¨æçæ¯ï¼ååçä¸è½½ç¼ç åªæ¯ä¼åä¸è½½çç¼ç èå·²ï¼å¦æä¸å­å¨è¯¥ç¼ç ï¼åä»ä¼åè§é¢æ¸æ°åº¦è°èæºå¶ä¸æ ·èªå¨éæ©å¶ä½ç¼ç ã
 èååé¨åçåæ°å¦æè®¾ç½®æé `copy`
 çå¼åå¯ä»¥ç¡®ä¿å¨ä¸è½½å®æåå¯¹å¶è¿è¡éæ°ç¼ç ï¼èä¸ä¸æ­¢æ¯æ
-`hevc` ä¸ `avc`ï¼åªè¦ä½ ç FFmpeg
+`av1`ã`hevc` ä¸ `avc`ï¼åªè¦ä½ ç FFmpeg
 æ¯æçè§é¢ç¼ç å¨ï¼å®é½å¯ä»¥å®æã #### æå®é³é¢ç¼ç  -
 åæ° `--acodec` - ä¸è½½ç¼ç å¯éå¼ `"mp4a"` - ä¿å­ç¼ç å¯éå¼
 FFmpeg ææå¯ç¨çé³é¢ç¼ç å¨ - é»è®¤å¼ `"mp4a:copy"`
 è¯¦æåè§é¢ç¼ç ã #### ä»ä¸è½½è§é¢æµ - åæ° `--video-only` -
 é»è®¤å¼ `False` #### ä»ä¸è½½é³é¢æµ - åæ° `--audio-only` - é»è®¤å¼
 `False` ä»ä¸è½½å¶ä¸­çé³é¢æµï¼ä¿å­ä¸º `.aac` æä»¶ã
 å¼å¾æ³¨æçæ¯ï¼å¨ä¸éæ©è§é¢æµæ¶ï¼åµå¥å­å¹ãå¼¹å¹åè½å°æ æ³å·¥ä½ã
@@ -104,15 +127,15 @@
 ://url/to/proxy/server>` - é»è®¤å¼ `"auto"`
 è®¾ç½®ä»£çæå¡å¨ï¼é»è®¤æ¯ä»ç¯å¢åéè¯»åï¼`no`
 åä¸ºä¸è®¾ç½®ä»£çï¼è®¾ç½®å¶å® http/https url
 åå°å¶ä½ä¸ºä»£çæå¡å¨ã #### å­æ¾æ ¹ç®å½ - åæ° `-d` æ `--
 dir` - é»è®¤å¼ `"./"` #### ä¸´æ¶æä»¶ç®å½ - åæ° `--tmp-dir` -
 é»è®¤å¼æ¯âå­æ¾æ ¹ç®å½âå³ `-d, --dir` çå¼ ####
 å­æ¾å­è·¯å¾æ¨¡æ¿ - åæ° `-tp` æ `--subpath-template` -
-å¯éåæ°åé `title | id | name | username | fav_title | pubdate`
+å¯éåæ°åé `title | id | name | username | series_title | pubdate`
 ï¼ä»¥åå¯è½ä¼ææ´å¤ï¼ - é»è®¤å¼ `"{auto}"`
 éè¿éç½®å­è·¯å¾æ¨¡æ¿å¯ä»¥çµæ´»å°æ§å¶è§é¢å­æ¾ä½ç½®ã
 é»è®¤æåµæ¯ç± yutto
 èªå¨æ§å¶å­æ¾ä½ç½®çãæ¯å¦ä¸è½½åä¸ªè§é¢æ¶é»è®¤å°±æ¯ç´æ¥å­æ¾å¨è®¾å®çæ ¹ç®å½ï¼ä¸ä¼åå»ºä¸å±å®¹å¨ç®å½ï¼æ­¤æ¶èªå¨éæ©äº
 `{name}`
 ä½ä¸ºæ¨¡æ¿ï¼èæ¹éä¸è½½æ¶åä¼æ ¹æ®è§é¢å±çº§çæå¤çº§ç®å½ï¼æ¯å¦çªå§ä¼æ¯
 `{title}/
@@ -122,17 +145,19 @@
 0>3}{name}`ã
 å¼å¾æ³¨æçæ¯ï¼å¹¶ä¸æ¯ææåéå¨åç§åºåä¸é½ä¼æä¾ï¼æ¯å¦
 `username` åéå½åä»å¨ UP ä¸»å¨é¨æç¨¿è§é¢/
 æ¶èå¤¹ææä¾ï¼å¨å¶å®æåµä¸ä¸åºä½¿ç¨å®ãååéè¯¦ç»ä½ç¨åæè¿°è§ä¸è¡¨ï¼
 |Variable|Description|Scope| |-|-|-| |title|ç³»åè§é¢æ»æ é¢ï¼çªå§å/
 æç¨¿è§é¢æ é¢ï¼|å¨é¨| |id|ç³»åè§é¢å p é¡ºåºæ å·|å¨é¨|
 |name|ç³»åè§é¢å p æ é¢|å¨é¨| |username|UP
-ä¸»ç¨æ·å|ä¸ªäººç©ºé´ãæ¶èå¤¹ä¸è½½|
-|pubdate|æç¨¿æ¥æ|ä»æç¨¿è§é¢| #### url å«åæä»¶è·¯å¾ - åæ° `-
-af` æ `--alias-file` - é»è®¤å¼ `None`
+ä¸»ç¨æ·å|ä¸ªäººç©ºé´ãæ¶èå¤¹ãåéä¸è½½|
+|series_title|åéæ é¢|æ¶èå¤¹ãè§é¢åéä¸è½½|
+|pubdate|æç¨¿æ¥æ|ä»æç¨¿è§é¢| >
+æªæ¥å¯è½ä¼å¯¹è·¯å¾åéåé»è®¤è·¯å¾æ¨¡æ¿è¿è¡è°æ´ #### url
+å«åæä»¶è·¯å¾ - åæ° `-af` æ `--alias-file` - é»è®¤å¼ `None`
 æå®å«åæä»¶è·¯å¾ï¼å«åæä»¶ä¸­å­æ¾ä¸ä¸ªå«åä¸å¶å¯¹åºç
 urlï¼ä½¿ç¨ç©ºæ ¼æè `=` åéï¼ç¤ºä¾å¦ä¸ï¼ ``` rimuru1=https://
 www.bilibili.com/bangumi/play/ss25739/ rimuru2=https://www.bilibili.com/
 bangumi/play/ss36170/ rimuru-nikki=https://www.bilibili.com/bangumi/play/
 ss38221/ ``` æ¯å¦å°ä¸è¿°åå®¹å­å¨å°
 `~/.yutto_alias`ï¼åéè¿ä»¥ä¸å½ä»¤å³å¯è§£æè¯¥æä»¶ï¼ ```bash yutto
 rimuru1 --batch --alias-file='~/.yutto_alias' ``` å½åæ°å¼ä¸º `-
@@ -192,28 +217,29 @@
 p ^~3,10,12~14,16,-4~$ # å¾ææ¾ï¼ä¸é¢çä¾å­å°±æ¯ä¸è½½å 3 è¯ãç¬¬
 10 è¯ãç¬¬ 12 å° 14 è¯ãç¬¬ 16 è¯ä»¥åå 4 è¯ ```
 ä¸é¢æ¯ä¸äºè¦æ³¨æçé®é¢ 1.
 è¿éä½¿ç¨çåºå·æ¯è§é¢çé¡ºåºåºå·ï¼èä¸æ¯çªå§ææ æ³¨ç`ç¬¬
 n è¯`ï¼å ä¸ºæå¯è½ä¼åºç° `ç¬¬ x.5 è¯`
 ç­ç­çç¹æ®æåµï¼æ­¤æ¶ä¸å®è¦æç§é¡ºåºèªè¡è®¡æ°ã 2.
 åæ°å¼éä¸å®ä¸è¦å ç©ºæ ¼ 3. åæ°å¼å¼å¤´ä¸º `-
-` æ¶åé¢åºè¯¥ä½¿ç¨ `=` èéç©ºæ ¼ #### åæ¶ä¸è½½éå å§é - åæ°
-`-s` æ `--with-section` - é»è®¤å¼ `False` ## ä» bilili1.x è¿ç§» ###
-åæ¶çåè½ - `- bilibili` ç®å½ççæ - æ­æ¾åè¡¨çæ -
-æºæ ¼å¼ä¿®æ¹åè½ï¼ä¸åæ¯æ flv
+` æ¶åé¢åºè¯¥ä½¿ç¨ `=` èéç©ºæ ¼ 4.
+ä¸ªäººç©ºé´ãåéãæ¶èå¤¹ç­æ¹éä¸è½½æä¸æ¯æééæä½ ####
+åæ¶ä¸è½½éå å§é - åæ° `-s` æ `--with-section` - é»è®¤å¼ `False`
+## ä» bilili1.x è¿ç§» ### åæ¶çåè½ - `- bilibili` ç®å½ççæ -
+æ­æ¾åè¡¨çæ - æºæ ¼å¼ä¿®æ¹åè½ï¼ä¸åæ¯æ flv
 æºè§é¢ä¸è½½ï¼å¦æä»æè§é¢ä¸æ¯æ dash æºï¼è¯·ç»§ç»­ä½¿ç¨
 bililiï¼ - å¯¹ Python3.8 çæ¯æï¼æä½æ¯æ Python3.9 - ä¸è½½åè¯¢é®
 ### é»è®¤è¡ä¸ºçä¿®æ¹ -
 ä½¿ç¨åç¨èéå¤çº¿ç¨è¿è¡ä¸è½½ï¼åæ¶ä¹ä¸æ¯æ¹éè§£ææ¹éä¸è½½ï¼èæ¯è¾¹è§£æè¾¹ä¸è½½
 - é»è®¤çæå¼¹å¹ä¸º ASS - é»è®¤å¯ç¨ä»å¤éåæºä¸è½½çç¹æ§ -
 ä¸ä»å¯ä»¥æ§å¶æ¯å¦ä½¿ç¨ç³»ç»ä»£çï¼è¿è½éç½®ç¹å®çä»£çæå¡å¨
 ### æ°å¢çç¹æ§ - åè§é¢ä¸è½½ä¸æ¹éä¸è½½å½ä»¤åç¦»ï¼`bilili`
 å½ä»¤ä¸ `yutto --batch` ç¸ç±»ä¼¼ï¼ - é³é¢/è§é¢ç¼ç éæ© -
-ä»ä¸è½½é³é¢/è§é¢ - å­æ¾å­è·¯å¾çèªç±å®å¶ - æ¯æ url alias -
-æ¯æ file scheme - æ´å¤çæ¹ä¸è½½æ¯æï¼ç°å·²æ¯æ UP
+ä»ä¸è½½é³é¢/è§é¢ - å­æ¾å­è·¯å¾çèªç±å®å¶ - æ¯æ url å«å -
+æ¯ææä»¶åè¡¨ - æ´å¤çæ¹ä¸è½½æ¯æï¼ç°å·²æ¯æ UP
 ä¸»å¨é¨è§é¢ä¸è½½ï¼æ©å±å¶å®æ¹ä¸è½½æ¯æä¹å¾ç®åï¼ -
 æ´å å®åç warning ä¸ error æç¤º - æ¯æä»è¾å¥ id
 å³å¯ä¸è½½ï¼aidãbvidãepisode_id ç­ï¼ -
 æ¯ææè¿°æä»¶çæï¼å½åä»çªå§ï¼ ## å°æå·§ ### ä½¿ç¨ uvloop
 æååç¨æç å¬è¯´ uvloop
 å¯ä»¥æé«åç¨æçï¼å¦æä½ çç³»ç»é Windows
 çè¯ï¼å¯ä»¥è¯ä¸ä¸å®è£ uvloopï¼ ```bash pip install uvloop ```
@@ -247,16 +273,16 @@
 www.bilibili.com/bangumi/play/ep395211?t=24) ### yutto ä¼å¾å¿«æ¿ä»£ bilili
 å ç­æåä¸ä¼ï¼bilili å¹¶ä¸ä¼æ¶å¤±ï¼å¨ä¸æ®µæ¶é´å bilili
 ä»ä¼åçº éæ§ç»´æ¤ï¼åªæ¯ä¸ä¼æä¾æ°ç¹æ§äºã yutto
 ç°å¨ä¹è¿ä¸æ¯éå¸¸ç¨³å®ï¼éè¦ç¨³å®çä½éªçè¯è¯·ç»§ç»­ä½¿ç¨
 bilili ï½ ## Roadmap ### 2.0.0-beta - [x] feat: æ¯æ bare name (bare id,
 bare path) - [x] refactor: url åè¡¨è½å¤é¢çº¿æ§å±å¼ - [x] feat:
 æ·»å åç§ return code - [x] test: ç¼åååæµè¯ ### 2.0.0 - [ ] feat:
-æç¨¿è§é¢æè¿°æä»¶æ¯æ - [ ] docs: å¯ç±ç
-logoï¼åååï¼æè°ä¼å logo åï¼ï¼ - [ ] docs:
+æç¨¿è§é¢æè¿°æä»¶æ¯æ - [ ] refactor: æ´çè·¯å¾åéå - [ ]
+docs: å¯ç±ç logoï¼åååï¼æè°ä¼å logo åï¼ï¼ - [ ] docs:
 å¯ç±çéæææ¡£ï¼å¯è½éè¦ VitePress å° 1.0ï¼ ### future - [ ]
 feat: å­å¹ãå¼¹å¹åµå¥è§é¢æ¯æï¼ä¹è®¸ï¼ï¼ - [ ] feat:
 å°é¢ä¸è½½æ¯æï¼ä¹è®¸ï¼ï¼ - [ ] refactor:
 ä»¥æä»¶å½¢å¼æ¯ææ´å¤é³è§é¢å¤çæ¹é¢çåè½ï¼æ¯å¦ç±»ä¼¼
 autosub çå·¥å·ï¼ä¹è®¸ï¼ï¼ - [ ] feat: æ´å¤æ¹ä¸è½½æ¯æ - [ ] feat:
 ä»¥åæ´å å¯ç±ï½ ## åè - åºæ¬ç»æï¼
 github.com/SigureMo/bilili> - åç¨ä¸è½½ï¼
```

