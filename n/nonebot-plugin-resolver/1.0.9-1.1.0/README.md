# Comparing `tmp/nonebot_plugin_resolver-1.0.9.tar.gz` & `tmp/nonebot_plugin_resolver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_resolver-1.0.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_resolver-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_resolver-1.0.9.tar` & `nonebot_plugin_resolver-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    13557 2023-02-16 16:48:33.888227 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/__init__.py
--rw-r--r--   0        0        0     4279 2023-02-16 08:27:09.540780 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/acfun_utils.py
--rw-r--r--   0        0        0     2992 2023-02-16 08:49:32.884612 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/bili23_utils.py
--rw-r--r--   0        0        0     2960 2023-02-16 08:41:49.053046 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/common_utils.py
--rw-r--r--   0        0        0      304 2023-02-16 08:27:09.514781 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/tiktok_utills.py
--rw-r--r--   0        0        0      204 2023-02-16 08:41:49.057046 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/twitter_utils.py
--rw-r--r--   0        0        0        0 2023-02-16 08:12:05.385391 nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/xhs_utils.py
--rw-r--r--   0        0        0      723 2023-02-16 16:48:45.906391 nonebot_plugin_resolver-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     1646 2023-02-16 16:07:56.464735 nonebot_plugin_resolver-1.0.9/README.md
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.0.9/setup.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     2101 2024-06-02 07:56:22.198471 nonebot_plugin_resolver-1.1.0/README.md
+-rw-r--r--   0        0        0    22283 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/__init__.py
+-rw-r--r--   0        0        0    16457 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/a-bogus.js
+-rw-r--r--   0        0        0     4282 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/acfun_utils.py
+-rw-r--r--   0        0        0     2904 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/bili23_utils.py
+-rw-r--r--   0        0        0     2960 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/common_utils.py
+-rw-r--r--   0        0        0      285 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/config.py
+-rw-r--r--   0        0        0     1156 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/constants.py
+-rw-r--r--   0        0        0      920 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/freyrjs.py
+-rw-r--r--   0        0        0     2363 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/tiktok_utills.py
+-rw-r--r--   0        0        0     1104 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/ytdlp_utils.py
+-rw-r--r--   0        0        0      729 2024-06-02 07:56:22.206471 nonebot_plugin_resolver-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 nonebot_plugin_resolver-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/acfun_utils.py` & `nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/acfun_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,128 @@
-import json
-import re
-import subprocess
-import os
-
-import httpx
-
-headers = {
-    'referer': 'https://www.acfun.cn/',
-    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83'
-}
-
-def parse_url(url: str):
-    """
-        解析acfun链接
-    :param url:
-    :return:
-    """
-    url_suffix = "?quickViewId=videoInfo_new&ajaxpipe=1"
-    url = url + url_suffix
-    # print(url)
-
-    raw = httpx.get(url, headers=headers).text
-    strs_remove_header = raw.split("window.pageInfo = window.videoInfo =")
-    strs_remove_tail = strs_remove_header[1].split("</script>")
-    str_json = strs_remove_tail[0]
-    str_json_escaped = escape_special_chars(str_json)
-    video_info = json.loads(str_json_escaped)
-    # print(video_info)
-    video_name = parse_video_name_fixed(video_info)
-    ks_play_json = video_info['currentVideoInfo']['ksPlayJson']
-    ks_play = json.loads(ks_play_json)
-    representations = ks_play['adaptationSet'][0]['representation']
-    url_m3u8s = [d['url'] for d in representations][0]
-    return url_m3u8s, video_name
-
-
-def parse_m3u8(m3u8_url: str):
-    """
-        解析m3u8链接
-    :param m3u8_url:
-    :return:
-    """
-    m3u8_file = httpx.get(m3u8_url, headers=headers).text
-    # 分离ts文件链接
-    raw_pieces = re.split(r"\n#EXTINF:.{8},\n", m3u8_file)
-    # print(raw_pieces)
-    # 过滤头部\
-    m3u8_relative_links = raw_pieces[1:]
-    # print(m3u8_relative_links)
-    # 修改尾部 去掉尾部多余的结束符
-    patched_tail = m3u8_relative_links[-1].split("\n")[0]
-    m3u8_relative_links[-1] = patched_tail
-    # print(m3u8_relative_links)
-
-    # 完整链接，直接加m3u8Url的通用前缀
-    m3u8_prefix = "/".join(m3u8_url.split("/")[0:-1])
-    m3u8_full_urls = [m3u8_prefix + "/" + d for d in m3u8_relative_links]
-    # aria2c下载的文件名，就是取url最后一段，去掉末尾url参数(?之后是url参数)
-    ts_names = [d.split("?")[0] for d in m3u8_relative_links]
-    # print(ts_names)
-    output_folder_name = ts_names[0][:-9]
-    output_file_name = output_folder_name + ".mp4"
-    # print(output_file_name)
-    return m3u8_full_urls, ts_names, output_folder_name, output_file_name
-
-
-async def download_m3u8_videos(m3u8_full_url, i):
-    """
-        批量下载m3u8
-    :param m3u8_full_urls:
-    :return:
-    """
-    async with httpx.AsyncClient() as client:
-        async with client.stream("GET", m3u8_full_url, headers=headers) as resp:
-            with open(f"{i}.ts", "wb") as f:
-                async for chunk in resp.aiter_bytes():
-                    f.write(chunk)
-
-def escape_special_chars(str_json):
-    return str_json.replace('\\\\"', '\\"').replace('\\"', '"')
-
-
-def parse_video_name(video_info: json):
-    """
-        获取视频信息
-    :param video_info:
-    :return:
-    """
-    ac_id = "ac" + video_info['dougaId'] if video_info['dougaId'] is not None else ""
-    title = video_info['title'] if video_info['title'] is not None else ""
-    author = video_info['user']['name'] if video_info['user']['name'] is not None else ""
-    upload_time = video_info['createTime'] if video_info['createTime'] is not None else ""
-    desc = video_info['description'] if video_info['description'] is not None else ""
-
-    raw = '_'.join([ac_id, title, author, upload_time, desc])[:101]
-    return raw
-
-def merge_ac_file_to_mp4(ts_names, full_file_name, should_delete = True):
-
-    concat_str = '\n'.join([f"file {i}.ts" for i, d in enumerate(ts_names)])
-    # print(concat_str)
-    with open('file.txt', 'w') as f:
-        f.write(concat_str)
-
-    subprocess.call(f'ffmpeg -y -f concat -safe 0 -i "file.txt" -c copy "{full_file_name}"', shell=True,
-                    stdout=subprocess.DEVNULL,
-                    stderr=subprocess.DEVNULL,
-    )
-    if should_delete:
-        os.unlink('file.txt')
-        # os.unlink(full_file_name)
-        for i in range(len(ts_names)):
-            os.unlink(f'{i}.ts')
-
-
-
-def parse_video_name_fixed(video_info: json):
-    """
-        校准文件名
-    :param video_info:
-    :return:
-    """
-    f = parse_video_name(video_info)
-    t = f.replace(" ", "-")
+import json
+import re
+import subprocess
+import os
+
+import httpx
+
+headers = {
+    'referer': 'https://www.acfun.cn/',
+    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83'
+}
+
+def parse_url(url: str):
+    """
+        解析acfun链接
+    :param url:
+    :return:
+    """
+    url_suffix = "?quickViewId=videoInfo_new&ajaxpipe=1"
+    url = url + url_suffix
+    # print(url)
+
+    raw = httpx.get(url, headers=headers).text
+    strs_remove_header = raw.split("window.pageInfo = window.videoInfo =")
+    strs_remove_tail = strs_remove_header[1].split("</script>")
+    str_json = strs_remove_tail[0]
+    str_json_escaped = escape_special_chars(str_json)
+    video_info = json.loads(str_json_escaped)
+    # print(video_info)
+    video_name = parse_video_name_fixed(video_info)
+    ks_play_json = video_info['currentVideoInfo']['ksPlayJson']
+    ks_play = json.loads(ks_play_json)
+    representations = ks_play['adaptationSet'][0]['representation']
+    # 这里[d['url'] for d in representations]，从4k~360，此处默认720p
+    url_m3u8s = [d['url'] for d in representations][3]
+    # print([d['url'] for d in representations])
+    return url_m3u8s, video_name
+
+
+def parse_m3u8(m3u8_url: str):
+    """
+        解析m3u8链接
+    :param m3u8_url:
+    :return:
+    """
+    m3u8_file = httpx.get(m3u8_url, headers=headers).text
+    # 分离ts文件链接
+    raw_pieces = re.split(r"\n#EXTINF:.{8},\n", m3u8_file)
+    # print(raw_pieces)
+    # 过滤头部\
+    m3u8_relative_links = raw_pieces[1:]
+    # print(m3u8_relative_links)
+    # 修改尾部 去掉尾部多余的结束符
+    patched_tail = m3u8_relative_links[-1].split("\n")[0]
+    m3u8_relative_links[-1] = patched_tail
+    # print(m3u8_relative_links)
+
+    # 完整链接，直接加m3u8Url的通用前缀
+    m3u8_prefix = "/".join(m3u8_url.split("/")[0:-1])
+    m3u8_full_urls = [m3u8_prefix + "/" + d for d in m3u8_relative_links]
+    # aria2c下载的文件名，就是取url最后一段，去掉末尾url参数(?之后是url参数)
+    ts_names = [d.split("?")[0] for d in m3u8_relative_links]
+    # print(ts_names)
+    output_folder_name = ts_names[0][:-9]
+    output_file_name = output_folder_name + ".mp4"
+    # print(output_file_name)
+    return m3u8_full_urls, ts_names, output_folder_name, output_file_name
+
+
+async def download_m3u8_videos(m3u8_full_url, i):
+    """
+        批量下载m3u8
+    :param m3u8_full_urls:
+    :return:
+    """
+    async with httpx.AsyncClient() as client:
+        async with client.stream("GET", m3u8_full_url, headers=headers) as resp:
+            with open(f"{i}.ts", "wb") as f:
+                async for chunk in resp.aiter_bytes():
+                    f.write(chunk)
+
+def escape_special_chars(str_json):
+    return str_json.replace('\\\\"', '\\"').replace('\\"', '"')
+
+
+def parse_video_name(video_info: json):
+    """
+        获取视频信息
+    :param video_info:
+    :return:
+    """
+    ac_id = "ac" + video_info['dougaId'] if video_info['dougaId'] is not None else ""
+    title = video_info['title'] if video_info['title'] is not None else ""
+    author = video_info['user']['name'] if video_info['user']['name'] is not None else ""
+    upload_time = video_info['createTime'] if video_info['createTime'] is not None else ""
+    desc = video_info['description'] if video_info['description'] is not None else ""
+
+    raw = '_'.join([ac_id, title, author, upload_time, desc])[:101]
+    return raw
+
+def merge_ac_file_to_mp4(ts_names, full_file_name, should_delete = True):
+
+    concat_str = '\n'.join([f"file {i}.ts" for i, d in enumerate(ts_names)])
+    # print(concat_str)
+    with open('file.txt', 'w') as f:
+        f.write(concat_str)
+
+    subprocess.call(f'ffmpeg -y -f concat -safe 0 -i "file.txt" -c copy "{full_file_name}"', shell=True,
+                    stdout=subprocess.DEVNULL,
+                    stderr=subprocess.DEVNULL,
+    )
+    if should_delete:
+        os.unlink('file.txt')
+        # os.unlink(full_file_name)
+        for i in range(len(ts_names)):
+            os.unlink(f'{i}.ts')
+
+
+
+def parse_video_name_fixed(video_info: json):
+    """
+        校准文件名
+    :param video_info:
+    :return:
+    """
+    f = parse_video_name(video_info)
+    t = f.replace(" ", "-")
     return t
