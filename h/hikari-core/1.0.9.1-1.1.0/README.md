# Comparing `tmp/hikari_core-1.0.9.1.tar.gz` & `tmp/hikari_core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-1.0.9.1.tar", max compression
+gzip compressed data, was "hikari_core-1.1.0.tar", max compression
```

## Comparing `hikari_core-1.0.9.1.tar` & `hikari_core-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     6011 2023-12-11 09:55:07.182805 hikari_core-1.0.9.1/hikari_core/__init__.py
--rw-r--r--   0        0        0    15655 2023-12-04 07:09:19.887174 hikari_core-1.0.9.1/hikari_core/analyze.py
--rw-r--r--   0        0        0     4836 2023-11-17 01:23:59.310345 hikari_core-1.0.9.1/hikari_core/command_select.py
--rw-r--r--   0        0        0     2161 2023-09-27 17:02:55.628020 hikari_core-1.0.9.1/hikari_core/config.py
--rw-r--r--   0        0        0    10676 2023-12-11 09:54:46.858604 hikari_core-1.0.9.1/hikari_core/data_source.py
--rw-r--r--   0        0        0        0 2023-08-29 06:12:41.281706 hikari_core-1.0.9.1/hikari_core/game/__init__.py
--rw-r--r--   0        0        0     2666 2023-12-06 03:10:08.217057 hikari_core-1.0.9.1/hikari_core/game/ban_search.py
--rw-r--r--   0        0        0     2389 2023-11-23 02:37:23.103917 hikari_core-1.0.9.1/hikari_core/game/box_check.py
--rw-r--r--   0        0        0     4864 2023-09-13 11:34:44.172882 hikari_core-1.0.9.1/hikari_core/game/help.py
--rw-r--r--   0        0        0     2179 2023-12-06 03:11:46.160777 hikari_core-1.0.9.1/hikari_core/game/roll.py
--rw-r--r--   0        0        0     2373 2023-11-23 02:36:52.379029 hikari_core-1.0.9.1/hikari_core/game/sx.py
--rw-r--r--   0        0        0      718 2023-08-29 06:12:41.223598 hikari_core-1.0.9.1/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2883 2023-08-29 06:12:41.225606 hikari_core-1.0.9.1/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5512 2023-08-29 06:12:41.228103 hikari_core-1.0.9.1/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-1.0.9.1/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-1.0.9.1/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-1.0.9.1/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-1.0.9.1/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-1.0.9.1/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     2727 2023-09-27 17:03:18.369031 hikari_core-1.0.9.1/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3239 2023-11-15 06:18:43.431831 hikari_core-1.0.9.1/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-1.0.9.1/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    11620 2023-12-11 09:53:07.575401 hikari_core-1.0.9.1/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0    10875 2023-09-18 10:54:10.026096 hikari_core-1.0.9.1/hikari_core/moudle/wws_bind.py
--rw-r--r--   0        0        0     3594 2023-09-18 10:54:22.458985 hikari_core-1.0.9.1/hikari_core/moudle/wws_clan.py
--rw-r--r--   0        0        0     3594 2023-11-07 07:26:52.281761 hikari_core-1.0.9.1/hikari_core/moudle/wws_clanrank.py
--rw-r--r--   0        0        0     2145 2023-11-15 06:51:40.263671 hikari_core-1.0.9.1/hikari_core/moudle/wws_cwrank.py
--rw-r--r--   0        0        0     2785 2023-09-18 13:01:49.848254 hikari_core-1.0.9.1/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0    13233 2023-12-06 12:23:01.385892 hikari_core-1.0.9.1/hikari_core/moudle/wws_real_game.py
--rw-r--r--   0        0        0     3575 2023-09-13 11:32:44.941040 hikari_core-1.0.9.1/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     2864 2023-09-27 18:54:06.479199 hikari_core-1.0.9.1/hikari_core/moudle/wws_recents.py
--rw-r--r--   0        0        0     4144 2023-09-18 10:54:47.099498 hikari_core-1.0.9.1/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     4133 2023-09-13 11:33:27.902012 hikari_core-1.0.9.1/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0     6718 2023-11-21 17:09:11.181217 hikari_core-1.0.9.1/hikari_core/moudle/wws_shiprank.py
--rw-r--r--   0        0        0     4462 2023-12-06 21:14:42.095272 hikari_core-1.0.9.1/hikari_core/Template/bind-list.html
--rw-r--r--   0        0        0     4740 2023-12-06 21:14:42.488647 hikari_core-1.0.9.1/hikari_core/Template/cw-rank.html
--rw-r--r--   0        0        0     2578 2023-12-06 21:14:42.297228 hikari_core-1.0.9.1/hikari_core/Template/select-clan.html
--rw-r--r--   0        0        0     3783 2023-12-06 21:14:42.284574 hikari_core-1.0.9.1/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5117 2023-12-06 21:14:42.311880 hikari_core-1.0.9.1/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      449 2023-12-06 21:14:42.324485 hikari_core-1.0.9.1/hikari_core/Template/text.html
--rw-r--r--   0        0        0     7262 2023-12-06 21:14:42.337147 hikari_core-1.0.9.1/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16729 2023-12-06 21:14:42.352805 hikari_core-1.0.9.1/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    26850 2023-12-06 21:14:42.365443 hikari_core-1.0.9.1/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    28107 2023-12-06 21:14:42.379050 hikari_core-1.0.9.1/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    23257 2023-12-06 21:14:42.393803 hikari_core-1.0.9.1/hikari_core/Template/wws-info-recents.html
--rw-r--r--   0        0        0    28033 2023-12-06 21:14:42.407443 hikari_core-1.0.9.1/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-12-06 21:14:42.420111 hikari_core-1.0.9.1/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    23774 2023-12-06 21:14:42.432753 hikari_core-1.0.9.1/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    21391 2023-12-06 21:14:42.446447 hikari_core-1.0.9.1/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0    13500 2023-12-09 09:18:28.754570 hikari_core-1.0.9.1/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5762 2023-12-06 21:14:42.475960 hikari_core-1.0.9.1/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4391 2023-08-29 06:12:41.339798 hikari_core-1.0.9.1/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-1.0.9.1/LICENSE
--rw-r--r--   0        0        0     1572 2023-12-11 09:54:50.101000 hikari_core-1.0.9.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-1.0.9.1/README.md
--rw-r--r--   0        0        0    14234 1970-01-01 00:00:00.000000 hikari_core-1.0.9.1/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-1.0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     6011 2023-12-14 16:55:34.466822 hikari_core-1.1.0/hikari_core/__init__.py
+-rw-r--r--   0        0        0    15655 2023-12-14 16:55:34.475881 hikari_core-1.1.0/hikari_core/analyze.py
+-rw-r--r--   0        0        0     4836 2023-12-14 16:55:34.478434 hikari_core-1.1.0/hikari_core/command_select.py
+-rw-r--r--   0        0        0     2161 2023-12-14 16:55:34.496097 hikari_core-1.1.0/hikari_core/config.py
+-rw-r--r--   0        0        0    10674 2024-06-02 08:46:08.588597 hikari_core-1.1.0/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-08-29 06:12:41.281706 hikari_core-1.1.0/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2666 2023-12-14 16:55:34.502222 hikari_core-1.1.0/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2389 2023-12-14 16:55:34.513881 hikari_core-1.1.0/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     4864 2023-12-14 16:55:34.515891 hikari_core-1.1.0/hikari_core/game/help.py
+-rw-r--r--   0        0        0     2179 2023-12-14 16:55:34.516895 hikari_core-1.1.0/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2373 2023-12-14 16:55:34.528552 hikari_core-1.1.0/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-08-29 06:12:41.223598 hikari_core-1.1.0/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-08-29 06:12:41.225606 hikari_core-1.1.0/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-08-29 06:12:41.228103 hikari_core-1.1.0/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-1.1.0/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-1.1.0/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-1.1.0/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-1.1.0/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-1.1.0/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2727 2023-12-14 16:55:34.443597 hikari_core-1.1.0/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3239 2023-12-14 16:55:34.543154 hikari_core-1.1.0/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-1.1.0/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11620 2023-12-14 16:55:34.545163 hikari_core-1.1.0/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10875 2023-12-14 16:55:34.557843 hikari_core-1.1.0/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     3594 2023-12-14 16:55:34.559850 hikari_core-1.1.0/hikari_core/moudle/wws_clan.py
+-rw-r--r--   0        0        0     3594 2023-12-14 16:55:34.588142 hikari_core-1.1.0/hikari_core/moudle/wws_clanrank.py
+-rw-r--r--   0        0        0     2145 2023-12-14 16:55:34.609912 hikari_core-1.1.0/hikari_core/moudle/wws_cwrank.py
+-rw-r--r--   0        0        0     2785 2023-12-14 16:55:34.627076 hikari_core-1.1.0/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0    13233 2023-12-14 16:55:34.629121 hikari_core-1.1.0/hikari_core/moudle/wws_real_game.py
+-rw-r--r--   0        0        0     3575 2023-12-14 16:55:34.632135 hikari_core-1.1.0/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     2864 2023-12-14 16:55:34.635153 hikari_core-1.1.0/hikari_core/moudle/wws_recents.py
+-rw-r--r--   0        0        0     4144 2023-12-14 16:55:34.638186 hikari_core-1.1.0/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     4142 2024-06-02 08:45:19.963029 hikari_core-1.1.0/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6718 2023-12-14 16:55:34.641718 hikari_core-1.1.0/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2024-05-20 11:39:49.254574 hikari_core-1.1.0/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     4740 2024-05-20 11:39:50.125799 hikari_core-1.1.0/hikari_core/Template/cw-rank.html
+-rw-r--r--   0        0        0     2578 2024-05-20 11:39:49.557086 hikari_core-1.1.0/hikari_core/Template/select-clan.html
+-rw-r--r--   0        0        0     3783 2024-05-20 11:39:49.516905 hikari_core-1.1.0/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5117 2024-05-20 11:39:49.592066 hikari_core-1.1.0/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2024-05-20 11:39:49.607736 hikari_core-1.1.0/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7262 2024-05-20 11:39:49.635490 hikari_core-1.1.0/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16729 2024-05-20 11:39:49.663869 hikari_core-1.1.0/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    26850 2024-05-20 11:39:49.700834 hikari_core-1.1.0/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28057 2024-05-20 11:39:49.739375 hikari_core-1.1.0/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    23257 2024-05-20 11:39:49.774780 hikari_core-1.1.0/hikari_core/Template/wws-info-recents.html
+-rw-r--r--   0        0        0    28099 2024-05-20 11:39:49.810941 hikari_core-1.1.0/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2024-05-20 11:39:49.861171 hikari_core-1.1.0/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    28315 2024-06-02 08:45:19.962013 hikari_core-1.1.0/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21516 2024-05-20 11:39:49.993917 hikari_core-1.1.0/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0    13500 2024-05-20 11:39:50.047212 hikari_core-1.1.0/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5762 2024-05-20 11:39:50.078181 hikari_core-1.1.0/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4391 2023-08-29 06:12:41.339798 hikari_core-1.1.0/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1570 2024-06-02 08:45:42.868681 hikari_core-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-1.1.0/README.md
+-rw-r--r--   0        0        0    14232 1970-01-01 00:00:00.000000 hikari_core-1.1.0/setup.py
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 hikari_core-1.1.0/PKG-INFO
```

### Comparing `hikari_core-1.0.9.1/hikari_core/__init__.py` & `hikari_core-1.1.0/hikari_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/analyze.py` & `hikari_core-1.1.0/hikari_core/analyze.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/command_select.py` & `hikari_core-1.1.0/hikari_core/command_select.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/config.py` & `hikari_core-1.1.0/hikari_core/config.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/data_source.py` & `hikari_core-1.1.0/hikari_core/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import traceback
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Tuple
 
 dir_path = Path(__file__).parent
 template_path = dir_path / 'Template'
