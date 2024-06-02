# Comparing `tmp/nonebot_plugin_chatgpt_turbo-0.3.0.tar.gz` & `tmp/nonebot_plugin_chatgpt_turbo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chatgpt_turbo-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_chatgpt_turbo-1.0.0.tar", max compression
```

## Comparing `nonebot_plugin_chatgpt_turbo-0.3.0.tar` & `nonebot_plugin_chatgpt_turbo-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,6 @@
--rw-r--r--   0        0        0     1979 2023-03-15 14:24:21.682820 nonebot_plugin_chatgpt_turbo-0.3.0/README.md
--rw-r--r--   0        0        0     1180 2023-03-20 14:37:11.310442 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-03-20 14:37:11.324724 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      185 2023-03-20 14:37:11.322453 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/misc.xml
--rw-r--r--   0        0        0      308 2023-03-20 14:37:11.319000 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/modules.xml
--rw-r--r--   0        0        0      284 2023-03-20 14:37:11.316095 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/nonebot_plugin_chatgpt_turbo.iml
--rw-r--r--   0        0        0      183 2023-03-20 14:37:11.327302 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/vcs.xml
--rw-r--r--   0        0        0     1996 2023-03-20 14:37:11.320009 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/.idea/workspace.xml
--rw-r--r--   0        0        0     1121 2023-03-23 06:45:53.930880 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/ChatSession.py
--rw-r--r--   0        0        0     4210 2023-03-27 02:11:34.479827 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/__init__.py
--rw-r--r--   0        0        0      465 2023-03-27 02:11:34.480225 nonebot_plugin_chatgpt_turbo-0.3.0/nonebot_plugin_chatgpt_turbo/config.py
--rw-r--r--   0        0        0      558 2023-03-27 02:11:34.481059 nonebot_plugin_chatgpt_turbo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 nonebot_plugin_chatgpt_turbo-0.3.0/setup.py
--rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 nonebot_plugin_chatgpt_turbo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1763 2024-06-02 13:05:53.160268 nonebot_plugin_chatgpt_turbo-1.0.0/README.md
+-rw-r--r--   0        0        0     6636 2024-06-02 13:06:48.022745 nonebot_plugin_chatgpt_turbo-1.0.0/nonebot_plugin_chatgpt_turbo/__init__.py
+-rw-r--r--   0        0        0      695 2024-06-02 12:45:55.314866 nonebot_plugin_chatgpt_turbo-1.0.0/nonebot_plugin_chatgpt_turbo/config.py
+-rw-r--r--   0        0        0      536 2024-06-02 13:07:15.016681 nonebot_plugin_chatgpt_turbo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 nonebot_plugin_chatgpt_turbo-1.0.0/setup.py
+-rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 nonebot_plugin_chatgpt_turbo-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_chatgpt_turbo-0.3.0/README.md` & `nonebot_plugin_chatgpt_turbo-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 
 <div align="center">
 
 # nonebot-plugin-chatgpt-turbo
 </div>
 
 # 介绍
-- 本插件适配OpenAI在2023年3月1日发布的最新版API，可以在nonebot中调用OpenAI的ChatGPT生产环境下的模型（GPT3.5-turbo）进行回复。
-- 接口调用速度与网络环境有关，经过测试，大陆外的服务器的OpenAI API响应时间能在十秒之内。
-- 免费版OpenAI的调用速度限制为20次/min
-- 本插件具有上下文回复功能(可选)，根据每个成员与机器人最近30条（可修改）的聊天记录进行响应回复,该功能消耗服务器资源较大
+- 本插件适配OneAPI和OpenAI接口，可以在nonebot中调用OpenAI官方或是OneAPI(gpt系列模型,gemini-1.5-pro)接口的模型进行回复。
+- 本插件具有上下文回复和多模态识别（识图）功能。
 # 安装
 
 * 手动安装
   ```
   git clone https://github.com/Alpaca4610/nonebot_plugin_chatgpt_turbo.git
   ```
 
@@ -32,24 +30,25 @@
   ```
 
 # 配置文件
 
 在Bot根目录下的.env文件中追加如下内容：
 
 ```
-OPENAI_API_KEY = key
-OPENAI_MODEL_NAME = "gpt-3.5-turbo"
-OPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 请使用代理访问api，中国大陆/香港IP调用API有几率会被封禁
+oneapi_key = ""  # OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY
+oneapi_model = "gpt-4o" # 使用的语言大模型，使用识图功能请填写合适的大模型名称
 ```
 
 可选内容：
 ```