```

### Comparing `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/bili23_utils.py` & `nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/bili23_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,187 +1,182 @@
-00000000: 696d 706f 7274 2068 7474 7078 0d0a 696d  import httpx..im
-00000010: 706f 7274 2072 650d 0a69 6d70 6f72 7420  port re..import 
-00000020: 6a73 6f6e 0d0a 696d 706f 7274 2073 7562  json..import sub
-00000030: 7072 6f63 6573 730d 0a69 6d70 6f72 7420  process..import 
-00000040: 6f73 0d0a 0d0a 6672 6f6d 202e 636f 6d6d  os....from .comm
-00000050: 6f6e 5f75 7469 6c73 2069 6d70 6f72 7420  on_utils import 
-00000060: 646f 776e 6c6f 6164 5f69 6d67 0d0a 0d0a  download_img....
-00000070: 6865 6164 6572 203d 207b 0d0a 2020 2020  header = {..    
-00000080: 2755 7365 722d 4167 656e 7427 3a0d 0a20  'User-Agent':.. 
-00000090: 2020 2020 2020 2027 4d6f 7a69 6c6c 612f         'Mozilla/
-000000a0: 352e 3020 2857 696e 646f 7773 204e 5420  5.0 (Windows NT 
-000000b0: 3130 2e30 3b20 5769 6e36 343b 2078 3634  10.0; Win64; x64
-000000c0: 2920 4170 706c 6557 6562 4b69 742f 3533  ) AppleWebKit/53
-000000d0: 372e 3336 2028 4b48 544d 4c2c 206c 696b  7.36 (KHTML, lik
-000000e0: 6520 4765 636b 6f29 2043 6872 6f6d 652f  e Gecko) Chrome/
-000000f0: 3130 302e 302e 3438 3936 2e31 3237 2053  100.0.4896.127 S
-00000100: 6166 6172 692f 3533 372e 3336 272c 0d0a  afari/537.36',..
-00000110: 2020 2020 2772 6566 6572 6572 273a 2027      'referer': '
-00000120: 6874 7470 733a 2f2f 7777 772e 6269 6c69  https://www.bili
-00000130: 6269 6c69 2e63 6f6d 272c 0d0a 7d0d 0a0d  bili.com',..}...
-00000140: 0a0d 0a64 6566 2067 6574 446f 776e 6c6f  ...def getDownlo
-00000150: 6164 5572 6c28 7572 6c3a 2073 7472 293a  adUrl(url: str):
-00000160: 0d0a 2020 2020 2222 220d 0a20 2020 2020  ..    """..     
-00000170: 2020 20e7 88ac e58f 96e4 b88b e8bd bde9     .............
-00000180: 93be e68e a50d 0a20 2020 203a 7061 7261  .......    :para
-00000190: 6d20 7572 6c3a 0d0a 2020 2020 3a72 6574  m url:..    :ret
-000001a0: 7572 6e3a 0d0a 2020 2020 2222 220d 0a20  urn:..    """.. 
-000001b0: 2020 2077 6974 6820 6874 7470 782e 436c     with httpx.Cl
-000001c0: 6965 6e74 2866 6f6c 6c6f 775f 7265 6469  ient(follow_redi
-000001d0: 7265 6374 733d 5472 7565 2920 6173 2063  rects=True) as c
-000001e0: 6c69 656e 743a 0d0a 2020 2020 2020 2020  lient:..        
-000001f0: 7265 7370 203d 2063 6c69 656e 742e 6765  resp = client.ge
-00000200: 7428 7572 6c2c 2068 6561 6465 7273 3d68  t(url, headers=h
-00000210: 6561 6465 7229 0d0a 2020 2020 2020 2020  eader)..        
-00000220: 696e 666f 203d 2072 652e 7365 6172 6368  info = re.search
-00000230: 2872 223c 7363 7269 7074 3e77 696e 646f  (r"<script>windo
-00000240: 775c 2e5f 5f70 6c61 7969 6e66 6f5f 5f3d  w\.__playinfo__=
-00000250: 287b 2e2a 7d29 3c5c 2f73 6372 6970 743e  ({.*})<\/script>
-00000260: 3c73 6372 6970 743e 222c 2072 6573 702e  <script>", resp.
-00000270: 7465 7874 295b 315d 0d0a 2020 2020 2020  text)[1]..      
-00000280: 2020 7265 7320 3d20 6a73 6f6e 2e6c 6f61    res = json.loa
-00000290: 6473 2869 6e66 6f29 0d0a 2020 2020 2020  ds(info)..      
-000002a0: 2020 7669 6465 6f55 726c 203d 2072 6573    videoUrl = res
-000002b0: 5b22 6461 7461 225d 5b22 6461 7368 225d  ["data"]["dash"]
-000002c0: 5b22 7669 6465 6f22 5d5b 305d 5b22 6261  ["video"][0]["ba
-000002d0: 7365 5572 6c22 5d20 6f72 2072 6573 5b22  seUrl"] or res["
-000002e0: 6461 7461 225d 5b22 6461 7368 225d 5b22  data"]["dash"]["
-000002f0: 7669 6465 6f22 5d5b 305d 5b22 6261 636b  video"][0]["back
-00000300: 7570 5572 6c22 5d5b 305d 0d0a 2020 2020  upUrl"][0]..    
-00000310: 2020 2020 6175 6469 6f55 726c 203d 2072      audioUrl = r
-00000320: 6573 5b22 6461 7461 225d 5b22 6461 7368  es["data"]["dash
-00000330: 225d 5b22 6175 6469 6f22 5d5b 305d 5b22  "]["audio"][0]["
-00000340: 6261 7365 5572 6c22 5d20 6f72 2072 6573  baseUrl"] or res
-00000350: 5b22 6461 7461 225d 5b22 6461 7368 225d  ["data"]["dash"]
-00000360: 5b22 6175 6469 6f22 5d5b 305d 5b22 6261  ["audio"][0]["ba
-00000370: 636b 7570 5572 6c22 5d5b 305d 0d0a 2020  ckupUrl"][0]..  
-00000380: 2020 2020 2020 6966 2076 6964 656f 5572        if videoUr
-00000390: 6c20 213d 2022 2220 616e 6420 6175 6469  l != "" and audi
-000003a0: 6f55 726c 2021 3d20 2222 3a0d 0a20 2020  oUrl != "":..   
-000003b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000003c0: 7669 6465 6f55 726c 2c20 6175 6469 6f55  videoUrl, audioU
-000003d0: 726c 0d0a 0d0a 0d0a 6173 796e 6320 6465  rl......async de
-000003e0: 6620 646f 776e 6c6f 6164 4246 696c 6528  f downloadBFile(
-000003f0: 7572 6c2c 2066 756c 6c46 696c 654e 616d  url, fullFileNam
-00000400: 652c 2070 726f 6772 6573 7343 616c 6c62  e, progressCallb
-00000410: 6163 6b29 3a0d 0a20 2020 2022 2222 0d0a  ack):..    """..
-00000420: 2020 2020 2020 2020 e4b8 8be8 bdbd e8a7          ........
-00000430: 86e9 a291 e696 87e4 bbb6 e592 8ce9 9fb3  ................
-00000440: e9a2 91e6 9687 e4bb b60d 0a20 2020 203a  ...........    :
-00000450: 7061 7261 6d20 7572 6c3a 0d0a 2020 2020  param url:..    
-00000460: 3a70 6172 616d 2066 756c 6c46 696c 654e  :param fullFileN
-00000470: 616d 653a 0d0a 2020 2020 3a70 6172 616d  ame:..    :param
-00000480: 2070 726f 6772 6573 7343 616c 6c62 6163   progressCallbac
-00000490: 6b3a 0d0a 2020 2020 3a72 6574 7572 6e3a  k:..    :return:
-000004a0: 0d0a 2020 2020 2222 220d 0a20 2020 2061  ..    """..    a
-000004b0: 7379 6e63 2077 6974 6820 6874 7470 782e  sync with httpx.
-000004c0: 4173 796e 6343 6c69 656e 7428 2920 6173  AsyncClient() as
-000004d0: 2063 6c69 656e 743a 0d0a 2020 2020 2020   client:..      
-000004e0: 2020 6173 796e 6320 7769 7468 2063 6c69    async with cli
-000004f0: 656e 742e 7374 7265 616d 2822 4745 5422  ent.stream("GET"
-00000500: 2c20 7572 6c2c 2068 6561 6465 7273 3d68  , url, headers=h
-00000510: 6561 6465 7229 2061 7320 7265 7370 3a0d  eader) as resp:.
-00000520: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-00000530: 7265 6e74 4c65 6e20 3d20 300d 0a20 2020  rentLen = 0..   
-00000540: 2020 2020 2020 2020 2074 6f74 616c 4c65           totalLe
-00000550: 6e20 3d20 696e 7428 7265 7370 2e68 6561  n = int(resp.hea
-00000560: 6465 7273 5b27 636f 6e74 656e 742d 6c65  ders['content-le
-00000570: 6e67 7468 275d 290d 0a20 2020 2020 2020  ngth'])..       
-00000580: 2020 2020 2070 7269 6e74 2874 6f74 616c       print(total
-00000590: 4c65 6e29 0d0a 2020 2020 2020 2020 2020  Len)..          
-000005a0: 2020 7769 7468 206f 7065 6e28 6675 6c6c    with open(full
-000005b0: 4669 6c65 4e61 6d65 2c20 2277 6222 2920  FileName, "wb") 
-000005c0: 6173 2066 3a0d 0a20 2020 2020 2020 2020  as f:..         
-000005d0: 2020 2020 2020 2061 7379 6e63 2066 6f72         async for
-000005e0: 2063 6875 6e6b 2069 6e20 7265 7370 2e61   chunk in resp.a
-000005f0: 6974 6572 5f62 7974 6573 2829 3a0d 0a20  iter_bytes():.. 
+00000000: 696d 706f 7274 2068 7474 7078 0a69 6d70  import httpx.imp
+00000010: 6f72 7420 7265 0a69 6d70 6f72 7420 6a73  ort re.import js
+00000020: 6f6e 0a69 6d70 6f72 7420 7375 6270 726f  on.import subpro
+00000030: 6365 7373 0a69 6d70 6f72 7420 6f73 0a0a  cess.import os..
+00000040: 6672 6f6d 202e 636f 6d6d 6f6e 5f75 7469  from .common_uti
+00000050: 6c73 2069 6d70 6f72 7420 646f 776e 6c6f  ls import downlo
+00000060: 6164 5f69 6d67 0a0a 6865 6164 6572 203d  ad_img..header =
+00000070: 207b 0a20 2020 2027 5573 6572 2d41 6765   {.    'User-Age
+00000080: 6e74 273a 0a20 2020 2020 2020 2027 4d6f  nt':.        'Mo
+00000090: 7a69 6c6c 612f 352e 3020 2857 696e 646f  zilla/5.0 (Windo
+000000a0: 7773 204e 5420 3130 2e30 3b20 5769 6e36  ws NT 10.0; Win6
+000000b0: 343b 2078 3634 2920 4170 706c 6557 6562  4; x64) AppleWeb
+000000c0: 4b69 742f 3533 372e 3336 2028 4b48 544d  Kit/537.36 (KHTM
+000000d0: 4c2c 206c 696b 6520 4765 636b 6f29 2043  L, like Gecko) C
+000000e0: 6872 6f6d 652f 3130 302e 302e 3438 3936  hrome/100.0.4896
+000000f0: 2e31 3237 2053 6166 6172 692f 3533 372e  .127 Safari/537.
+00000100: 3336 272c 0a20 2020 2027 7265 6665 7265  36',.    'refere
+00000110: 7227 3a20 2768 7474 7073 3a2f 2f77 7777  r': 'https://www
+00000120: 2e62 696c 6962 696c 692e 636f 6d27 2c0a  .bilibili.com',.
+00000130: 7d0a 0a0a 6465 6620 6765 7444 6f77 6e6c  }...def getDownl
+00000140: 6f61 6455 726c 2875 726c 3a20 7374 7229  oadUrl(url: str)
+00000150: 3a0a 2020 2020 2222 220a 2020 2020 2020  :.    """.      
+00000160: 2020 e788 ace5 8f96 e4b8 8be8 bdbd e993    ..............
+00000170: bee6 8ea5 0a20 2020 203a 7061 7261 6d20  .....    :param 
+00000180: 7572 6c3a 0a20 2020 203a 7265 7475 726e  url:.    :return
+00000190: 3a0a 2020 2020 2222 220a 2020 2020 7769  :.    """.    wi
+000001a0: 7468 2068 7474 7078 2e43 6c69 656e 7428  th httpx.Client(
+000001b0: 666f 6c6c 6f77 5f72 6564 6972 6563 7473  follow_redirects
+000001c0: 3d54 7275 6529 2061 7320 636c 6965 6e74  =True) as client
+000001d0: 3a0a 2020 2020 2020 2020 7265 7370 203d  :.        resp =
+000001e0: 2063 6c69 656e 742e 6765 7428 7572 6c2c   client.get(url,
+000001f0: 2068 6561 6465 7273 3d68 6561 6465 7229   headers=header)
+00000200: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
+00000210: 7265 2e73 6561 7263 6828 7222 3c73 6372  re.search(r"<scr
+00000220: 6970 743e 7769 6e64 6f77 5c2e 5f5f 706c  ipt>window\.__pl
+00000230: 6179 696e 666f 5f5f 3d28 7b2e 2a7d 293c  ayinfo__=({.*})<
+00000240: 5c2f 7363 7269 7074 3e3c 7363 7269 7074  \/script><script
+00000250: 3e22 2c20 7265 7370 2e74 6578 7429 5b31  >", resp.text)[1
+00000260: 5d0a 2020 2020 2020 2020 7265 7320 3d20  ].        res = 
+00000270: 6a73 6f6e 2e6c 6f61 6473 2869 6e66 6f29  json.loads(info)
+00000280: 0a20 2020 2020 2020 2076 6964 656f 5572  .        videoUr
+00000290: 6c20 3d20 7265 735b 2264 6174 6122 5d5b  l = res["data"][
+000002a0: 2264 6173 6822 5d5b 2276 6964 656f 225d  "dash"]["video"]
+000002b0: 5b30 5d5b 2262 6173 6555 726c 225d 206f  [0]["baseUrl"] o
+000002c0: 7220 7265 735b 2264 6174 6122 5d5b 2264  r res["data"]["d
+000002d0: 6173 6822 5d5b 2276 6964 656f 225d 5b30  ash"]["video"][0
+000002e0: 5d5b 2262 6163 6b75 7055 726c 225d 5b30  ]["backupUrl"][0
+000002f0: 5d0a 2020 2020 2020 2020 6175 6469 6f55  ].        audioU
+00000300: 726c 203d 2072 6573 5b22 6461 7461 225d  rl = res["data"]
+00000310: 5b22 6461 7368 225d 5b22 6175 6469 6f22  ["dash"]["audio"
+00000320: 5d5b 305d 5b22 6261 7365 5572 6c22 5d20  ][0]["baseUrl"] 
+00000330: 6f72 2072 6573 5b22 6461 7461 225d 5b22  or res["data"]["
+00000340: 6461 7368 225d 5b22 6175 6469 6f22 5d5b  dash"]["audio"][
+00000350: 305d 5b22 6261 636b 7570 5572 6c22 5d5b  0]["backupUrl"][
+00000360: 305d 0a20 2020 2020 2020 2069 6620 7669  0].        if vi
+00000370: 6465 6f55 726c 2021 3d20 2222 2061 6e64  deoUrl != "" and
+00000380: 2061 7564 696f 5572 6c20 213d 2022 223a   audioUrl != "":
+00000390: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000003a0: 7572 6e20 7669 6465 6f55 726c 2c20 6175  urn videoUrl, au
+000003b0: 6469 6f55 726c 0a0a 0a61 7379 6e63 2064  dioUrl...async d
+000003c0: 6566 2064 6f77 6e6c 6f61 6442 4669 6c65  ef downloadBFile
+000003d0: 2875 726c 2c20 6675 6c6c 4669 6c65 4e61  (url, fullFileNa
+000003e0: 6d65 2c20 7072 6f67 7265 7373 4361 6c6c  me, progressCall
+000003f0: 6261 636b 293a 0a20 2020 2022 2222 0a20  back):.    """. 
+00000400: 2020 2020 2020 20e4 b88b e8bd bde8 a786         .........
+00000410: e9a2 91e6 9687 e4bb b6e5 928c e99f b3e9  ................
+00000420: a291 e696 87e4 bbb6 0a20 2020 203a 7061  .........    :pa
+00000430: 7261 6d20 7572 6c3a 0a20 2020 203a 7061  ram url:.    :pa
+00000440: 7261 6d20 6675 6c6c 4669 6c65 4e61 6d65  ram fullFileName
+00000450: 3a0a 2020 2020 3a70 6172 616d 2070 726f  :.    :param pro
+00000460: 6772 6573 7343 616c 6c62 6163 6b3a 0a20  gressCallback:. 
+00000470: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
+00000480: 2222 220a 2020 2020 6173 796e 6320 7769  """.    async wi
+00000490: 7468 2068 7474 7078 2e41 7379 6e63 436c  th httpx.AsyncCl
+000004a0: 6965 6e74 2829 2061 7320 636c 6965 6e74  ient() as client
+000004b0: 3a0a 2020 2020 2020 2020 6173 796e 6320  :.        async 
+000004c0: 7769 7468 2063 6c69 656e 742e 7374 7265  with client.stre
+000004d0: 616d 2822 4745 5422 2c20 7572 6c2c 2068  am("GET", url, h
+000004e0: 6561 6465 7273 3d68 6561 6465 7229 2061  eaders=header) a
+000004f0: 7320 7265 7370 3a0a 2020 2020 2020 2020  s resp:.        
+00000500: 2020 2020 6375 7272 656e 744c 656e 203d      currentLen =
+00000510: 2030 0a20 2020 2020 2020 2020 2020 2074   0.            t
+00000520: 6f74 616c 4c65 6e20 3d20 696e 7428 7265  otalLen = int(re
+00000530: 7370 2e68 6561 6465 7273 5b27 636f 6e74  sp.headers['cont
+00000540: 656e 742d 6c65 6e67 7468 275d 290a 2020  ent-length']).  
+00000550: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00000560: 746f 7461 6c4c 656e 290a 2020 2020 2020  totalLen).      
+00000570: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00000580: 6675 6c6c 4669 6c65 4e61 6d65 2c20 2277  fullFileName, "w
+00000590: 6222 2920 6173 2066 3a0a 2020 2020 2020  b") as f:.      
+000005a0: 2020 2020 2020 2020 2020 6173 796e 6320            async 
+000005b0: 666f 7220 6368 756e 6b20 696e 2072 6573  for chunk in res
+000005c0: 702e 6169 7465 725f 6279 7465 7328 293a  p.aiter_bytes():
+000005d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005e0: 2020 2020 2063 7572 7265 6e74 4c65 6e20       currentLen 
+000005f0: 2b3d 206c 656e 2863 6875 6e6b 290a 2020  += len(chunk).  
 00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2063 7572 7265 6e74 4c65 6e20 2b3d     currentLen +=
-00000620: 206c 656e 2863 6875 6e6b 290d 0a20 2020   len(chunk)..   
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2066 2e77 7269 7465 2863 6875 6e6b 290d   f.write(chunk).
-00000650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000660: 2020 2020 2070 726f 6772 6573 7343 616c       progressCal
-00000670: 6c62 6163 6b28 6375 7272 656e 744c 656e  lback(currentLen
-00000680: 202f 2074 6f74 616c 4c65 6e29 0d0a 0d0a   / totalLen)....
-00000690: 0d0a 6465 6620 6d65 7267 6546 696c 6554  ..def mergeFileT
-000006a0: 6f4d 7034 2876 4675 6c6c 4669 6c65 4e61  oMp4(vFullFileNa
-000006b0: 6d65 3a20 7374 722c 2061 4675 6c6c 4669  me: str, aFullFi
-000006c0: 6c65 4e61 6d65 3a20 7374 722c 206f 7574  leName: str, out
-000006d0: 7075 7446 696c 654e 616d 653a 2073 7472  putFileName: str
-000006e0: 2c20 7368 6f75 6c64 4465 6c65 7465 3d54  , shouldDelete=T
-000006f0: 7275 6529 3a0d 0a20 2020 2022 2222 0d0a  rue):..    """..
-00000700: 2020 2020 2020 2020 e590 88e5 b9b6 e8a7          ........
-00000710: 86e9 a291 e696 87e4 bbb6 e592 8ce9 9fb3  ................
-00000720: e9a2 91e6 9687 e4bb b60d 0a20 2020 203a  ...........    :
-00000730: 7061 7261 6d20 7646 756c 6c46 696c 654e  param vFullFileN
-00000740: 616d 653a 0d0a 2020 2020 3a70 6172 616d  ame:..    :param
-00000750: 2061 4675 6c6c 4669 6c65 4e61 6d65 3a0d   aFullFileName:.
-00000760: 0a20 2020 203a 7061 7261 6d20 6f75 7470  .    :param outp
-00000770: 7574 4669 6c65 4e61 6d65 3a0d 0a20 2020  utFileName:..   
-00000780: 203a 7061 7261 6d20 7368 6f75 6c64 4465   :param shouldDe
-00000790: 6c65 7465 3a0d 0a20 2020 203a 7265 7475  lete:..    :retu
-000007a0: 726e 3a0d 0a20 2020 2022 2222 0d0a 2020  rn:..    """..  
-000007b0: 2020 2320 e8b0 83e7 94a8 6666 6d70 6567    # ......ffmpeg
-000007c0: 0d0a 2020 2020 7375 6270 726f 6365 7373  ..    subprocess
-000007d0: 2e63 616c 6c28 6627 6666 6d70 6567 202d  .call(f'ffmpeg -
-000007e0: 7920 2d69 2022 7b76 4675 6c6c 4669 6c65  y -i "{vFullFile
-000007f0: 4e61 6d65 7d22 202d 6920 227b 6146 756c  Name}" -i "{aFul
-00000800: 6c46 696c 654e 616d 657d 2220 2d63 2063  lFileName}" -c c
-00000810: 6f70 7920 227b 6f75 7470 7574 4669 6c65  opy "{outputFile
-00000820: 4e61 6d65 7d22 272c 2073 6865 6c6c 3d54  Name}"', shell=T
-00000830: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00000840: 2020 2020 2020 2020 2020 7374 646f 7574            stdout
-00000850: 3d73 7562 7072 6f63 6573 732e 4445 564e  =subprocess.DEVN
-00000860: 554c 4c2c 0d0a 2020 2020 2020 2020 2020  ULL,..          
-00000870: 2020 2020 2020 2020 2020 7374 6465 7272            stderr
-00000880: 3d73 7562 7072 6f63 6573 732e 4445 564e  =subprocess.DEVN
-00000890: 554c 4c2c 0d0a 2020 2020 2020 2020 2020  ULL,..          
-000008a0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-000008b0: 2023 20e5 88a0 e999 a4e4 b8b4 e697 b6e6   # .............
-000008c0: 9687 e4bb b60d 0a20 2020 2069 6620 7368  .......    if sh
-000008d0: 6f75 6c64 4465 6c65 7465 3a0d 0a20 2020  ouldDelete:..   
-000008e0: 2020 2020 206f 732e 756e 6c69 6e6b 2876       os.unlink(v
-000008f0: 4675 6c6c 4669 6c65 4e61 6d65 290d 0a20  FullFileName).. 
-00000900: 2020 2020 2020 206f 732e 756e 6c69 6e6b         os.unlink
-00000910: 2861 4675 6c6c 4669 6c65 4e61 6d65 290d  (aFullFileName).
-00000920: 0a0d 0a64 6566 2067 6574 5f64 796e 616d  ...def get_dynam
-00000930: 6963 2864 796e 616d 6963 5f69 643a 2073  ic(dynamic_id: s
-00000940: 7472 293a 0d0a 2020 2020 2222 220d 0a20  tr):..    """.. 
-00000950: 2020 2020 2020 20e8 8eb7 e58f 96e5 9394         .........
-00000960: e593 a9e5 9394 e593 a9e5 8aa8 e680 810d  ................
-00000970: 0a20 2020 203a 7061 7261 6d20 6479 6e61  .    :param dyna
-00000980: 6d69 635f 6964 3a0d 0a20 2020 203a 7265  mic_id:..    :re
-00000990: 7475 726e 3a0d 0a20 2020 2022 2222 0d0a  turn:..    """..
-000009a0: 2020 2020 6479 6e61 6d69 635f 6170 6920      dynamic_api 
-000009b0: 3d20 6627 6874 7470 733a 2f2f 6170 692e  = f'https://api.
-000009c0: 7663 2e62 696c 6962 696c 692e 636f 6d2f  vc.bilibili.com/
-000009d0: 6479 6e61 6d69 635f 7376 722f 7631 2f64  dynamic_svr/v1/d
-000009e0: 796e 616d 6963 5f73 7672 2f67 6574 5f64  ynamic_svr/get_d
-000009f0: 796e 616d 6963 5f64 6574 6169 6c3f 6479  ynamic_detail?dy
-00000a00: 6e61 6d69 635f 6964 3d7b 6479 6e61 6d69  namic_id={dynami
-00000a10: 635f 6964 7d27 0d0a 2020 2020 7265 7370  c_id}'..    resp
-00000a20: 203d 2068 7474 7078 2e67 6574 2864 796e   = httpx.get(dyn
-00000a30: 616d 6963 5f61 7069 2c20 6865 6164 6572  amic_api, header
-00000a40: 733d 6865 6164 6572 290d 0a0d 0a20 2020  s=header)....   
-00000a50: 2064 796e 616d 6963 5f6a 736f 6e20 3d20   dynamic_json = 
-00000a60: 6a73 6f6e 2e6c 6f61 6473 2872 6573 702e  json.loads(resp.
-00000a70: 636f 6e74 656e 7429 5b27 6461 7461 275d  content)['data']
-00000a80: 5b27 6361 7264 275d 0d0a 2020 2020 6361  ['card']..    ca
-00000a90: 7264 203d 206a 736f 6e2e 6c6f 6164 7328  rd = json.loads(
-00000aa0: 6479 6e61 6d69 635f 6a73 6f6e 5b27 6361  dynamic_json['ca
-00000ab0: 7264 275d 290d 0a20 2020 2064 796e 616d  rd'])..    dynam
-00000ac0: 6963 5f6f 7269 6769 6e20 3d20 6361 7264  ic_origin = card
-00000ad0: 5b27 6974 656d 275d 0d0a 0d0a 2020 2020  ['item']....    
-00000ae0: 6479 6e61 6d69 635f 6465 7363 203d 2064  dynamic_desc = d
-00000af0: 796e 616d 6963 5f6f 7269 6769 6e5b 2764  ynamic_origin['d
-00000b00: 6573 6372 6970 7469 6f6e 275d 0d0a 2020  escription']..  
-00000b10: 2020 6479 6e61 6d69 635f 7372 6320 3d20    dynamic_src = 
-00000b20: 5b5d 0d0a 2020 2020 666f 7220 7069 6320  []..    for pic 
-00000b30: 696e 2064 796e 616d 6963 5f6f 7269 6769  in dynamic_origi
-00000b40: 6e5b 2770 6963 7475 7265 7327 5d3a 0d0a  n['pictures']:..
-00000b50: 2020 2020 2020 2020 6479 6e61 6d69 635f          dynamic_
-00000b60: 7372 632e 6170 7065 6e64 2864 6f77 6e6c  src.append(downl
-00000b70: 6f61 645f 696d 6728 7069 635b 2769 6d67  oad_img(pic['img
-00000b80: 5f73 7263 275d 2929 0d0a 0d0a 2020 2020  _src']))....    
-00000b90: 7265 7475 726e 2064 796e 616d 6963 5f64  return dynamic_d
-00000ba0: 6573 632c 2064 796e 616d 6963 5f73 7263  esc, dynamic_src
+00000610: 2020 662e 7772 6974 6528 6368 756e 6b29    f.write(chunk)
+00000620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000630: 2020 2020 2070 726f 6772 6573 7343 616c       progressCal
+00000640: 6c62 6163 6b28 6375 7272 656e 744c 656e  lback(currentLen
+00000650: 202f 2074 6f74 616c 4c65 6e29 0a0a 0a64   / totalLen)...d
+00000660: 6566 206d 6572 6765 4669 6c65 546f 4d70  ef mergeFileToMp
+00000670: 3428 7646 756c 6c46 696c 654e 616d 653a  4(vFullFileName:
+00000680: 2073 7472 2c20 6146 756c 6c46 696c 654e   str, aFullFileN
+00000690: 616d 653a 2073 7472 2c20 6f75 7470 7574  ame: str, output
+000006a0: 4669 6c65 4e61 6d65 3a20 7374 722c 2073  FileName: str, s
+000006b0: 686f 756c 6444 656c 6574 653d 5472 7565  houldDelete=True
+000006c0: 293a 0a20 2020 2022 2222 0a20 2020 2020  ):.    """.     
+000006d0: 2020 20e5 9088 e5b9 b6e8 a786 e9a2 91e6     .............
+000006e0: 9687 e4bb b6e5 928c e99f b3e9 a291 e696  ................
+000006f0: 87e4 bbb6 0a20 2020 203a 7061 7261 6d20  .....    :param 
+00000700: 7646 756c 6c46 696c 654e 616d 653a 0a20  vFullFileName:. 
+00000710: 2020 203a 7061 7261 6d20 6146 756c 6c46     :param aFullF
+00000720: 696c 654e 616d 653a 0a20 2020 203a 7061  ileName:.    :pa
+00000730: 7261 6d20 6f75 7470 7574 4669 6c65 4e61  ram outputFileNa
+00000740: 6d65 3a0a 2020 2020 3a70 6172 616d 2073  me:.    :param s
+00000750: 686f 756c 6444 656c 6574 653a 0a20 2020  houldDelete:.   
+00000760: 203a 7265 7475 726e 3a0a 2020 2020 2222   :return:.    ""
+00000770: 220a 2020 2020 2320 e8b0 83e7 94a8 6666  ".    # ......ff
+00000780: 6d70 6567 0a20 2020 2073 7562 7072 6f63  mpeg.    subproc
+00000790: 6573 732e 6361 6c6c 2866 2766 666d 7065  ess.call(f'ffmpe
+000007a0: 6720 2d79 202d 6920 227b 7646 756c 6c46  g -y -i "{vFullF
+000007b0: 696c 654e 616d 657d 2220 2d69 2022 7b61  ileName}" -i "{a
+000007c0: 4675 6c6c 4669 6c65 4e61 6d65 7d22 202d  FullFileName}" -
+000007d0: 6320 636f 7079 2022 7b6f 7574 7075 7446  c copy "{outputF
+000007e0: 696c 654e 616d 657d 2227 2c20 7368 656c  ileName}"', shel
+000007f0: 6c3d 5472 7565 2c0a 2020 2020 2020 2020  l=True,.        
+00000800: 2020 2020 2020 2020 2020 2020 7374 646f              stdo
+00000810: 7574 3d73 7562 7072 6f63 6573 732e 4445  ut=subprocess.DE
+00000820: 564e 554c 4c2c 0a20 2020 2020 2020 2020  VNULL,.         
+00000830: 2020 2020 2020 2020 2020 2073 7464 6572             stder
+00000840: 723d 7375 6270 726f 6365 7373 2e44 4556  r=subprocess.DEV
+00000850: 4e55 4c4c 2c0a 2020 2020 2020 2020 2020  NULL,.          
+00000860: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00000870: 2320 e588 a0e9 99a4 e4b8 b4e6 97b6 e696  # ..............
+00000880: 87e4 bbb6 0a20 2020 2069 6620 7368 6f75  .....    if shou
+00000890: 6c64 4465 6c65 7465 3a0a 2020 2020 2020  ldDelete:.      
+000008a0: 2020 6f73 2e75 6e6c 696e 6b28 7646 756c    os.unlink(vFul
+000008b0: 6c46 696c 654e 616d 6529 0a20 2020 2020  lFileName).     
+000008c0: 2020 206f 732e 756e 6c69 6e6b 2861 4675     os.unlink(aFu
+000008d0: 6c6c 4669 6c65 4e61 6d65 290a 0a64 6566  llFileName)..def
+000008e0: 2067 6574 5f64 796e 616d 6963 2864 796e   get_dynamic(dyn
+000008f0: 616d 6963 5f69 643a 2073 7472 293a 0a20  amic_id: str):. 
+00000900: 2020 2022 2222 0a20 2020 2020 2020 20e8     """.        .
+00000910: 8eb7 e58f 96e5 9394 e593 a9e5 9394 e593  ................
+00000920: a9e5 8aa8 e680 810a 2020 2020 3a70 6172  ........    :par
+00000930: 616d 2064 796e 616d 6963 5f69 643a 0a20  am dynamic_id:. 
+00000940: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
+00000950: 2222 220a 2020 2020 6479 6e61 6d69 635f  """.    dynamic_
+00000960: 6170 6920 3d20 6627 6874 7470 733a 2f2f  api = f'https://
+00000970: 6170 692e 7663 2e62 696c 6962 696c 692e  api.vc.bilibili.
+00000980: 636f 6d2f 6479 6e61 6d69 635f 7376 722f  com/dynamic_svr/
+00000990: 7631 2f64 796e 616d 6963 5f73 7672 2f67  v1/dynamic_svr/g
+000009a0: 6574 5f64 796e 616d 6963 5f64 6574 6169  et_dynamic_detai
+000009b0: 6c3f 6479 6e61 6d69 635f 6964 3d7b 6479  l?dynamic_id={dy
+000009c0: 6e61 6d69 635f 6964 7d27 0a20 2020 2072  namic_id}'.    r
+000009d0: 6573 7020 3d20 6874 7470 782e 6765 7428  esp = httpx.get(
+000009e0: 6479 6e61 6d69 635f 6170 692c 2068 6561  dynamic_api, hea
+000009f0: 6465 7273 3d68 6561 6465 7229 0a0a 2020  ders=header)..  
+00000a00: 2020 6479 6e61 6d69 635f 6a73 6f6e 203d    dynamic_json =
+00000a10: 206a 736f 6e2e 6c6f 6164 7328 7265 7370   json.loads(resp
+00000a20: 2e63 6f6e 7465 6e74 295b 2764 6174 6127  .content)['data'
+00000a30: 5d5b 2763 6172 6427 5d0a 2020 2020 6361  ]['card'].    ca
+00000a40: 7264 203d 206a 736f 6e2e 6c6f 6164 7328  rd = json.loads(
+00000a50: 6479 6e61 6d69 635f 6a73 6f6e 5b27 6361  dynamic_json['ca
+00000a60: 7264 275d 290a 2020 2020 6479 6e61 6d69  rd']).    dynami
+00000a70: 635f 6f72 6967 696e 203d 2063 6172 645b  c_origin = card[
+00000a80: 2769 7465 6d27 5d0a 0a20 2020 2064 796e  'item']..    dyn
+00000a90: 616d 6963 5f64 6573 6320 3d20 6479 6e61  amic_desc = dyna
+00000aa0: 6d69 635f 6f72 6967 696e 5b27 6465 7363  mic_origin['desc
+00000ab0: 7269 7074 696f 6e27 5d0a 2020 2020 6479  ription'].    dy
+00000ac0: 6e61 6d69 635f 7372 6320 3d20 5b5d 0a20  namic_src = []. 
+00000ad0: 2020 2066 6f72 2070 6963 2069 6e20 6479     for pic in dy
+00000ae0: 6e61 6d69 635f 6f72 6967 696e 5b27 7069  namic_origin['pi
+00000af0: 6374 7572 6573 275d 3a0a 2020 2020 2020  ctures']:.      
+00000b00: 2020 6479 6e61 6d69 635f 7372 632e 6170    dynamic_src.ap
+00000b10: 7065 6e64 2864 6f77 6e6c 6f61 645f 696d  pend(download_im
+00000b20: 6728 7069 635b 2769 6d67 5f73 7263 275d  g(pic['img_src']
+00000b30: 2929 0a0a 2020 2020 7265 7475 726e 2064  ))..    return d
+00000b40: 796e 616d 6963 5f64 6573 632c 2064 796e  ynamic_desc, dyn
+00000b50: 616d 6963 5f73 7263                      amic_src
```

### Comparing `nonebot_plugin_resolver-1.0.9/nonebot-plugin-resolver/common_utils.py` & `nonebot_plugin_resolver-1.1.0/nonebot-plugin-resolver/common_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,81 @@
-import aiohttp
-import httpx
-import random
-import os
-import re
-
-# twitter 代理地址
-proxies = {
-    'http': 'http://127.0.0.1:7890',
-    'https': 'http://127.0.0.1:7890'
-}
-
-# httpx 代理地址格式
-httpx_proxies = {
-    "http://": "http://127.0.0.1:7890",
-    "https://": "http://127.0.0.1:7890",
-}
-header = {
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.64 Safari/537.36'}
-
-
-async def download_video_random(url):
-    """
-        异步下载视频
-    :param url:
-    :return:
-    """
-    # 获取文件名
-    path = os.getcwd() + "/" + f"{str(random.randint(1, 100))}.mp4"
-    # 下载文件
-    async with httpx.AsyncClient(proxies=httpx_proxies) as client2:
-        async with client2.stream("GET", url, headers=header) as resp:
-            with open(path, "wb") as f:
-                async for chunk in resp.aiter_bytes():
-                    f.write(chunk)
-    return path
-
-async def download_video_with_proxy(url):
-    """
-        异步下载视频
-    :param url:
-    :return:
-    """
-    # 获取文件名
-    path = os.getcwd() + "/" + f"{str(random.randint(1, 100))}.mp4"
-    # 下载文件
-    async with httpx.AsyncClient(proxies=httpx_proxies) as client2:
-        async with client2.stream("GET", url, headers=header) as resp:
-            with open(path, "wb") as f:
-                async for chunk in resp.aiter_bytes():
-                    f.write(chunk)
-    return path
-
-async def download_img(url: str, path='') -> str:
-    """
-        异步下载网络图片（eg. https://pbs.twimg.com/media/FoQVwyxacAEIRdS.jpg）
-    :param path:
-    :param url:
-    :return:
-    """
-    if path == '':
-        path = os.getcwd() + "/" + url.split('/').pop()
-    # print(path)
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url) as response:
-            if response.status == 200:
-                data = await response.read()
-                with open(path, 'wb') as f:
-                    f.write(data)
-    return path
-
-async def download_img_with_proxy(url: str) -> str:
-    """
-        异步下载网络图片（eg. https://pbs.twimg.com/media/FoQVwyxacAEIRdS.jpg）
-    :param url:
-    :return:
-    """
-    path = os.getcwd() + "/" + url.split('/').pop()
-    # print(path)
-    async with aiohttp.ClientSession() as session:
-        async with session.get(url, proxy=proxies.get("http")) as response:
-            if response.status == 200:
-                data = await response.read()
-                with open(path, 'wb') as f:
-                    f.write(data)
-    return path
-
-def delete_boring_characters(sentence):
-    """
-        去除标题的特殊字符
-    :param sentence:
-    :return:
-    """
-    return re.sub('[0-9’!"∀〃#$%&\'()*+,-./:;<=>?@，。?★、…【】《》？“”‘’！[\\]^_`{|}~～\s]+', "", sentence)
+import aiohttp
+import httpx
+import os
+import re
+import time
+
+header = {
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (HTML, like Gecko) Chrome/101.0.4951.64 Safari/537.36'
+}
+
+async def download_video(url, proxy: str = None):
+    """
+    异步下载（httpx）视频，并支持通过代理下载。
+    文件名将使用时间戳生成，以确保唯一性。
+    如果提供了代理地址，则会通过该代理下载视频。
+
+    :param url: 要下载的视频的URL。
+    :param proxy: 可选，下载视频时使用的代理服务器的URL。
+    :return: 保存视频的路径。
+    """
+    # 使用时间戳生成文件名，确保唯一性
+    path = os.path.join(os.getcwd(), f"{int(time.time())}.mp4")
+
+    # 配置代理
+    client_config = {
+        'headers': header,
+        'timeout': httpx.Timeout(60, connect=5.0),
+        'follow_redirects': True
+    }
+    if proxy:
+        client_config['proxies'] = {'https': proxy}
+    # 下载文件
+    try:
+        async with httpx.AsyncClient(**client_config) as client:
+            async with client.stream("GET", url) as resp:
+                with open(path, "wb") as f:
+                    async for chunk in resp.aiter_bytes():
+                        f.write(chunk)
+        return path
+    except Exception as e:
+        print(f"下载视频错误原因是: {e}")
+        return None
+
+
+async def download_img(url: str, path: str = '', proxy: str = None, session = None) -> str:
+    """
+    异步下载（aiohttp）网络图片，并支持通过代理下载。
+    如果未指定path，则图片将保存在当前工作目录并以图片的文件名命名。
+    如果提供了代理地址，则会通过该代理下载图片。
+
+    :param url: 要下载的图片的URL。
+    :param path: 图片保存的路径。如果为空，则保存在当前目录。
+    :param proxy: 可选，下载图片时使用的代理服务器的URL。
+    :return: 保存图片的路径。
+    """
+    if path == '':
+        path = os.path.join(os.getcwd(), url.split('/').pop())
+    # 单个文件下载
+    if session is None:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, proxy=proxy) as response:
+                if response.status == 200:
+                    data = await response.read()
+                    with open(path, 'wb') as f:
+                        f.write(data)
+    #多个文件异步下载
+    else:
+        async with session.get(url, proxy=proxy) as response:
+            if response.status == 200:
+                data = await response.read()
+                with open(path, 'wb') as f:
+                    f.write(data)
+    return path
+
+def delete_boring_characters(sentence):
+    """
+        去除标题的特殊字符
+    :param sentence:
+    :return:
+    """
+    return re.sub('[0-9’!"∀〃#$%&\'()*+,-./:;<=>?@，。?★、…【】《》？“”‘’！[\\]^_`{|}~～\s]+', "", sentence)
```