-__version__ = '1.0.9.1'
+__version__ = '1.1.0'
 
 
 @dataclass
 class matching:
     keywords: Tuple[str, ...]
     match_keywords: str
```

### Comparing `hikari_core-1.0.9.1/hikari_core/game/ban_search.py` & `hikari_core-1.1.0/hikari_core/game/ban_search.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/game/box_check.py` & `hikari_core-1.1.0/hikari_core/game/box_check.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/game/help.py` & `hikari_core-1.1.0/hikari_core/game/help.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/game/roll.py` & `hikari_core-1.1.0/hikari_core/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/game/sx.py` & `hikari_core-1.1.0/hikari_core/game/sx.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Html_Render/__init__.py` & `hikari_core-1.1.0/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Html_Render/browser.py` & `hikari_core-1.1.0/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Html_Render/data_source.py` & `hikari_core-1.1.0/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-1.1.0/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-1.1.0/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-1.1.0/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/HttpClient_Pool.py` & `hikari_core-1.1.0/hikari_core/HttpClient_Pool.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/model.py` & `hikari_core-1.1.0/hikari_core/model.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/publicAPI.py` & `hikari_core-1.1.0/hikari_core/moudle/publicAPI.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_bind.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_bind.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_clan.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_clan.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_clanrank.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_clanrank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_cwrank.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_cwrank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_info.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_real_game.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_real_game.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_recent.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_recents.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_recents.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_ship_info.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_ship_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_ship_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,29 @@
         else:
             is_cache = await check_yuyuko_cache(hikari.Input.Platform, hikari.Input.PlatformId)
         if is_cache:
             logger.success('上报数据成功')
         else:
             logger.success('跳过上报数据，直接请求')
 
-        url = 'https://recent.wows.shinoaki.com:8890/api/wows/recent/day/info'
+        url = 'https://recent.wows.shinoaki.com:8890/api/wows/recent/day/list/info'
         if hikari.Input.Search_Type == 3:
             params = {
                 'server': hikari.Input.Server,
                 'accountId': hikari.Input.AccountId,
                 'dateTime': hikari.Input.Recent_Date,
-                'day': hikari.Input.Recent_Day,
+                # 'day': hikari.Input.Recent_Day,
                 'shipId': hikari.Input.ShipInfo.Ship_Id,
             }
         else:
             params = {
                 'server': hikari.Input.Platform,
                 'accountId': hikari.Input.PlatformId,
                 'dateTime': hikari.Input.Recent_Date,
-                'day': hikari.Input.Recent_Day,
+                # 'day': hikari.Input.Recent_Day,
                 'shipId': hikari.Input.ShipInfo.Ship_Id,
             }
 
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
```

### Comparing `hikari_core-1.0.9.1/hikari_core/moudle/wws_shiprank.py` & `hikari_core-1.1.0/hikari_core/moudle/wws_shiprank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/bind-list.html` & `hikari_core-1.1.0/hikari_core/Template/bind-list.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/cw-rank.html` & `hikari_core-1.1.0/hikari_core/Template/cw-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/select-clan.html` & `hikari_core-1.1.0/hikari_core/Template/select-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/select-ship.html` & `hikari_core-1.1.0/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/ship-rank.html` & `hikari_core-1.1.0/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-ban.html` & `hikari_core-1.1.0/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-box-christmas.html` & `hikari_core-1.1.0/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-clan.html` & `hikari_core-1.1.0/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-info-recent.html` & `hikari_core-1.1.0/hikari_core/Template/wws-info-recent.html`

 * *Files 10% similar despite different names*

```diff
@@ -5,399 +5,399 @@
 		<title></title>
 	</head>
 	<style>
 		* {
 			padding: 0;
 			margin: 0;
 		}
-		
+
 		.flex-2 {
 			flex: 2;
 		}
-		
+
 		.flex-3 {
 			flex: 3;
 		}
-		
+
 		.flex-4 {
 			flex: 4;
 		}
-		
+
 		.flex-8 {
 			flex: 8;
 		}
-		
+
 		.flex-10 {
 			flex: 10;
 		}
-		
+
 		.main-content {
 			width: 1500px;
 			font-size: 30px;
 			font-family: "Microsoft YaHei";
 			font-weight: bold;
 		}