-OPENAI_MAX_HISTORY_LIMIT = 30   # 保留与每个用户的聊天记录条数
-ENABLE_PRIVATE_CHAT = True   # 私聊开关，默认开启，改为False关闭
+oneapi_url = ""  # （可选）大模型中转服务商提供的中转地址，使用OpenAI官方服务不需要填写
+enable_private_chat = True   # 私聊开关，默认开启，改为False关闭
 ```
 
+# 效果
+![](demo.jpg)
 
 # 使用方法
 
 - @机器人发送问题时机器人不具有上下文回复的能力
 - chat 使用该命令进行问答时，机器人具有上下文回复的能力
 - clear 清除当前用户的聊天记录
```

#### html2text {}

```diff
@@ -1,27 +1,24 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-chatgpt-turbo
 # ä»ç» -
-æ¬æä»¶ééOpenAIå¨2023å¹´3æ1æ¥åå¸çææ°çAPIï¼å¯ä»¥å¨nonebotä¸­è°ç¨OpenAIçChatGPTçäº§ç¯å¢ä¸çæ¨¡åï¼GPT3.5-
-turboï¼è¿è¡åå¤ã -
-æ¥å£è°ç¨éåº¦ä¸ç½ç»ç¯å¢æå³ï¼ç»è¿æµè¯ï¼å¤§éå¤çæå¡å¨çOpenAI
-APIååºæ¶é´è½å¨åç§ä¹åã -
-åè´¹çOpenAIçè°ç¨éåº¦éå¶ä¸º20æ¬¡/min -
-æ¬æä»¶å·æä¸ä¸æåå¤åè½
-(å¯é)ï¼æ ¹æ®æ¯ä¸ªæåä¸æºå¨äººæè¿30æ¡ï¼å¯ä¿®æ¹ï¼çèå¤©è®°å½è¿è¡ååºåå¤,è¯¥åè½æ¶èæå¡å¨èµæºè¾å¤§
-# å®è£ * æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
+æ¬æä»¶ééOneAPIåOpenAIæ¥å£ï¼å¯ä»¥å¨nonebotä¸­è°ç¨OpenAIå®æ¹ææ¯OneAPI
+(gptç³»åæ¨¡å,gemini-1.5-pro)æ¥å£çæ¨¡åè¿è¡åå¤ã -
+æ¬æä»¶å·æä¸ä¸æåå¤åå¤æ¨¡æè¯å«ï¼è¯å¾ï¼åè½ã # å®è£
+* æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
 nonebot_plugin_chatgpt_turbo.git ```
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼ ```
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-gpt3.5-turbo"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-chatgpt-
 turbo ``` # éç½®æä»¶
-å¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼ ``` OPENAI_API_KEY =
-key OPENAI_MODEL_NAME = "gpt-3.5-turbo" OPENAI_HTTP_PROXY = "http://127.0.0.1:
-8001" # è¯·ä½¿ç¨ä»£çè®¿é®apiï¼ä¸­å½å¤§é/
-é¦æ¸¯IPè°ç¨APIæå çä¼è¢«å°ç¦ ``` å¯éåå®¹ï¼ ```
-OPENAI_MAX_HISTORY_LIMIT = 30 # ä¿çä¸æ¯ä¸ªç¨æ·çèå¤©è®°å½æ¡æ°
-ENABLE_PRIVATE_CHAT = True # ç§èå¼å³ï¼é»è®¤å¼å¯ï¼æ¹ä¸ºFalseå³é­
-``` # ä½¿ç¨æ¹æ³ -
+å¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼ ``` oneapi_key = "" #
+OpenAIå®æ¹æèæ¯æ¯æOneAPIçå¤§æ¨¡åä¸­è½¬æå¡åæä¾çKEY
+oneapi_model = "gpt-4o" #
+ä½¿ç¨çè¯­è¨å¤§æ¨¡åï¼ä½¿ç¨è¯å¾åè½è¯·å¡«ååéçå¤§æ¨¡ååç§°
+``` å¯éåå®¹ï¼ ``` oneapi_url = "" #
+ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°åï¼ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å
+enable_private_chat = True # ç§èå¼å³ï¼é»è®¤å¼å¯ï¼æ¹ä¸ºFalseå³é­
+``` # ææ ![](demo.jpg) # ä½¿ç¨æ¹æ³ -
 @æºå¨äººåéé®é¢æ¶æºå¨äººä¸å·æä¸ä¸æåå¤çè½å - chat
 ä½¿ç¨è¯¥å½ä»¤è¿è¡é®ç­æ¶ï¼æºå¨äººå·æä¸ä¸æåå¤çè½å -
 clear æ¸é¤å½åç¨æ·çèå¤©è®°å½