-		
+
 		.page-box {
 			width: 1500px;
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.page-header {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.clan-user-server {
 			height: 120px;
 			text-align: center;
 			font-size: 45px;
 			line-height: 120px;
 		}
-		
+
 		.clan {
 			display: inline-block;
 			padding-right: 10px;
 			height: 120px;
 		}
-		
+
 		.user {
 			display: inline-block;
 			height: 120px;
 		}
-		
+
 		.server {
 			display: inline-block;
 			padding-left: 10px;
 		}
-		
+
 		.server-border {
 			width: 200px;
 			height: 50px;
 			line-height: 50px;
 			text-align: center;
 			background-color: #F2F2F2;
 			border-radius: 25px;
 			font-size: 35px;
 		}
-		
+
 		.pr {
 			display: flex;
 			height: 120px;
 			font-weight: bold;
 			line-height: 60px;
 			padding: 0 100px;
 		}
-		
+
 		.pr-bar-bg {
 			position: relative;
 			flex: 1;
 			line-height: 80px;
 			background-color: #A6A6A6;
 			height: 80px;
 			border-radius: 40px;
 			margin-top: 10px;
 			text-align: center;
 			color: #FFFFFF;
 		}
-		
+
 		.pr-bar {
 			position: absolute;
 			top: 0;
 			left: 0;
 			height: 80px;
 			z-index: 1;
 			border-radius: 40px;
 		}
-		
+
 		.pr-number {
 			z-index: 99;
 			position: absolute;
 			left: 0px;
 			right: 0px;
 			font-size: 35px;
 			font-weight: bold;
 		}
-		
+
 		.recnet-time {
 			text-align: center;
 			font-weight: normal;
 		}
-		
+
 		.overview-change {
 			display: flex;
 			margin-top: 30px;
 			padding: 0 80px;
 			height: 450px;
 		}
-		
+
 		.overview-change-item {
 			flex: 1;
 			display: flex;
 			flex-direction: column;
 			margin: 0 20px;
-		
+
 		}
-		
+
 		.item-top {
 			flex: 5;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.item-bottom {
 			display: flex;
 			flex: 4;
 			margin-top: 20px;
 		}
-		
-		
+
+
 		.bottom-mini-item-left {
 			flex: 1;
 			margin-right: 10px;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.bottom-mini-item-right {
 			flex: 1;
 			margin-left: 10px;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.item-top {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.item-top div {
 			height: 120px;
 			text-align: center;
 			font-size: 60px;
 		}
-		
+
 		.item-top-top {
 			color: #606266;
 			font-weight: normal;
 			line-height: 150px;
 		}
-		
+
 		.item-top-bottom {
 			line-height: 90px;
 		}
-		
-		
+
+
 		.change-pr-title {
 			color: #606266;
 			height: 95px;
 			display: flex;
 			font-weight: normal;
 			line-height: 125px;
 		}
-		
+
 		.change-pr {
 			height: 95px;
 			line-height: 75px;
 			text-align: center;
 			font-size: 45px;
 		}
-		
+
 		.change-pr-title-left {
 			flex: 1;
 			font-size: 50px;
 			text-align: right;
 			margin-right: 20px;
 		}
-		
+
 		.change-pr-title-right {
 			flex: 1;
 		}
-		
+
 		.bottom-mini-item-left,
 		.bottom-mini-item-right {
 			display: flex;
 			flex-direction: column;
 		}
-		
+
 		.mini-item-top {
 			color: #606266;
 			font-weight: normal;
 			line-height: 135px;
 		}
-		
+
 		.mini-item-bottom {
 			line-height: 45px;
 		}
-		
+
 		.bottom-mini-item-left div,
 		.bottom-mini-item-right div {
 			height: 95px;
 			text-align: center;
 			font-size: 35px;
 		}
-		
+
 		.information-header {
 			margin: 0 400px;
 			margin-top: 30px;
 			height: 60px;
 			line-height: 60px;
 			border-radius: 16px;
 			background-color: #D9D9D9;
 			text-align: center;
 		}
-		
+
 		.information-body {
 			margin: 0 100px;
 			margin-top: 30px;
 			display: flex;
 			flex-direction: column;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.information-col {
 			height: 60px;
 			display: flex;
 			line-height: 60px;
 		}
-		
+
 		.information-col-item {
 			flex: 1;
 			text-align: center;
 		}
-		
+
 		.information-table-header {
 			color: #606266;
 		}
-		
+
 		.information-type {
 			color: #909399;
 		}
-		
+
 		.random-header {
 			margin: 0 400px;
 			margin-top: 30px;
 			height: 60px;
 			line-height: 60px;
 			border-radius: 16px;
 			background-color: #D9D9D9;
 			text-align: center;
 		}
-		
+
 		.random-data {
 			display: flex;
 			flex-direction: column;
 			margin: 0 100px;
 			margin-top: 30px;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 		}
-		
+
 		.random-data-col {
 			display: flex;
 			height: 90px;
 		}
-		
+
 		.random-col-item {
 			line-height: 90px;
 			text-align: center;
 		}
-		
+
 		.random-table-header {
 			color: #606266;
 			height: 60px;
 			display: flex;
 		}
-		
+
 		.random-table-header .random-col-item {
 			line-height: 60px;
 		}
-		
+
 		.footer {
 			margin-top: 30px;
 			text-align: center;
 			font-weight: bold;
 			font-size: 24px;
 			color: #909399;
 			margin-bottom: 20px;
 		}
-		
+
 		.rank-data-col {
 			display: flex;
 			height: 90px;
 		}
 
 		.frag-data {
 			display: flex;
 			margin: 30px 90px;
 		}
-		
+
 		.frag-data-col {
 			display: flex;
 			flex: 1;
 			margin-bottom: 20px;
 		}
 		.frag-item {
 			flex: 1;
 			text-align: center;
 			background-color: #F2F2F2;
 			border-radius: 16px;
 			margin: 0 10px;
         }
-		
+
 		.frag-key,.frag-value {
 			height: 100px;
 			font-size: 35px;
 		}
-		
+
 		.frag-key {
 			color: #606266;
 			font-weight: normal;
 			line-height: 120px;
 		}
 		.frag-value {
 			line-height: 80px;
 		}
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
-				
+
 				<div class="page-header">
 					<div class="clan-user-server">
 						{% if data['userInfo']['clanInfo']['tag'] %}
 						<div class="clan" style="color: {{ data['userInfo']['clanInfo']['color'] }};">[{{ data['userInfo']['clanInfo']['tag'] }}]</div>
 						{% endif %}
 						<div class="user">{{ data['userInfo']['userName'] }}</div>
 						<div class="server">
 							<div class="server-border">
 								{{ data['userInfo']['serverCn'] }}
 							</div>
 						</div>
 					</div>
 				</div>
-				
+
 				<div class="pr">
 					<!-- 动态设置长度及颜色，填写PR即可 -->
 					<div class="pr-bar-bg">
 						{% if data['battleTypeInfo']['PVP']['prInfo']['color'] != '#828282' %}
-						<span class="pr-number">{{ data['battleTypeInfo']['PVP']['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+						<span class="pr-number">{{ data['battleTypeInfo']['PVP']['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text">{{ data['battleTypeInfo']['PVP']['prInfo']['name'] }}</span></span>
 						{% else %}
-						<span class="pr-number">{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+						<span class="pr-number">{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text">{{ data['battleTypeInfo']['PVP']['prInfo']['name'] }}</span></span>
 						{% endif %}
 						<div class="pr-bar"></div>
 					</div>
 				</div>
-				
+
 				<div class="recnet-time">
 					<span>记录时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data['recordTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(time.time())) }}</span>
 				</div>
-				
+
 				{% if data['battleTypeInfo']['PVP']['battle'] %}
 				<div class="overview-change">
 					<div class="overview-change-item left-item">
 						<div class="left-item-top item-top">
 							<div class="overview-count-title item-top-top">场次</div>
 							<div class="overview-count item-top-bottom">{{ data['battleTypeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}</div>
 						</div>
@@ -446,18 +446,18 @@
 								<div class="mini-item-top">KD</div>
 								<div class="mini-item-bottom">{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['kd']) }}</div>
 							</div>
 						</div>
 					</div>
 				</div>
 				{% endif %}
-				
-				
+
+
 				<div class="information-header">总体战绩</div>
-				
+
 				<div class="information-body">
 					<div class="information-col information-table-header">
 						<div class="information-col-item">类型</div>
 						<div class="information-col-item">场次</div>
 						<div class="information-col-item">胜率</div>
 						<div class="information-col-item">PR</div>
 						<div class="information-col-item">场均</div>
@@ -471,56 +471,56 @@
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_SOLO']['prInfo']['color'] }};">{{ data['battleTypeInfo']['PVP_SOLO']['prInfo']['value'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_SOLO']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 					</div>
 					{% endif %}
-					
+
 					{% if data['battleTypeInfo']['PVP_DIV2']['battle'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">自行车</div>
 						<div class="information-col-item">{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV2']['prInfo']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV2']['prInfo']['value'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['frags']) }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV2']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 					</div>
 					{% endif %}
-					
+
 					{% if data['battleTypeInfo']['PVP_DIV3']['battle'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">三轮车</div>
 						<div class="information-col-item">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['prInfo']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['prInfo']['value'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['frags']) }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 					</div>
 					{% endif %}
-					
+
 					{% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">排位</div>
 						<div class="information-col-item">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 					</div>
 					{% endif %}
 				</div>
-				
+
 				{% if data['battleTypeInfo']['PVP']['battle'] %}
 				<div class="random-header">随机战数据</div>
 				{% endif %}
-				
+
 				{% if data['battleTypeInfo']['PVP']['battle'] %}
 				<div class="random-data">
 					<div class="random-table-header">
 						<div class="random-col-item flex-3">等级</div>
 						<div class="random-col-item flex-8">战舰</div>
 						<div class="random-col-item flex-3">场次</div>
 						<div class="random-col-item flex-3">PR</div>
@@ -541,20 +541,20 @@
 							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['typeInfo']['PVP']['battleInfo']['avgInfo']['frags']) }}</div>
 							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['typeInfo']['PVP']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 						</div>
 						{% endif %}
 					{% endfor %}
 				</div>
 				{% endif %}
-				
+
 				<!-- 以下为排位数据，不再额外做类名样式 -->
 				{% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
 				<div class="random-header">排位战数据</div>
 				{% endif %}
-				
+
 				{% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
 				<div class="random-data">
 					<div class="random-table-header">
 						<div class="random-col-item flex-3">等级</div>
 						<div class="random-col-item flex-8">战舰</div>
 						<div class="random-col-item flex-3">场次</div>
 						<div class="random-col-item flex-3">PR</div>
@@ -607,70 +607,70 @@
 						</div>
 						<div class="frag-item">
 							<div class="frag-key">深弹击沉</div>
 							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByDbomb'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByDbomb'] }}</div>
 						</div>
 					</div>
 				</div>
-				
+
 				<div class="footer">
 					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 					<p>Design By 冷眠 H5 Converted By C1ystal</p>
 					<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 				</div>
-				
+
 			</div>
 		</div>
 	</body>
-	
+
 	<script>
 		// PR条颜色动态变化
 		let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
 		let pr_number = document.querySelector('.pr-number').innerText;
 		pr_number = parseInt(pr_number);
 		if (pr_number == 0) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#828282";
-			document.querySelector(".pr-text").innerText = "暂无数据";
+			{#document.querySelector(".pr-text").innerText = "暂无数据";#}
 		} else if (pr_number < 750) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
-			document.querySelector(".pr-text").innerText = "还需努力";
+			{#document.querySelector(".pr-text").innerText = "还需努力";#}
 		} else if (pr_number < 1100) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
-			document.querySelector(".pr-text").innerText = "低于平均";
+			{#document.querySelector(".pr-text").innerText = "低于平均";#}
 		} else if (pr_number < 1350) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
-			document.querySelector(".pr-text").innerText = "平均水平";
+			{#document.querySelector(".pr-text").innerText = "平均水平";#}
 			document.querySelector(".pr-number").style.color = "#303133";
 		} else if (pr_number < 1550) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
-			document.querySelector(".pr-text").innerText = "好";
+			{#document.querySelector(".pr-text").innerText = "好";#}
 		} else if (pr_number < 1750) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
-			document.querySelector(".pr-text").innerText = "很好";
+			{#document.querySelector(".pr-text").innerText = "很好";#}
 		} else if (pr_number < 2100) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
-			document.querySelector(".pr-text").innerText = "非常好";
+			{#document.querySelector(".pr-text").innerText = "非常好";#}
 		} else if (pr_number < 2450) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
-			document.querySelector(".pr-text").innerText = "大佬水平";
+			{#document.querySelector(".pr-text").innerText = "大佬水平";#}
 		} else {
 			document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
-			document.querySelector(".pr-text").innerText = "神佬水平";
+			{#document.querySelector(".pr-text").innerText = "神佬水平";#}
 			pr_number = 2450; //防止pr条溢出
 		}
-	
+
 		if (pr_number < 220 && pr_number > 0) {
 			pr_number = 220; //防止pr过低导致圆角异常
 		}
 		// PR条动态长度
 		let width = bar_bg_width * (pr_number / 2450);
 		document.querySelector('.pr-bar').style.width = width + "px";
 	</script>
-	
+
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
 		if (server_name == "亚服") {
 			document.querySelector(".server").style.color = "#92D050";
 		} else if (server_name == "国服") {
 			document.querySelector(".server").style.color = "#BF9000";
@@ -678,81 +678,81 @@
 			document.querySelector(".server").style.color = "#009664";
 		} else if (server_name == "美服") {
 			document.querySelector(".server").style.color = "#6872C4";
 		} else if (server_name == "俄服") {
 			document.querySelector(".server").style.color = "#FF0000";
 		}
 	</script>
-	
+
 	<script>
 		// 数据变化动态颜色填充
 		let change_avgdmg = document.querySelector(".change-avgdmg").innerText;
 		change_avgdmg = parseInt(change_avgdmg);
-	
+
 		let change_win = document.querySelector(".change-win").innerText;
 		change_win = change_win.split("%", 1);
 		change_win = parseFloat(change_win);
-	
+
 		let change_pr = document.querySelector(".change-pr").innerText;
 		change_pr = parseInt(change_pr);
-	
+
 		if (change_avgdmg > 0) {
 			document.querySelector(".change-avgdmg").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-avgdmg").style.color = "#FF0000";
 		}
-	
+
 		if (change_win > 0) {
 			document.querySelector(".change-win").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-win").style.color = "#FF0000";
 		}
-	
+
 		if (change_pr > 0) {
 			document.querySelector(".change-pr").style.color = "#70AD47";
 		} else {
 			document.querySelector(".change-pr").style.color = "#FF0000";
 		}
 	</script>
-	
+
 	<script>
 		let arr_information = document.getElementsByClassName('information-col');
 		for(let i=0;i<arr_information.length;i++) {
 			if(i%2 != 0 && i == (arr_information.length-1)) {
 				arr_information[i].style.backgroundColor = "#E4E4E4";
 				arr_information[i].style.borderBottomLeftRadius = "16px";
 				arr_information[i].style.borderBottomRightRadius = "16px";
 			} else if (i%2 != 0) {
 				arr_information[i].style.backgroundColor = "#E4E4E4";
 			}
 		}
 	</script>
-	
+
 	<script>
 		let arr_random = document.getElementsByClassName('random-data-col');
 		for(let i=0;i<arr_random.length;i++) {
 			if(i%2 == 0 && i == (arr_random.length-1)) {
 				arr_random[i].style.backgroundColor = "#E4E4E4";
 				arr_random[i].style.borderBottomLeftRadius = "16px";
 				arr_random[i].style.borderBottomRightRadius = "16px";
 			} else if (i%2 == 0) {
 				arr_random[i].style.backgroundColor = "#E4E4E4";
 			}
 		}
 	</script>
-	
+
 	<script>
 		let ship_level_doc = document.getElementsByClassName('ship-level');
 		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
 		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
 		for(let k=0;k<ship_level_doc.length;k++) {
 			ship_level_doc[k].innerText = level_roma[level_number.indexOf(ship_level_doc[k].innerText)];
 		}
 	</script>
-	
+
 	<script>
 		let arr_rank = document.getElementsByClassName('rank-data-col');
 		for(let i=0;i<arr_rank.length;i++) {
 			if(i%2 == 0 && i == (arr_rank.length-1)) {
 				arr_rank[i].style.backgroundColor = "#E4E4E4";
 				arr_rank[i].style.borderBottomLeftRadius = "16px";
 				arr_rank[i].style.borderBottomRightRadius = "16px";
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 {% if data['userInfo']['clanInfo']['tag'] %}
 [{{ data['userInfo']['clanInfo']['tag'] }}]
 {% endif %}
 {{ data['userInfo']['userName'] }}
 {{ data['userInfo']['serverCn'] }}
 {% if data['battleTypeInfo']['PVP']['prInfo']['color'] != '#828282' %} {{ data
-['battleTypeInfo']['PVP']['prInfo']['value'] }}     {% else %} {{ data
-['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}     {% endif %}
+['battleTypeInfo']['PVP']['prInfo']['value'] }}    {{ data['battleTypeInfo']
+['PVP']['prInfo']['name'] }} {% else %} {{ data['battleTypeInfo']['RANK_SOLO']
+['prInfo']['value'] }}    {{ data['battleTypeInfo']['PVP']['prInfo']['name'] }}
+{% endif %}
 记录时间：{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data
 ['recordTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime
 (time.time())) }}
 {% if data['battleTypeInfo']['PVP']['battle'] %}
 场次
 {{ data['battleTypeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}
 基础经验
```

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-info-recents.html` & `hikari_core-1.1.0/hikari_core/Template/wws-info-recents.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-info.html` & `hikari_core-1.1.0/hikari_core/Template/wws-info.html`

 * *Files 2% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 					</div>
 				</div>
 
 				<div class="pr">
 					<!-- 动态设置长度及颜色，填写PR即可 -->
 					<div class="pr-bar-bg">
 						<span class="pr-number">{{ data['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span
-								class="pr-text"></span></span>
+								class="pr-text">{{ data['prInfo']['name'] }}</span></span>
 						<div class="pr-bar"></div>
 					</div>
 				</div>
 
 				<div class="recnet-time">
 					<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['lastBattleTime'])))}}</span>
 				</div>
@@ -701,40 +701,40 @@
 <script>
 	// PR条颜色动态变化
 	let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
 	let pr_number = document.querySelector('.pr-number').innerText;
 	pr_number = parseInt(pr_number);
 	if (pr_number == 0) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#828282";
-		document.querySelector(".pr-text").innerText = "暂无数据";
+		{#document.querySelector(".pr-text").innerText = "暂无数据";#}
 	} else if (pr_number < 750) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
-		document.querySelector(".pr-text").innerText = "还需努力";
+		{#document.querySelector(".pr-text").innerText = "还需努力";#}
 	} else if (pr_number < 1100) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
-		document.querySelector(".pr-text").innerText = "低于平均";
+		{#document.querySelector(".pr-text").innerText = "低于平均";#}
 	} else if (pr_number < 1350) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
-		document.querySelector(".pr-text").innerText = "平均水平";
+		{#document.querySelector(".pr-text").innerText = "平均水平";#}
 		document.querySelector(".pr-number").style.color = "#303133";
 	} else if (pr_number < 1550) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
-		document.querySelector(".pr-text").innerText = "好";
+		{#document.querySelector(".pr-text").innerText = "好";#}
 	} else if (pr_number < 1750) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
-		document.querySelector(".pr-text").innerText = "很好";
+		{#document.querySelector(".pr-text").innerText = "很好";#}
 	} else if (pr_number < 2100) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
-		document.querySelector(".pr-text").innerText = "非常好";
+		{#document.querySelector(".pr-text").innerText = "非常好";#}
 	} else if (pr_number < 2450) {
 		document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
-		document.querySelector(".pr-text").innerText = "大佬水平";
+		{#document.querySelector(".pr-text").innerText = "大佬水平";#}
 	} else {
 		document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
-		document.querySelector(".pr-text").innerText = "神佬水平";
+		{#document.querySelector(".pr-text").innerText = "神佬水平";#}
 		pr_number = 2450; //防止pr条溢出
 	}
 
 	if (pr_number < 220 && pr_number > 0) {
 		pr_number = 220; //防止pr过低导致圆角异常
 	}
 	// PR条动态长度
@@ -811,8 +811,8 @@
 			arr_information[i].style.borderBottomRightRadius = "16px";
 		} else if (i % 2 != 0) {
 			arr_information[i].style.backgroundColor = "#E4E4E4";
 		}
 	}
 </script>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% if data['userInfo']['clanInfo']['tag'] %}
 [{{ data['userInfo']['clanInfo']['tag'] }}]
 {% endif %}
 {{ data['userInfo']['userName'] }}
 {{ data['userInfo']['serverCn'] }}
-{{ data['prInfo']['value'] }}    
+{{ data['prInfo']['value'] }}    {{ data['prInfo']['name'] }}
 最后战斗时间：{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data
 ['lastBattleTime'])))}}
 场次
 {{ data['battleTypeInfo']['PVP']['shipInfo']['battleInfo']['battle'] }}
 PR
 较上次
 {{ '%+d' | format(data['dwpData']['pr']) }}
```

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-personalRecord.html` & `hikari_core-1.1.0/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-ship-recent.html` & `hikari_core-1.1.0/hikari_core/Template/wws-ship.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,133 @@
 <!DOCTYPE html>
 <html>
 	<head>
 		<meta charset="utf-8">
 		<title></title>
+		<link rel="stylesheet" type="text/css" href="wws-ship.css" />
 	</head>
 	<style>
 		* {
 			padding: 0;
 			margin: 0;
 		}
 
-		.flex-2 {
-			flex: 2;
-		}
-
-		.flex-3 {
-			flex: 3;
-		}
-
-		.flex-4 {
-			flex: 4;
-		}
-
-		.flex-8 {
-			flex: 8;
-		}
-
-		.flex-10 {
-			flex: 10;
-		}
-
 		.main-content {
 			width: 1000px;
-			font-size: 30px;
+			border-radius: 16px;
 			font-family: "Microsoft YaHei";
-			font-weight: bold;
+			font-size: 30px;
 		}
 
 		.page-box {
 			width: 1000px;
 			display: flex;
 			flex-direction: column;
 		}
 
 		.page-header {
-			display: flex;
-			flex-direction: column;
+			font-size: 40px;
+			padding: 20px;
 		}
 
 		.clan-user-server {
-			height: 120px;
+			height: 80px;
+			line-height: 80px;
+			font-weight: bold;
 			text-align: center;
-			font-size: 45px;
-			line-height: 120px;
 		}
 
 		.clan {
 			display: inline-block;
+			height: 80px;
 			padding-right: 10px;
-			height: 120px;
 		}
 
-		.user {
+		.server {
 			display: inline-block;
-			height: 120px;
+			height: 80px;
+			padding-left: 20px;
 		}
 
-		.server {
+		.username {
 			display: inline-block;
-			padding-left: 10px;
+			height: 80px;
 		}
 
 		.server-border {
-			width: 200px;
-			height: 50px;
-			line-height: 50px;
+			width: 160px;
+			height: 40px;
+			margin-top: 20px;
+			line-height: 40px;
 			text-align: center;
 			background-color: #F2F2F2;
-			border-radius: 25px;
-			font-size: 35px;
+			border-radius: 20px;
+			font-size: 30px;
 		}
 
-		.ship-bar {
-			height: 80px;
-			font-size: 40px;
-			line-height: 80px;
-			text-align: center;
+		.ship-detail {
 			display: flex;
+			height: 60px;
+			line-height: 60px;
+			font-weight: bold;
 		}
 
+
 		.ship-level {
 			flex: 1;
 			text-align: right;
-			margin-right: 30px;
+			padding-right: 60px;
+		}
+
+		.ship-name {
+			display: inline-block;
+			height: 60px;
 		}
 
 		.ship-icon {
 			flex: 1;
-			text-align: left;
-			margin-left: 30px;
+			padding-left: 70px;
 		}
 
 		.ship-icon img {
-			width: 80px;
-			height: 80px;
+			width: 60px;
+			height: 60px;
+		}
+
+
+		.ranking {
+			display: flex;
+			justify-content: space-around;
+			align-content: space-around;
+			height: 60px;
+			line-height: 40px;
+			font-weight: bold;
+			margin-bottom: 15px;
+		}
+
+		.ranking_border {
+			margin-top: 10px;
+			height: 40px;
+			border-radius: 28px;
+			padding: 4px 20px;
+			background-color: #F2F2F2;
+		}
+
+		.last-time {
+			text-align: center;
+			color: #606266;
 		}
 
 		.pr {
 			display: flex;
-			height: 100px;
+			height: 120px;
 			font-weight: bold;
 			line-height: 60px;
-			padding: 0 50px;
+			padding: 0 60px;
+			margin-top: 20px;
 		}
 
 		.pr-bar-bg {
 			position: relative;
 			flex: 1;
 			line-height: 80px;
 			background-color: #A6A6A6;
@@ -140,480 +152,448 @@
 			position: absolute;
 			left: 0px;
 			right: 0px;
 			font-size: 35px;
 			font-weight: bold;
 		}
 
-		.recnet-time {
-			text-align: center;
-			font-weight: normal;
+		.data-change {
+			margin: 10px 60px;
+			height: 120px;
+			display: flex;
+			flex-direction: column;
+			background-color: #F2F2F2;
+			border-radius: 15px;
+			font-weight: bold;
 		}
 
-		.overview-change {
+		.change-header {
+			flex: 1;
 			display: flex;
-			margin-top: 30px;
-			padding: 0 30px;
-			height: 300px;
+			background-color: #D9D9D9;
+			border-radius: 15px;
+			color: #606266;
 		}
 
-		.overview-change-item {
+		.change-body {
 			flex: 1;
 			display: flex;
-			flex-direction: column;
-			margin: 0 20px;
-
 		}
 
-		.item-top {
-			flex: 5;
-			background-color: #F2F2F2;
-			border-radius: 16px;
+		.change-header-item,
+		.change-body-item {
+			flex: 1;
+			text-align: center;
+			line-height: 60px;
 		}
 
-		.item-bottom {
+		.ship-overview {
+			margin: 10px 50px;
+			height: 420px;
 			display: flex;
-			flex: 4;
-			margin-top: 20px;
-		}
-
-		.left-item-bottom {
-			background-color: #F2F2F2;
-			border-radius: 16px;
+			flex-direction: column;
 		}
 
-		.bottom-mini-item-left {
+		.overview-col {
 			flex: 1;
-			margin-right: 10px;
-			background-color: #F2F2F2;
-			border-radius: 16px;
+			display: flex;
 		}
 
-		.bottom-mini-item-right {
+		.overview-item {
 			flex: 1;
-			margin-left: 10px;
 			background-color: #F2F2F2;
-			border-radius: 16px;
-		}
-
-		.item-top {
+			border-radius: 15px;
+			margin: 10px;
 			display: flex;
 			flex-direction: column;
-		}
-
-		.item-top div {
-			height: 80px;
-			text-align: center;
 			font-size: 40px;
+			font-weight: bold;
 		}
 
-		.item-top-top {
+		.overview-item-title {
+			height: 95px;
+			line-height: 125px;
+			text-align: center;
 			color: #606266;
-			font-weight: normal;
-			line-height: 100px;
 		}
 
-		.item-top-bottom {
-			line-height: 60px;
+		.overview-item-data {
+			height: 95px;
+			line-height: 65px;
+			text-align: center;
 		}
 
-		.left-item-bottom {
-			display: flex;
-			flex-direction: column;
-		}
 
-		.change-pr-title {
-			color: #606266;
-			height: 60px;
-			display: flex;
-			font-weight: normal;
-			line-height: 70px;
-		}
 
-		.change-pr {
+
+		.information-header {
+			width: 680px;
+			margin: 20px 160px;
 			height: 60px;
-			line-height: 50px;
+			line-height: 60px;
+			font-weight: bold;
 			text-align: center;
-			font-size: 30px;
-		}
-
-		.change-pr-title-left {
-			flex: 1;
-			font-size: 35px;
-			text-align: right;
-			margin-right: 30px;
-		}
-
-		.change-pr-title-right {
-			flex: 1;
-			font-size: 20px;
+			background-color: #BFBFBF;
+			border-radius: 15px;
 		}
 
-		.bottom-mini-item-left,
-		.bottom-mini-item-right {
+		.information-body {
+			width: 880px;
+			margin: 0 60px;
+			margin-top: 30px;
 			display: flex;
 			flex-direction: column;
+			font-weight: bold;
+			background-color: #F2F2F2;
+			border-radius: 15px;
 		}
 
-		.mini-item-top {
+		.information-body-top {
+			display: flex;
+			background-color: #D9D9D9;
+			border-radius: 8px;
 			color: #606266;
-			font-weight: normal;
-			line-height: 70px;
 		}
 
-		.mini-item-bottom {
-			line-height: 45px;
-			font-size: 27px;
-		}
-
-		.bottom-mini-item-left div,
-		.bottom-mini-item-right div {
-			height: 60px;
-			text-align: center;
-		}
-
-		.information-header,
-		.day-header {
-			margin: 0 200px;
-			margin-top: 30px;
+		.information-item {
 			height: 60px;
 			line-height: 60px;
-			border-radius: 16px;
-			background-color: #D9D9D9;
+			flex: 1;
 			text-align: center;
 		}
 
-		.information-body {
-			margin: 0 50px;
-			margin-top: 30px;
+		.information-body-data {
 			display: flex;
-			flex-direction: column;
-			background-color: #F2F2F2;
-			border-radius: 16px;
+			border-radius: 8px;
 		}
 
-		.information-col {
+		.ship-highest-header {
 			height: 60px;
-			display: flex;
 			line-height: 60px;
-		}
-
-		.information-col-item,
-		.day-col-item {
-			flex: 1;
+			width: 680px;
+			margin: 40px 160px 20px 160px;
+			font-weight: bold;
 			text-align: center;
+			background-color: #BFBFBF;
+			border-radius: 15px;
 		}
 
-		.information-table-header {
-			color: #606266;
+		.ship-highest-data {
+			width: 900px;
+			margin: 20px 50px;
+			display: flex;
+			flex-direction: column;
 		}
 
-		.information-type {
-			color: #909399;
+		.high-col {
+			display: flex;
+			justify-content: space-around;
 		}
 
-		.day-body {
-			margin: 0 50px;
-			margin-top: 30px;
+		.high-item {
+			flex: 1;
+			height: 120px;
+			line-height: 100px;
+			background-color: #F2F2F2;
+			border-radius: 8px;
+			display: flex;
+			flex-direction: column;
+			margin: 10px;
 		}
 
-		.day-table-header {
+		.high-item-top {
 			height: 60px;
-			line-height: 60px;
-			background-color: #D9D9D9;
-			display: flex;
-			border-radius: 16px;
+			line-height: 70px;
+			font-weight: bold;
 			color: #606266;
-		}
-
-		.date {
-			background-color: #D9D9D9;
-			width: 300px;
-			height: 40px;
-			line-height: 40px;
 			text-align: center;
-			border-radius: 20px;
-			margin-top: 10px;
 		}
 
-		.day-col {
-			display: flex;
+		.high-item-bottom {
 			height: 60px;
-			line-height: 60px;
-			background-color: #F2F2F2;
-			border-radius: 30px;
-			margin: 10px 0;
+			line-height: 50px;
+			font-weight: bold;
+			text-align: center;
 		}
 
 		.footer {
-			margin-top: 30px;
 			text-align: center;
 			font-weight: bold;
 			font-size: 24px;
 			color: #909399;
 			margin-bottom: 20px;
 		}
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
 				<div class="page-header">
-					<div class="clan-user-server">
-						{% if data['userInfo']['clanInfo']['tag'] %}
-						<div class="clan" style="color: {{ data['userInfo']['clanInfo']['color'] }};">[{{ data['userInfo']['clanInfo']['tag'] }}]</div>
+
+						<div class="clan-user-server">
+					 	{% if data['userInfo']['clanInfo']['tag'] %}
+							<div class="clan" style="color: {{ data['userInfo']['clanInfo']['color'] }};">
+								[{{ data['userInfo']['clanInfo']['tag'] }}]</div>
 						{% endif %}
-						<div class="user">{{ data['userInfo']['userName'] }}</div>
-						<div class="server">
-							<div class="server-border">
-								{{ data['userInfo']['serverCn'] }}
+							<div class="username">{{ data['userInfo']['userName'] }}</div>
+							<div class="server">
+								<!-- 动态设置服务器字体颜色 -->
+								<div class="server-border">{{ data['userInfo']['serverCn'] }}</div>
 							</div>
 						</div>
-					</div>
-				</div>
 
-				<div class="ship-bar">
-					<div class="ship-level">{{ data['shipInfoBattleList'][0]['shipInfo']['level'] }}</div>
-					<div class="ship-name">{{ data['shipInfoBattleList'][0]['shipInfo']['nameCn'] }}</div>
-					
-					<div class="ship-icon"><img
-									src={% if data['shipInfoBattleList'][0]['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
-									{% elif data['shipInfoBattleList'][0]['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
-									{% elif data['shipInfoBattleList'][0]['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
-									{% elif data['shipInfoBattleList'][0]['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
+						<div class="ship-detail">
+							<div class="ship-level">{{ data['shipInfo']['level'] }}</div>
+							<div class="ship-name">{{ data['shipInfo']['nameCn'] }}</div>
+							<div class="ship-icon"><img
+									src={% if data['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
+									{% elif data['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
+									{% elif data['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
+									{% elif data['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
 									{% else %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png"
-									{% endif %} />
+									{% endif %} /></div>
+						</div>
 					</div>
-				</div>
 
-				<div class="pr">
-					<!-- 动态设置长度及颜色，填写PR即可 -->
-					<div class="pr-bar-bg">
-						{% if data['battleTypeInfo']['PVP']['prInfo']['color'] != '#828282' %}
-						<span class="pr-number">{{ data['battleTypeInfo']['PVP']['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
-						{% else %}
-						<span class="pr-number">{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
-						{% endif %}
-						<div class="pr-bar"></div>
+					<div class="pr">
+						<!-- 动态设置长度及颜色，填写PR即可 -->
+						<div class="pr-bar-bg">
+							{% if data['typeInfo']['PVP']['prInfo']['color'] and data['typeInfo']['PVP']['prInfo']['color'] != '#828282' %}
+							<span class="pr-number">{{ data['typeInfo']['PVP']['prInfo']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
+									class="pr-text">{{ data['typeInfo']['PVP']['prInfo']['name'] }}</span></span>
+							{% else %}
+							<span class="pr-number">{{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
+									class="pr-text">{{ data['typeInfo']['RANK_SOLO']['prInfo']['name'] }}</span></span>
+							{% endif %}
+							<div class="pr-bar"></div>
+						</div>
 					</div>
-				</div>
 
-				<div class="recnet-time">
-					<span>记录时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data['recordTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(time.time())) }}</span>
-				</div>
+					<div class="last-time">
+						<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['typeInfo']['PVP']['battleInfo']['lastBattleTime']))) }}</span>
+					</div>
 
-				{% if data['battleTypeInfo']['PVP']['battle'] %}
-				<div class="overview-change">
-					<div class="overview-change-item left-item">
-						<div class="left-item-top item-top">
-							<div class="overview-count-title item-top-top">场次</div>
-							<div class="overview-count item-top-bottom">{{ data['battleTypeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}</div>
-						</div>
-						<div class="left-item-bottom item-bottom">
-							<div class="change-avgdmg-box bottom-mini-item-left">
-								<div class="mini-item-top">基础经验</div>
-								{% if data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['basicXp'] %}
-								<div class="mini-item-bottom change-avgdmg">{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['basicXp'] }}</div>
-								{% else %}
-								<div class="mini-item-bottom change-avgdmg">暂不可用</div>
-								{% endif %}
-							</div>
-							<div class="change-win-box bottom-mini-item-right">
-								<div class="mini-item-top">加成经验</div>
-								<div class="mini-item-bottom change-win">{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['xp'] }}</div>
-							</div>
+					{% if data['shipRank'] %}
+					<div class="ranking">
+						<div class="ranking_border"><span
+								style="color: #606266;">排名</span>&nbsp;&nbsp;<span>{{data['shipRank']}}</span>
 						</div>
 					</div>
-					<div class="overview-change-item mid-item">
-						<div class="mid-item-top item-top">
-							<div class="overview-win-title item-top-top">胜率</div>
-							<div class="overview-win item-top-bottom" style="color: {{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%</div>
-						</div>
-						<div class="mid-item-bottom item-bottom">
-							<div class="change-avgdmg-box bottom-mini-item-left">
-								<div class="mini-item-top">侦察</div>
-								<div class="mini-item-bottom change-avgdmg">{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['shipsSpotted']) }}</div>
-							</div>
-							<div class="change-win-box bottom-mini-item-right">
-								<div class="mini-item-top">击落</div>
-								<div class="mini-item-bottom change-win">{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['planesKilled']) }}</div>
+					{% endif %}
+
+					<div class="data-change">
+						<div class="change-header">
+							<div class="change-header-item">场均</div>
+							<div class="change-header-item">胜率</div>
+							<div class="change-header-item">PR</div>
+						</div>
+						<div class="change-body">
+							<div class="change-body-item change-avgdmg">
+								{{ '%+d' | format(data['dwpData']['damage']) }}</div>
+							<div class="change-body-item change-win">{{ '%+.2f' | format(data['dwpData']['wins']) }}
 							</div>
+							<div class="change-body-item change-pr">{{ '%+d' | format(data['dwpData']['pr']) }}</div>
 						</div>
 					</div>
-					<div class="overview-change-item right-item">
-						<div class="right-item-top item-top">
-							<div class="overview-avgdmg-title item-top-top">场均</div>
-							<div class="overview-avgdmg item-top-bottom" style="color: {{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}</div>
-						</div>
-						<div class="right-item-bottom item-bottom">
-							<div class="overview-kd-box bottom-mini-item-left">
-								<div class="mini-item-top">击杀</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['frags']) }}</div>
-							</div>
-							<div class="overview-hit-box bottom-mini-item-right">
-								<div class="mini-item-top">KD</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['kd']) }}</div>
+
+					<div class="ship-overview">
+						<div class="overview-col">
+							<div class="overview-item">
+								<div class="overview-item-title">场次</div>
+								<div class="overview-item-data">{{ data['typeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">胜率</div>
+								<div class="overview-item-data"
+									style="color: {{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['winsData']['color'] }};">
+									{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">场均</div>
+								<div class="overview-item-data"
+									style="color: {{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['damageData']['color'] }};">
+									{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}</div>
+							</div>
+						</div>
+						<div class="overview-col">
+							<div class="overview-item">
+								<div class="overview-item-title">经验</div>
+								<div class="overview-item-data">{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['xp'] }}</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">击杀</div>
+								<div class="overview-item-data">{{ '%.2f' | format(data['typeInfo']['PVP']['battleInfo']['avgInfo']['frags']) }}</div>
+							</div>
+							<div class="overview-item">
+								<div class="overview-item-title">命中</div>
+								<div class="overview-item-data">{{ data['typeInfo']['PVP']['battleInfo']['hitRatioInfo']['ratioMain'] }}%</div>
 							</div>
 						</div>
 					</div>
-				</div>
-				{% endif %}
 
-				<div class="information-header">总体战绩</div>
-
-				<div class="information-body">
-					<div class="information-col information-table-header">
-						<div class="information-col-item">类型</div>
-						<div class="information-col-item">场次</div>
-						<div class="information-col-item">胜率</div>
-						<div class="information-col-item">PR</div>
-						<div class="information-col-item">场均</div>
-						<div class="information-col-item">击杀</div>
-					</div>
-					
-					{% if data['battleTypeInfo']['PVP_SOLO']['battle'] %}
-					<div class="information-col">
-						<div class="information-col-item information-type">单野</div>
-						<div class="information-col-item">{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_SOLO']['prInfo']['color'] }};">{{ data['battleTypeInfo']['PVP_SOLO']['prInfo']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_SOLO']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
-					</div>
-					{% endif %}
-					
-					{% if data['battleTypeInfo']['PVP_DIV2']['battle'] %}
-					<div class="information-col">
-						<div class="information-col-item information-type">自行车</div>
-						<div class="information-col-item">{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV2']['prInfo']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV2']['prInfo']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV2']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
-					</div>
-					{% endif %}
-					
-					{% if data['battleTypeInfo']['PVP_DIV3']['battle'] %}
-					<div class="information-col">
-						<div class="information-col-item information-type">三轮车</div>
-						<div class="information-col-item">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['prInfo']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['prInfo']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
+					<div class="information-header">
+						总体战绩
 					</div>
-					{% endif %}
-					
-					{% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
-					<div class="information-col">
-						<div class="information-col-item information-type">排位</div>
-						<div class="information-col-item">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
-					</div>
-					{% endif %}
-
-				</div>
 
-				<div class="day-header">每日战绩</div>
+					<div class="information-body">
+						<div class="information-body-top">
+							<div class="information-item">类型</div>
+							<div class="information-item">场次</div>
+							<div class="information-item">胜率</div>
+							<div class="information-item">PR</div>
+							<div class="information-item">场均</div>
+							<div class="information-item">击杀</div>
+						</div>
 
-				<div class="day-body">
-					<div class="day-table-header">
-						<div class="day-col-item">类型</div>
-						<div class="day-col-item">场次</div>
-						<div class="day-col-item">胜率</div>
-						<div class="day-col-item">PR</div>
-						<div class="day-col-item">场均</div>
-						<div class="day-col-item">击杀</div>
+						{% if data['typeInfo']['PVP_SOLO']['battle'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">单野</div>
+							<div class="information-item">{{ data['typeInfo']['PVP_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['PVP_SOLO']['prInfo']['color'] }};">
+								{{ data['typeInfo']['PVP_SOLO']['prInfo']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
+						</div>
+						{% endif %}
+						{% if data['typeInfo']['PVP_DIV2']['battle'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">自行车</div>
+							<div class="information-item">{{ data['typeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['PVP_DIV2']['prInfo']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV2']['prInfo']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['frags']) }}</div>
+						</div>
+						{% endif %}
+						{% if data['typeInfo']['PVP_DIV3']['battle'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">三轮车</div>
+							<div class="information-item">{{ data['typeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['PVP_DIV3']['prInfo']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV3']['prInfo']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['frags']) }}</div>
+						</div>
+						{% endif %}
+						{% if data['typeInfo']['RANK_SOLO']['battle'] %}
+						<div class="information-body-data">
+							<div class="information-item" style="color: #909399;">排位</div>
+							<div class="information-item">{{ data['typeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['RANK_SOLO']['prInfo']['color'] }};">
+								{{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }}</div>
+							<div class="information-item"
+								style="color: {{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
+						</div>
+						{% endif %}
 					</div>
 
+					<div class="ship-highest-header">
+						最高纪录
+					</div>
 
-						<div class="data-item">
-							{% for eachShipData in data['shipInfoBattleList'] %}
-							    {% if eachShipData['typeInfo']['PVP']['battle'] or eachShipData['typeInfo']['RANK_SOLO']['battle'] %}
-								<div class="date">{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData['recordDateTime']/1000)))) }}</div>
-									{% for each in eachShipData %}
-										{% for index,value in enumerate(['shipSolo','shipTwo','shipThree','rankSolo']) %}
-											{% if each|string == value and eachShipData[each]['battles'] %}
-											<div class="day-data">
-												<div class="day-col">
-													<div class="day-col-item" style="color: #606266;;">{{ ['单野','自行车','三轮车','排位'][index] }}</div>
-													<div class="day-col-item">{{ eachShipData[each]['battles'] }}</div>
-													<div class="day-col-item" style="color: {{ eachShipData[each]['winsData']['color'] }};">{{ eachShipData[each]['wins'] }}%</div>
-													<div class="day-col-item" style="color: {{ eachShipData[each]['pr']['color'] }};">{{ eachShipData[each]['pr']['value'] }}</div>
-													<div class="day-col-item" style="color: {{ eachShipData[each]['damageData']['color'] }};">{{ eachShipData[each]['damage'] }}</div>
-													<div class="day-col-item">{{ '%.2f' | format(eachShipData[each]['frags']) }}</div>
-												</div>
-											</div>
-											{% endif %}
-										{% endfor %}
-									{% endfor %}
-								{% endif %}
-							{% endfor %}
+					<div class="ship-highest-data">
+						<div class="high-col">
+							<div class="high-item">
+								<div class="high-item-top">最高伤害</div>
+								<div class="high-item-bottom">{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxDamageDealt']['value'] }}
+								</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">侦察伤害</div>
+								<div class="high-item-bottom">
+									{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxScoutingDamage']['value'] }}</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">最高潜在</div>
+								<div class="high-item-bottom">
+									{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxTotalAgro']['value'] }}</div>
+							</div>
+						</div>
+						<div class="high-col">
+							<div class="high-item">
+								<div class="high-item-top">经验</div>
+								<div class="high-item-bottom">{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxXp']['value'] }}</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">击杀</div>
+								<div class="high-item-bottom">{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxFrags']['value'] }}
+								</div>
+							</div>
+							<div class="high-item">
+								<div class="high-item-top">飞机击落</div>
+								<div class="high-item-bottom">
+									{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxPlanesKilled']['value'] }}</div>
+							</div>
 						</div>
+					</div>
 
 					<div class="footer">
-						<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
+						<p>© 西行寺雨季&nbsp;&nbsp;© 本心</p>
 						<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 						<p>Design By 冷眠 H5 Converted By C1ystal</p>
 						<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 					</div>
-
 				</div>
-
-
-
 			</div>
-		</div>
 	</body>
 	<script>
-		// PR条颜色动态变化
+		// 胜率条颜色动态变化
 		let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
 		let pr_number = document.querySelector('.pr-number').innerText;
 		pr_number = parseInt(pr_number);
 		if (pr_number == 0) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#828282";
-			document.querySelector(".pr-text").innerText = "暂无数据";
+			{#document.querySelector(".pr-text").innerText = "暂无数据";#}
 		} else if (pr_number < 750) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
-			document.querySelector(".pr-text").innerText = "还需努力";
+			{#document.querySelector(".pr-text").innerText = "还需努力";#}
 		} else if (pr_number < 1100) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
-			document.querySelector(".pr-text").innerText = "低于平均";
+			{#document.querySelector(".pr-text").innerText = "低于平均";#}
 		} else if (pr_number < 1350) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
-			document.querySelector(".pr-text").innerText = "平均水平";
+			{#document.querySelector(".pr-text").innerText = "平均水平";#}
 			document.querySelector(".pr-number").style.color = "#303133";
 		} else if (pr_number < 1550) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
-			document.querySelector(".pr-text").innerText = "好";
+			{#document.querySelector(".pr-text").innerText = "好";#}
 		} else if (pr_number < 1750) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
-			document.querySelector(".pr-text").innerText = "很好";
+			{#document.querySelector(".pr-text").innerText = "很好";#}
 		} else if (pr_number < 2100) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
-			document.querySelector(".pr-text").innerText = "非常好";
+			{#document.querySelector(".pr-text").innerText = "非常好";#}
 		} else if (pr_number < 2450) {
 			document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
-			document.querySelector(".pr-text").innerText = "大佬水平";
+			{#document.querySelector(".pr-text").innerText = "大佬水平";#}
 		} else {
 			document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
-			document.querySelector(".pr-text").innerText = "神佬水平";
+			{#document.querySelector(".pr-text").innerText = "神佬水平";#}
 			pr_number = 2450; //防止pr条溢出
 		}
 
 		if (pr_number < 220 && pr_number > 0) {
 			pr_number = 220; //防止pr过低导致圆角异常
 		}
-		// PR条动态长度
+		// 胜率条动态长度
 		let width = bar_bg_width * (pr_number / 2450);
 		document.querySelector('.pr-bar').style.width = width + "px";
 	</script>
 
 	<script>
 		// 服务器字体颜色自动填充
 		let server_name = document.querySelector(".server").innerText;
@@ -665,20 +645,8 @@
 		let ship_level = document.querySelector(".ship-level").innerText;
 		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
 		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
 		let ship_level_roma = level_roma[level_number.indexOf(ship_level)]
 		document.querySelector(".ship-level").innerText = ship_level_roma;
 	</script>
 
-	<script>
-		let arr_information = document.getElementsByClassName('information-col');
-		for (let i = 0; i < arr_information.length; i++) {
-			if (i % 2 != 0 && i == (arr_information.length - 1)) {
-				arr_information[i].style.backgroundColor = "#E4E4E4";
-				arr_information[i].style.borderBottomLeftRadius = "16px";
-				arr_information[i].style.borderBottomRightRadius = "16px";
-			} else if (i % 2 != 0) {
-				arr_information[i].style.backgroundColor = "#E4E4E4";
-			}
-		}
-	</script>
 </html>
```

#### html2text {}

```diff
@@ -1,126 +1,106 @@
 {% if data['userInfo']['clanInfo']['tag'] %}
 [{{ data['userInfo']['clanInfo']['tag'] }}]
 {% endif %}
 {{ data['userInfo']['userName'] }}
 {{ data['userInfo']['serverCn'] }}
-{{ data['shipInfoBattleList'][0]['shipInfo']['level'] }}
-{{ data['shipInfoBattleList'][0]['shipInfo']['nameCn'] }}
+{{ data['shipInfo']['level'] }}
+{{ data['shipInfo']['nameCn'] }}
 = 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/
-shipType_Icon/icon_sunk_destroyer.png" {% elif data['shipInfoBattleList'][0]
-['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-
-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png" {% elif data
-['shipInfoBattleList'][0]['shipInfo']['shipType'] == 'Battleship' %} "https://
-hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
-icon_sunk_battleship.png" {% elif data['shipInfoBattleList'][0]['shipInfo']
-['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-
-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png" {% else %}
-"https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
-icon_sunk_submarine.png" {% endif %} />
-{% if data['battleTypeInfo']['PVP']['prInfo']['color'] != '#828282' %} {{ data
-['battleTypeInfo']['PVP']['prInfo']['value'] }}     {% else %} {{ data
-['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}     {% endif %}
-记录时间：{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data
-['recordTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime
-(time.time())) }}
-{% if data['battleTypeInfo']['PVP']['battle'] %}
-场次
-{{ data['battleTypeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}
-基础经验
-{% if data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['basicXp'] %}
-{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['basicXp'] }}
-{% else %}
-暂不可用
+shipType_Icon/icon_sunk_destroyer.png" {% elif data['shipInfo']['shipType'] ==
+'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/
+shipType_Icon/icon_sunk_cruiser.png" {% elif data['shipInfo']['shipType'] ==
+'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/
+shipType_Icon/icon_sunk_battleship.png" {% elif data['shipInfo']['shipType'] ==
+'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/
+shipType_Icon/icon_sunk_aircarrier.png" {% else %} "https://hikari-
+resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png" {%
+endif %} />
+{% if data['typeInfo']['PVP']['prInfo']['color'] and data['typeInfo']['PVP']
+['prInfo']['color'] != '#828282' %} {{ data['typeInfo']['PVP']['prInfo']
+['value'] }}     {{ data['typeInfo']['PVP']['prInfo']['name'] }} {% else %} {
+{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }}     {{ data['typeInfo']
+['RANK_SOLO']['prInfo']['name'] }} {% endif %}
+最后战斗时间：{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['typeInfo']
+['PVP']['battleInfo']['lastBattleTime']))) }}
+{% if data['shipRank'] %}
+排名  {{data['shipRank']}}
 {% endif %}
-加成经验
-{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['xp'] }}
+场均
+胜率
+PR
+{{ '%+d' | format(data['dwpData']['damage']) }}
+{{ '%+.2f' | format(data['dwpData']['wins']) }}
+{{ '%+d' | format(data['dwpData']['pr']) }}
+场次
+{{ data['typeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}
 胜率
-{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%
-侦察
-{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']
-['shipsSpotted']) }}
-击落
-{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']
-['planesKilled']) }}
+{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%
 场均
-{{ data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}
+经验
+{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['xp'] }}
 击杀
-{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']
-['frags']) }}
-KD
-{{ '%.2f' | format(data['battleTypeInfo']['PVP']['battleInfo']['avgInfo']
-['kd']) }}
-{% endif %}
+{{ '%.2f' | format(data['typeInfo']['PVP']['battleInfo']['avgInfo']['frags'])
+}}
+命中
+{{ data['typeInfo']['PVP']['battleInfo']['hitRatioInfo']['ratioMain'] }}%
 总体战绩
 类型
 场次
 胜率
 PR
 场均
 击杀
-{% if data['battleTypeInfo']['PVP_SOLO']['battle'] %}
+{% if data['typeInfo']['PVP_SOLO']['battle'] %}
 单野
-{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['battleInfo']['battle'] }}
-{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%
-{{ data['battleTypeInfo']['PVP_SOLO']['prInfo']['value'] }}
-{{ data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}
-{{ '%.2f' | format(data['battleTypeInfo']['PVP_SOLO']['battleInfo']['avgInfo']
+{{ data['typeInfo']['PVP_SOLO']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['PVP_SOLO']['prInfo']['value'] }}
+{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']
 ['frags']) }}
-{{ '%.2f' | format(data['battleTypeInfo']['PVP_SOLO']['battleInfo']
-['hitRatioInfo']['ratioMain']) }}%
-{% endif %} {% if data['battleTypeInfo']['PVP_DIV2']['battle'] %}
+{% endif %} {% if data['typeInfo']['PVP_DIV2']['battle'] %}
 自行车
-{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}
-{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%
-{{ data['battleTypeInfo']['PVP_DIV2']['prInfo']['value'] }}
-{{ data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}
-{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV2']['battleInfo']['avgInfo']
+{{ data['typeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['PVP_DIV2']['prInfo']['value'] }}
+{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']
 ['frags']) }}
-{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV2']['battleInfo']
-['hitRatioInfo']['ratioMain']) }}%
-{% endif %} {% if data['battleTypeInfo']['PVP_DIV3']['battle'] %}
+{% endif %} {% if data['typeInfo']['PVP_DIV3']['battle'] %}
 三轮车
-{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}
-{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%
-{{ data['battleTypeInfo']['PVP_DIV3']['prInfo']['value'] }}
-{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}
-{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']
+{{ data['typeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['PVP_DIV3']['prInfo']['value'] }}
+{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']
 ['frags']) }}
-{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']
-['hitRatioInfo']['ratioMain']) }}%
-{% endif %} {% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
+{% endif %} {% if data['typeInfo']['RANK_SOLO']['battle'] %}
 排位
-{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}
-{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%
-{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}
-{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}
-{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']
+{{ data['typeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }}
+{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']
 ['frags']) }}
-{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']
-['hitRatioInfo']['ratioMain']) }}%
 {% endif %}
-每日战绩
-类型
-场次
-胜率
-PR
-场均
+最高纪录
+最高伤害
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxDamageDealt']['value']
+}}
+侦察伤害
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxScoutingDamage']
+['value'] }}
+最高潜在
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxTotalAgro']['value'] }}
+经验
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxXp']['value'] }}
 击杀
-{% for eachShipData in data['shipInfoBattleList'] %} {% if eachShipData
-['typeInfo']['PVP']['battle'] or eachShipData['typeInfo']['RANK_SOLO']
-['battle'] %}
-{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData
-['recordDateTime']/1000)))) }}
-{% for each in eachShipData %} {% for index,value in enumerate(
-['shipSolo','shipTwo','shipThree','rankSolo']) %} {% if each|string == value
-and eachShipData[each]['battles'] %}
-{{ ['单野','自行车','三轮车','排位'][index] }}
-{{ eachShipData[each]['battles'] }}
-{{ eachShipData[each]['wins'] }}%
-{{ eachShipData[each]['pr']['value'] }}
-{{ eachShipData[each]['damage'] }}
-{{ '%.2f' | format(eachShipData[each]['frags']) }}
-{% endif %} {% endfor %} {% endfor %} {% endif %} {% endfor %}
-©西行寺雨季  ©本心
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxFrags']['value'] }}
+飞机击落
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxPlanesKilled']['value']
+}}
+© 西行寺雨季  © 本心
 QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~
 Design By 冷眠 H5 Converted By C1ystal
 赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说
```

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-sx.html` & `hikari_core-1.1.0/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/Template/wws-unban.html` & `hikari_core-1.1.0/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/hikari_core/utils.py` & `hikari_core-1.1.0/hikari_core/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/LICENSE` & `hikari_core-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-1.0.9.1/pyproject.toml` & `hikari_core-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "1.0.9.1"
+version = "1.1.0"
 description = "SDK for yuyuko,战舰世界yuyuko平台BOT SDK"
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 homepage = "https://github.com/wows-yuyuko/Hikari-core"
 repository = "https://github.com/wows-yuyuko/Hikari-core"
 keywords = ["qqbot", "wows", "wws","bot","stats"]
```

### Comparing `hikari_core-1.0.9.1/setup.py` & `hikari_core-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
  'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.40.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '1.0.9.1',
+    'version': '1.1.0',
     'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wows-yuyuko/Hikari-core',
```

### Comparing `hikari_core-1.0.9.1/PKG-INFO` & `hikari_core-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 1.0.9.1
+Version: 1.1.0
 Summary: SDK for yuyuko,战舰世界yuyuko平台BOT SDK
 Home-page: https://github.com/wows-yuyuko/Hikari-core
 Keywords: qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