```

### Comparing `nonebot_plugin_chatgpt_turbo-0.3.0/pyproject.toml` & `nonebot_plugin_chatgpt_turbo-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-chatgpt-turbo"
-version = "0.3.0"
-description = "A nonebot plugin for openai gpt3.5-turbo"
+version = "1.0.0"
+description = "A nonebot plugin for oneapi and openai"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = "^2.2.1"
-openai = "^0.27.0"
-aiohttp = "^3.8.4"
+openai = "^1.30.5"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true 
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_chatgpt_turbo-0.3.0/setup.py` & `nonebot_plugin_chatgpt_turbo-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['nonebot_plugin_chatgpt_turbo']
 
 package_data = \
-{'': ['*'],
- 'nonebot_plugin_chatgpt_turbo': ['.idea/*', '.idea/inspectionProfiles/*']}
+{'': ['*']}
 
 install_requires = \
-['aiohttp>=3.8.4,<4.0.0',
- 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
+['nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
- 'openai>=0.27.0,<0.28.0']
+ 'openai>=1.30.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-chatgpt-turbo',
-    'version': '0.3.0',
-    'description': 'A nonebot plugin for openai gpt3.5-turbo',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-chatgpt-turbo\n</div>\n\n# 介绍\n- 本插件适配OpenAI在2023年3月1日发布的最新版API，可以在nonebot中调用OpenAI的ChatGPT生产环境下的模型（GPT3.5-turbo）进行回复。\n- 接口调用速度与网络环境有关，经过测试，大陆外的服务器的OpenAI API响应时间能在十秒之内。\n- 免费版OpenAI的调用速度限制为20次/min\n- 本插件具有上下文回复功能(可选)，根据每个成员与机器人最近30条（可修改）的聊天记录进行响应回复,该功能消耗服务器资源较大\n# 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_chatgpt_turbo.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-gpt3.5-turbo"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-chatgpt-turbo\n  ```\n\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n```\nOPENAI_API_KEY = key\nOPENAI_MODEL_NAME = "gpt-3.5-turbo"\nOPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 请使用代理访问api，中国大陆/香港IP调用API有几率会被封禁\n```\n\n可选内容：\n```\nOPENAI_MAX_HISTORY_LIMIT = 30   # 保留与每个用户的聊天记录条数\nENABLE_PRIVATE_CHAT = True   # 私聊开关，默认开启，改为False关闭\n```\n\n\n# 使用方法\n\n- @机器人发送问题时机器人不具有上下文回复的能力\n- chat 使用该命令进行问答时，机器人具有上下文回复的能力\n- clear 清除当前用户的聊天记录\n',
+    'version': '1.0.0',
+    'description': 'A nonebot plugin for oneapi and openai',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-chatgpt-turbo\n</div>\n\n# 介绍\n- 本插件适配OneAPI和OpenAI接口，可以在nonebot中调用OpenAI官方或是OneAPI(gpt系列模型,gemini-1.5-pro)接口的模型进行回复。\n- 本插件具有上下文回复和多模态识别（识图）功能。\n# 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_chatgpt_turbo.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-gpt3.5-turbo"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-chatgpt-turbo\n  ```\n\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n```\noneapi_key = ""  # OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\noneapi_model = "gpt-4o" # 使用的语言大模型，使用识图功能请填写合适的大模型名称\n```\n\n可选内容：\n```\noneapi_url = ""  # （可选）大模型中转服务商提供的中转地址，使用OpenAI官方服务不需要填写\nenable_private_chat = True   # 私聊开关，默认开启，改为False关闭\n```\n\n# 效果\n![](demo.jpg)\n\n# 使用方法\n\n- @机器人发送问题时机器人不具有上下文回复的能力\n- chat 使用该命令进行问答时，机器人具有上下文回复的能力\n- clear 清除当前用户的聊天记录\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,40 +1,37 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_chatgpt_turbo'] package_data = \ {'': ['*'],
-'nonebot_plugin_chatgpt_turbo': ['.idea/*', '.idea/inspectionProfiles/*']}
-install_requires = \ ['aiohttp>=3.8.4,<4.0.0', 'nonebot-adapter-
-onebot>=2.2.1,<3.0.0', 'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=0.27.0,<0.28.0']
-setup_kwargs = { 'name': 'nonebot-plugin-chatgpt-turbo', 'version': '0.3.0',
-'description': 'A nonebot plugin for openai gpt3.5-turbo', 'long_description':
-'
+['nonebot_plugin_chatgpt_turbo'] package_data = \ {'': ['*']} install_requires
+= \ ['nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot2>=2.0.0rc3,<3.0.0',
+'openai>=1.30.5,<2.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-chatgpt-
+turbo', 'version': '1.0.0', 'description': 'A nonebot plugin for oneapi and
+openai', 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
                      \n\n# nonebot-plugin-chatgpt-turbo\n
 \n\n# ä»ç»\n-
-æ¬æä»¶ééOpenAIå¨2023å¹´3æ1æ¥åå¸çææ°çAPIï¼å¯ä»¥å¨nonebotä¸­è°ç¨OpenAIçChatGPTçäº§ç¯å¢ä¸çæ¨¡åï¼GPT3.5-
-turboï¼è¿è¡åå¤ã\n-
-æ¥å£è°ç¨éåº¦ä¸ç½ç»ç¯å¢æå³ï¼ç»è¿æµè¯ï¼å¤§éå¤çæå¡å¨çOpenAI
-APIååºæ¶é´è½å¨åç§ä¹åã\n-
-åè´¹çOpenAIçè°ç¨éåº¦éå¶ä¸º20æ¬¡/min\n-
-æ¬æä»¶å·æä¸ä¸æåå¤åè½
-(å¯é)ï¼æ ¹æ®æ¯ä¸ªæåä¸æºå¨äººæè¿30æ¡ï¼å¯ä¿®æ¹ï¼çèå¤©è®°å½è¿è¡ååºåå¤,è¯¥åè½æ¶èæå¡å¨èµæºè¾å¤§\n#
+æ¬æä»¶ééOneAPIåOpenAIæ¥å£ï¼å¯ä»¥å¨nonebotä¸­è°ç¨OpenAIå®æ¹ææ¯OneAPI
+(gptç³»åæ¨¡å,gemini-1.5-pro)æ¥å£çæ¨¡åè¿è¡åå¤ã\n-
+æ¬æä»¶å·æä¸ä¸æåå¤åå¤æ¨¡æè¯å«ï¼è¯å¾ï¼åè½ã\n#
 å®è£\n\n* æå¨å®è£\n ```\n git clone https://github.com/Alpaca4610/
 nonebot_plugin_chatgpt_turbo.git\n ```\n\n
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼\n\n
 ```\n plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/
 nonebot-plugin-gpt3.5-turbo"]\n ```\n* ä½¿ç¨ pip\n ```\n pip install nonebot-
 plugin-chatgpt-turbo\n ```\n\n#
-éç½®æä»¶\n\nå¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼\n\n```\nOPENAI_API_KEY
-= key\nOPENAI_MODEL_NAME = "gpt-3.5-turbo"\nOPENAI_HTTP_PROXY = "http://
-127.0.0.1:8001" # è¯·ä½¿ç¨ä»£çè®¿é®apiï¼ä¸­å½å¤§é/
-é¦æ¸¯IPè°ç¨APIæå çä¼è¢«å°ç¦\n```\n\nå¯éåå®¹ï¼\n```\nOPENAI_MAX_HISTORY_LIMIT
-= 30 # ä¿çä¸æ¯ä¸ªç¨æ·çèå¤©è®°å½æ¡æ°\nENABLE_PRIVATE_CHAT = True #
-ç§èå¼å³ï¼é»è®¤å¼å¯ï¼æ¹ä¸ºFalseå³é­\n```\n\n\n# ä½¿ç¨æ¹æ³\n\n-
+éç½®æä»¶\n\nå¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼\n\n```\noneapi_key
+= "" #
+OpenAIå®æ¹æèæ¯æ¯æOneAPIçå¤§æ¨¡åä¸­è½¬æå¡åæä¾çKEY\noneapi_model
+= "gpt-4o" #
+ä½¿ç¨çè¯­è¨å¤§æ¨¡åï¼ä½¿ç¨è¯å¾åè½è¯·å¡«ååéçå¤§æ¨¡ååç§°\n```\n\nå¯éåå®¹ï¼\n```\noneapi_url
+= "" #
+ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°åï¼ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å\nenable_private_chat
+= True # ç§èå¼å³ï¼é»è®¤å¼å¯ï¼æ¹ä¸ºFalseå³é­\n```\n\n# ææ\n![]
+(demo.jpg)\n\n# ä½¿ç¨æ¹æ³\n\n-
 @æºå¨äººåéé®é¢æ¶æºå¨äººä¸å·æä¸ä¸æåå¤çè½å\n- chat
 ä½¿ç¨è¯¥å½ä»¤è¿è¡é®ç­æ¶ï¼æºå¨äººå·æä¸ä¸æåå¤çè½å\n-
 clear æ¸é¤å½åç¨æ·çèå¤©è®°å½\n', 'author': 'Alpaca', 'author_email':
 'alpaca@bupt.edu.cn', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
 'None', 'packages': packages, 'package_data': package_data, 'install_requires':
 install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_chatgpt_turbo-0.3.0/PKG-INFO` & `nonebot_plugin_chatgpt_turbo-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-turbo
-Version: 0.3.0
-Summary: A nonebot plugin for openai gpt3.5-turbo
+Version: 1.0.0
+Summary: A nonebot plugin for oneapi and openai
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
-Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: openai (>=1.30.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-chatgpt-turbo
 </div>
 
 # 介绍
-- 本插件适配OpenAI在2023年3月1日发布的最新版API，可以在nonebot中调用OpenAI的ChatGPT生产环境下的模型（GPT3.5-turbo）进行回复。
-- 接口调用速度与网络环境有关，经过测试，大陆外的服务器的OpenAI API响应时间能在十秒之内。
-- 免费版OpenAI的调用速度限制为20次/min
-- 本插件具有上下文回复功能(可选)，根据每个成员与机器人最近30条（可修改）的聊天记录进行响应回复,该功能消耗服务器资源较大
+- 本插件适配OneAPI和OpenAI接口，可以在nonebot中调用OpenAI官方或是OneAPI(gpt系列模型,gemini-1.5-pro)接口的模型进行回复。
+- 本插件具有上下文回复和多模态识别（识图）功能。
 # 安装
 
 * 手动安装
   ```
   git clone https://github.com/Alpaca4610/nonebot_plugin_chatgpt_turbo.git
   ```
 
@@ -52,25 +49,26 @@
   ```
 
 # 配置文件
 
 在Bot根目录下的.env文件中追加如下内容：
 
 ```
-OPENAI_API_KEY = key
-OPENAI_MODEL_NAME = "gpt-3.5-turbo"
-OPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 请使用代理访问api，中国大陆/香港IP调用API有几率会被封禁
+oneapi_key = ""  # OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY
+oneapi_model = "gpt-4o" # 使用的语言大模型，使用识图功能请填写合适的大模型名称
 ```
 
 可选内容：
 ```
-OPENAI_MAX_HISTORY_LIMIT = 30   # 保留与每个用户的聊天记录条数
-ENABLE_PRIVATE_CHAT = True   # 私聊开关，默认开启，改为False关闭
+oneapi_url = ""  # （可选）大模型中转服务商提供的中转地址，使用OpenAI官方服务不需要填写
+enable_private_chat = True   # 私聊开关，默认开启，改为False关闭
 ```
 
+# 效果
+![](demo.jpg)
 
 # 使用方法
 
 - @机器人发送问题时机器人不具有上下文回复的能力
 - chat 使用该命令进行问答时，机器人具有上下文回复的能力
 - clear 清除当前用户的聊天记录
```

#### html2text {}

```diff
@@ -1,37 +1,34 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-turbo Version: 0.3.0
-Summary: A nonebot plugin for openai gpt3.5-turbo License: MIT Author: Alpaca
+Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-turbo Version: 1.0.0
+Summary: A nonebot plugin for oneapi and openai License: MIT Author: Alpaca
 Author-email: alpaca@bupt.edu.cn Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Requires-Dist:
-openai (>=0.27.0,<0.28.0) Description-Content-Type: text/markdown
+Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0rc3,<3.0.0) Requires-Dist: openai (>=1.30.5,<2.0.0) Description-
+Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-chatgpt-turbo
 # ä»ç» -
-æ¬æä»¶ééOpenAIå¨2023å¹´3æ1æ¥åå¸çææ°çAPIï¼å¯ä»¥å¨nonebotä¸­è°ç¨OpenAIçChatGPTçäº§ç¯å¢ä¸çæ¨¡åï¼GPT3.5-
-turboï¼è¿è¡åå¤ã -
-æ¥å£è°ç¨éåº¦ä¸ç½ç»ç¯å¢æå³ï¼ç»è¿æµè¯ï¼å¤§éå¤çæå¡å¨çOpenAI
-APIååºæ¶é´è½å¨åç§ä¹åã -
-åè´¹çOpenAIçè°ç¨éåº¦éå¶ä¸º20æ¬¡/min -
-æ¬æä»¶å·æä¸ä¸æåå¤åè½
-(å¯é)ï¼æ ¹æ®æ¯ä¸ªæåä¸æºå¨äººæè¿30æ¡ï¼å¯ä¿®æ¹ï¼çèå¤©è®°å½è¿è¡ååºåå¤,è¯¥åè½æ¶èæå¡å¨èµæºè¾å¤§
-# å®è£ * æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
+æ¬æä»¶ééOneAPIåOpenAIæ¥å£ï¼å¯ä»¥å¨nonebotä¸­è°ç¨OpenAIå®æ¹ææ¯OneAPI
+(gptç³»åæ¨¡å,gemini-1.5-pro)æ¥å£çæ¨¡åè¿è¡åå¤ã -
+æ¬æä»¶å·æä¸ä¸æåå¤åå¤æ¨¡æè¯å«ï¼è¯å¾ï¼åè½ã # å®è£
+* æå¨å®è£ ``` git clone https://github.com/Alpaca4610/
 nonebot_plugin_chatgpt_turbo.git ```
 ä¸è½½å®æåå¨boté¡¹ç®çpyproject.tomlæä»¶æå¨æ·»å æä»¶ï¼ ```
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-gpt3.5-turbo"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-chatgpt-
 turbo ``` # éç½®æä»¶
-å¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼ ``` OPENAI_API_KEY =
-key OPENAI_MODEL_NAME = "gpt-3.5-turbo" OPENAI_HTTP_PROXY = "http://127.0.0.1:
-8001" # è¯·ä½¿ç¨ä»£çè®¿é®apiï¼ä¸­å½å¤§é/
-é¦æ¸¯IPè°ç¨APIæå çä¼è¢«å°ç¦ ``` å¯éåå®¹ï¼ ```
-OPENAI_MAX_HISTORY_LIMIT = 30 # ä¿çä¸æ¯ä¸ªç¨æ·çèå¤©è®°å½æ¡æ°
-ENABLE_PRIVATE_CHAT = True # ç§èå¼å³ï¼é»è®¤å¼å¯ï¼æ¹ä¸ºFalseå³é­
-``` # ä½¿ç¨æ¹æ³ -
+å¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼ ``` oneapi_key = "" #
+OpenAIå®æ¹æèæ¯æ¯æOneAPIçå¤§æ¨¡åä¸­è½¬æå¡åæä¾çKEY
+oneapi_model = "gpt-4o" #
+ä½¿ç¨çè¯­è¨å¤§æ¨¡åï¼ä½¿ç¨è¯å¾åè½è¯·å¡«ååéçå¤§æ¨¡ååç§°
+``` å¯éåå®¹ï¼ ``` oneapi_url = "" #
+ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°åï¼ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å
+enable_private_chat = True # ç§èå¼å³ï¼é»è®¤å¼å¯ï¼æ¹ä¸ºFalseå³é­
+``` # ææ ![](demo.jpg) # ä½¿ç¨æ¹æ³ -
 @æºå¨äººåéé®é¢æ¶æºå¨äººä¸å·æä¸ä¸æåå¤çè½å - chat
 ä½¿ç¨è¯¥å½ä»¤è¿è¡é®ç­æ¶ï¼æºå¨äººå·æä¸ä¸æåå¤çè½å -
 clear æ¸é¤å½åç¨æ·çèå¤©è®°å½
```

