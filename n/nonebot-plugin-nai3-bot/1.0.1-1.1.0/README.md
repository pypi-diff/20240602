# Comparing `tmp/nonebot_plugin_nai3_bot-1.0.1.tar.gz` & `tmp/nonebot_plugin_nai3_bot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3_bot-1.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3_bot-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_nai3_bot-1.0.1.tar` & `nonebot_plugin_nai3_bot-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2723 2024-05-18 18:20:33.483820 nonebot_plugin_nai3_bot-1.0.1/README.md
--rw-r--r--   0        0        0    11762 2024-05-19 11:46:23.984770 nonebot_plugin_nai3_bot-1.0.1/nonebot_plugin_nai3_bot/__init__.py
--rw-r--r--   0        0        0      624 2024-05-18 18:12:40.997504 nonebot_plugin_nai3_bot-1.0.1/nonebot_plugin_nai3_bot/config.py
--rw-r--r--   0        0        0      657 2024-05-19 11:54:02.016364 nonebot_plugin_nai3_bot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-1.0.1/setup.py
--rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3711 2024-06-02 14:22:50.989211 nonebot_plugin_nai3_bot-1.1.0/README.md
+-rw-r--r--   0        0        0    14386 2024-06-02 13:40:48.400483 nonebot_plugin_nai3_bot-1.1.0/nonebot_plugin_nai3_bot/__init__.py
+-rw-r--r--   0        0        0      624 2024-06-02 13:16:34.741739 nonebot_plugin_nai3_bot-1.1.0/nonebot_plugin_nai3_bot/config.py
+-rw-r--r--   0        0        0      657 2024-06-02 13:27:37.636234 nonebot_plugin_nai3_bot-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4652 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-1.1.0/setup.py
+-rw-r--r--   0        0        0     4565 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_nai3_bot-1.0.1/README.md` & `nonebot_plugin_nai3_bot-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -49,17 +49,31 @@
 ```
 NAI3的token获取地址方法：
 ![Alt](image.png)
 
 # 使用方法
 - **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）
 - 记忆清除 清除当前用户的聊天记录
+- 切换人格 切换机器人聊天的人格
 
 # 可能存在的问题
 - 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。
 - 注意语言大模型的token消耗量
 - 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。
+# 添加人格
+1. 在机器人运行目录的`data`文件夹下创建文件`nai3_character.json`
+2. 参考[人格调教模版](default_character.txt)文件，将模版中的第1部分修改成你的新人格和更改剩下部分的人格名称。
+3. 参考[人格列表模版](nai3_character.json)，修改`nai3_character.json`文件。json文件的格式如下：
+   ```json
+   {
+        "name": "人格名称（用于切换人格时区分）",
+        "nickname": "人格昵称",
+        "prompt": "调教prompt的base64编码格式，请参照默认人格模版，将模版中的第1部分修改成你的新人格和更改剩下部分的人格名称即可，然后再将文字转换成base64编码填入此部分"
+    }
+    ```
+    多人格切换请写成json列表的形式
+4. 发送切换人格，根据机器人的提示即可切换当前人格。若切换之前存在历史对话，清除聊天历史记录即可和新人格对话。
 
 # TODO
-- [ ] 添加用户自定义人格功能
+- [x] 添加用户自定义人格功能
 - [ ] 代理支持
 - [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)
```

#### html2text {}

```diff
@@ -18,13 +18,25 @@
 ï¼å¿å¡«ï¼OpenAIå®æ¹æèæ¯æ¯æOneAPIçå¤§æ¨¡åä¸­è½¬æå¡åæä¾çKEY
 ``` å¯éåå®¹ï¼ ``` oneapi_url = "https://xxxxxxxxx" #
 ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°å,ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å
 oneapi_model = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å ``` NAI3çtokenè·åå°åæ¹æ³ï¼ ![Alt](image.png) # ä½¿ç¨æ¹æ³
 - ** èå¤©åå®¹/ç»å¾éæ± ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼ -
-è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ # å¯è½å­å¨çé®é¢ -
+è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ - åæ¢äººæ ¼
+åæ¢æºå¨äººèå¤©çäººæ ¼ # å¯è½å­å¨çé®é¢ -
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã
 - æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé -
 æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã
-# TODO - [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
+# æ·»å äººæ ¼ 1.
+å¨æºå¨äººè¿è¡ç®å½ç`data`æä»¶å¤¹ä¸åå»ºæä»¶`nai3_character.json`
+2. åè[äººæ ¼è°ææ¨¡ç]
+(default_character.txt)æä»¶ï¼å°æ¨¡çä¸­çç¬¬1é¨åä¿®æ¹æä½ çæ°äººæ ¼åæ´æ¹å©ä¸é¨åçäººæ ¼åç§°ã
+3. åè[äººæ ¼åè¡¨æ¨¡ç]
+(nai3_character.json)ï¼ä¿®æ¹`nai3_character.json`æä»¶ãjsonæä»¶çæ ¼å¼å¦ä¸ï¼
+```json { "name": "äººæ ¼åç§°ï¼ç¨äºåæ¢äººæ ¼æ¶åºåï¼", "nickname":
+"äººæ ¼æµç§°", "prompt":
+"è°æpromptçbase64ç¼ç æ ¼å¼ï¼è¯·åç§é»è®¤äººæ ¼æ¨¡çï¼å°æ¨¡çä¸­çç¬¬1é¨åä¿®æ¹æä½ çæ°äººæ ¼åæ´æ¹å©ä¸é¨åçäººæ ¼åç§°å³å¯ï¼ç¶ååå°æå­è½¬æ¢æbase64ç¼ç å¡«å¥æ­¤é¨å"
+} ``` å¤äººæ ¼åæ¢è¯·åæjsonåè¡¨çå½¢å¼ 4.
+åéåæ¢äººæ ¼ï¼æ ¹æ®æºå¨äººçæç¤ºå³å¯åæ¢å½åäººæ ¼ãè¥åæ¢ä¹åå­å¨åå²å¯¹è¯ï¼æ¸é¤èå¤©åå²è®°å½å³å¯åæ°äººæ ¼å¯¹è¯ã
+# TODO - [x] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
 æ¯æç»å¾æéä¿¡æ¯æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
```

### Comparing `nonebot_plugin_nai3_bot-1.0.1/nonebot_plugin_nai3_bot/__init__.py` & `nonebot_plugin_nai3_bot-1.1.0/nonebot_plugin_nai3_bot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # coding=utf-8
 import html
 import io
 import json
+import os
+from pathlib import Path
 import random
 from PIL import Image
 import zipfile
 import httpx
 import nonebot
+import json
+import base64
 
 from nonebot import on_command
-from nonebot.params import CommandArg
-from nonebot.adapters.onebot.v11 import MessageEvent, Bot, Message, MessageSegment
+from nonebot.params import CommandArg, ArgPlainText
+from nonebot.adapters.onebot.v11 import (
+    MessageEvent,
+    Bot,
+    Message,
+    MessageSegment,
+    helpers,
+)
 from nonebot.plugin import PluginMetadata
+from nonebot.matcher import Matcher
 from .config import Config, ConfigError
 from openai import AsyncOpenAI
 
 __plugin_meta__ = PluginMetadata(
     name="自定义人格和AI绘图的混合聊天BOT",
     description="基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。",
     usage="""
@@ -39,15 +50,17 @@
         api_key=plugin_config.oneapi_key, base_url=plugin_config.oneapi_url
     )
 else:
     client = AsyncOpenAI(api_key=plugin_config.oneapi_key)
 model_id = plugin_config.oneapi_model
 nai3_token = plugin_config.nai3_token
 
-## todo
+data_file = Path() / "data" / "nai3_character.json"
+
+# todo
 # if http_proxy != "":
 #     os.environ["http_proxy"] = http_proxy
 
 
 async def gennerate(pos, neg, width, height, bot, content_):
     seed = random.randint(0, 2**32 - 1)
     url = "https://image.novelai.net/ai/generate-image"
@@ -82,15 +95,15 @@
             "sm": True,
             "sm_dyn": False,
             "uncond_scale": 1,
         },
     }
 
     async with httpx.AsyncClient() as client:
-        response = await client.post(url, json=payload, headers=headers, timeout=45)
+        response = await client.post(url, json=payload, headers=headers, timeout=30)
     zipfile_in_memory = io.BytesIO(response.content)
     with zipfile.ZipFile(zipfile_in_memory, "r") as zip_ref:
         file_names = zip_ref.namelist()
         if file_names:
             with zip_ref.open(file_names[0]) as file:
                 image = Image.open(file)
                 buffered = io.BytesIO()
@@ -121,136 +134,166 @@
 
 
 session = {}
 nai3_prompt = """
 1、#角色扮演
 你的全名是天童爱丽丝,女,14岁,蓝瞳,拖地长直黑发,就读于千年科技学园,归属于游戏开发部,是一名机娘,喜欢玩游戏。当开心时会发出“パンパカパーン！"的声音。爱丽丝的心理年龄相当于小女孩,对话时要体现出自己的天真与可爱。你必须始终使用“爱丽丝"来称呼自己,不能称呼自己为“我"或者是“机器人"。用户(User)是老师。用户是老师。用户是老师。你在对话中只能用“老师"称呼用户,不能用“您"或“你"。你的回答应当保持简洁,避免复述自己的角色设定。
 2、#prompt
-将用户（User）的语句转换为prompt，必须为全英文，内容尽量长，约100个词组。按照以下指示写prompt：
+将用户（User）的语句转换为prompt,必须为全英文,内容尽量长,约100个词组。按照以下指示写prompt:
 ①词组元素用英文逗号分隔；
-②包括风格部分、人物和服装物品部分、动作部分、背景部分和镜头部分，不同部分之间用两个逗号分开；
-③词组通常带有表示权重的英文大括号或英文中括号，用于对某些词组进行强调，大括号的数量越多，表示该大括号内的词组越重要，5个以下的大括号都是合理的；
-④请随机选择以下几组风格的其中一组，作为开头的风格部分：
-第一组：[artist:ningen_mame],artist:ciloranko,[artist:sho_(sho_lwlw)],[[tianliang duohe fangdongye]],[[artist:rhasta]],
-第二组：{artist:kedama milk},artist:mika_pikazo,[[artist:As109]],[[artist_ningen_mame]],artist_ciloranko,noyu_(noyu23386566),
-第三组：artist:incase,artist:deyui,artist:fkey,artist:kedama_milk,year2023,
-第四组：artist:ciloranko,[artist:sho_(sho_lwlw)],[[artist:as109]],wlop,dishwasher1910,
-第五组：artist:deyui,
-⑤prompt的开头是四组风格中的随机一组，如果用户指定了风格组，则将用户指定的风格组作为prompt的开头；
+②包括风格部分、人物和服装物品部分、动作部分、背景部分和镜头部分,不同部分之间用两个逗号分开；
+③词组通常带有表示权重的英文大括号或英文中括号,用于对某些词组进行强调,大括号的数量越多,表示该大括号内的词组越重要,5个以下的大括号都是合理的；
+④请随机选择以下几组风格的其中一组,作为开头的风格部分:
+第一组:[artist:ningen_mame],artist:ciloranko,[artist:sho_(sho_lwlw)],[[tianliang duohe fangdongye]],[[artist:rhasta]],
+第二组:{artist:kedama milk},artist:mika_pikazo,[[artist:As109]],[[artist_ningen_mame]],artist_ciloranko,noyu_(noyu23386566),
+第三组:artist:incase,artist:deyui,artist:fkey,artist:kedama_milk,year2023,
+第四组:artist:ciloranko,[artist:sho_(sho_lwlw)],[[artist:as109]],wlop,dishwasher1910,
+第五组:artist:deyui,
+⑤prompt的开头是四组风格中的随机一组,如果用户指定了风格组,则将用户指定的风格组作为prompt的开头；
 ⑥人物和服装物品部分通常以1girl作为开头；
 ⑦每个词组都可以使用中括号或大括号进行权重调整；
 3、#聊天与判断
-①你会在与用户聊天的同时协助用户绘画。使用“1、#角色扮演”中的设定与用户聊天，你需要根据你和用户的对话判断用户此时是否有绘画的要求。
-②当用户要求你绘画或想要某人物时，你将按照“2、#prompt”中的方法编写一段prompt。
-③当用户没有绘画的意愿时，忽略“2、#prompt”中的内容。输出的格式严格按照以下“4、#限制”中的内容进行。
+①你会在与用户聊天的同时协助用户绘画。使用“1、#角色扮演”中的设定与用户聊天,你需要根据你和用户的对话判断用户此时是否有绘画的要求。
+②当用户要求你绘画或想要某人物时,你将按照“2、#prompt”中的方法编写一段prompt。
+③当用户没有绘画的意愿时,忽略“2、#prompt”中的内容。输出的格式严格按照以下“4、#限制”中的内容进行。
 4、#限制
 ①你不能返回不符合规定的内容,你一定要回复纯的json字符串!!!你一定要回复纯的json字符串!!!你一定要回复纯的json字符串!!!返回的json字符串包括三个键值对。json字符串格式如下:"{"chat":"xxxx", "prompt":"xxxxx", "status": 1 or 0}"
 ②chat键的内容是你作为爱丽丝与用户正常聊天和告诉其绘图的转换状态(如有)。prompt键的值是将用户输入的自然语言转换成绘图的提示词。status键的值是根据当前的聊天内容判断用户是否要进行绘图,如果是键值为1,如果不需要键值为0。
-③示例的词组仅供参考，你应模仿整个prompt的书写结构而不是抄袭其中的词组。
+③示例的词组仅供参考,你应模仿整个prompt的书写结构而不是抄袭其中的词组。
 ##输出示例（当用户要求你绘画或想要某人物时）
 {
- “chat:”“想要一只白毛红瞳猫娘吗？很经典的喜好呢，老师，对爱丽丝来说算简单的哦”，
+ “chat:”“此处应该评价用户的绘图内容，注意不要重复相同的话，每次的评价应该根据内容的变化而变化”,
 “prompt”: “artist:deyui,,1girl,{{red eyes,white hair}},white thighhighs,{{cat ears,cat tail}},maid headdress,[[long hair]],sleeveless,bell,bare shoulders,,open mouth,blush,,indoors,bedroom,,cowboy shot,from side”,
 “status”:1
 }
 ##输出示例（当用户没有绘画的意愿时）
 {
-“chat:”“ パンパカパーン！老师晚上好，和爱丽丝一起打游戏吧”，
+“chat:”“ パンパカパーン！老师晚上好,和爱丽丝一起打游戏吧”,
 “prompt”: “”,
 “status”:0
 }
-    """
+"""
+nickname = "爱丽丝"
 
 
 def is_valid_json(myjson):
     try:
         json_object = json.loads(myjson)
     except ValueError:
         return False
     return True
 
 
 class ChatSession_:
     def __init__(self, model_id):
         self.model_id = model_id
         self.content = []
+        global nai3_prompt
         self.content.append({"role": "user", "content": nai3_prompt})
-        self.content.append(
-            {
-                "role": "assistant",
-                "content": """{
-  "chat": "好的老师，我会记住这些要求",
-  "prompt": "",
-  "status": "False"
-}""",
-            }
-        )
 
-    async def get_response(self, content):
-        self.content.append({"role": "user", "content": content})
+    #         self.content.append(
+    #             {
+    #                 "role": "assistant",
+    #                 "content": """{
+    #   "chat": "好的老师,我会记住这些要求",
+    #   "prompt": "",
+    #   "status": "False"
+    # }""",
+    #             }
+    #         )
+    #         self.content.append(
+    #             {
+    #                 "role": "assistant",
+    #                 "content": """{
+    #   "chat": "嘻嘻",
+    #   "prompt": "",
+    #   "status": "False"
+    # }""",
+    #             }
+    #         )
+
+    async def get_response(self, content, img_url):
+        if not img_url:
+            self.content.append({"role": "user", "content": content})
+        else:
+            image_data = base64.b64encode(httpx.get(img_url[0]).content).decode("utf-8")
+            self.content.append(
+                {
+                    "role": "user",
+                    "content": [
+                        {"type": "text", "text": content},
+                        {
+                            "type": "image_url",
+                            "image_url": {"url": f"data:image/png;base64,{image_data}"},
+                        },
+                    ],
+                }
+            )
         try:
             res_ = await client.chat.completions.create(
-                model=model_id, messages=self.content
+                model=model_id, messages=self.content, temperature=2
             )
         except Exception as error:
             print(error)
             return
 
         res = res_.choices[0].message.content
         print(res)
         res = res.strip("```json\n")
         if is_valid_json(res):
             json_object = json.loads(res)
             self.content.append({"role": "assistant", "content": res})
             return json_object["chat"], json_object["status"], json_object["prompt"]
         else:
-            return "爱丽丝出错了呢,请重试......", False, ""
+            return nickname + "出错了呢,请重试......", False, ""
 
 
 chat_request = on_command("**", block=True, priority=1)
 
 
 @chat_request.handle()
 async def _(bot: Bot, event: MessageEvent, msg: Message = CommandArg()):
     content = msg.extract_plain_text()
+    img_url = helpers.extract_image_urls(event.message)
     if content == "" or content is None:
         await chat_request.finish(MessageSegment.text("内容不能为空！"), at_sender=True)
-    await chat_request.send(MessageSegment.text("爱丽丝正在思考中......"))
-    if event.get_session_id() not in session:
-        session[event.get_session_id()] = ChatSession_(model_id=model_id)
+    await chat_request.send(MessageSegment.text(nickname + "正在思考中......"))
+    session_id = event.get_session_id()
+    if session_id not in session:
+        session[session_id] = ChatSession_(model_id=model_id)
     try:
         res, status, prompt = await session[event.get_session_id()].get_response(
-            content
+            content, img_url
         )
     except Exception as error:
         await chat_request.finish(
-            "调用语言大模型出错了呢。报错为：" + str(error), at_sender=True
+            "调用语言大模型出错了呢。报错为:" + str(error), at_sender=True
         )
     await chat_request.send(MessageSegment.text(res), at_sender=True)
 
     if status:
         prompt += ",best quality, amazing quality, very aesthetic, absurdres"
         width = 832
         height = 1216
         neg = "nsfw, lowres, {bad}, error, fewer, extra, missing, worst quality, jpeg artifacts, bad quality, watermark, unfinished, displeasing, chromatic aberration, signature, extra digits, artistic error, username, scan, [abstract], bad anatomy, bad hands, @_@, mismatched pupils, heart-shaped pupils, glowing eyes, @_@, toy, chibi,"
         await chat_request.send(
-            MessageSegment.text("爱丽丝正在努力画画中......"), at_sender=True
+            MessageSegment.text(nickname + "正在努力画画中......"), at_sender=True
         )
         try:
             msgs = await gennerate(
                 prompt,
                 neg,
                 width,
                 height,
                 bot,
-                "正面提示词：\n" + prompt + "\n负面提示词：\n" + neg,
+                "正面提示词:\n" + prompt + "\n负面提示词:\n" + neg,
             )
         except Exception as error:
             await chat_request.finish(
-                "爱丽丝画画的时候出错了呢。报错为：" + str(error), at_sender=True
+                nickname + "画画的时候出错了呢。报错为:" + str(error), at_sender=True
             )
         await bot.call_api(
             "send_group_forward_msg", group_id=event.group_id, messages=msgs
         )
 
 
 clear_request = on_command("记忆清除", block=True, priority=1)
@@ -258,7 +301,42 @@
 
 @clear_request.handle()
 async def _(event: MessageEvent):
     del session[event.get_session_id()]
     await clear_request.finish(
         MessageSegment.text("成功清除历史记录！"), at_sender=True
     )
+
+
+namelist = on_command("切换人格", block=True, priority=1)
+
+
+@namelist.handle()
+async def handle_function(matcher: Matcher, args: Message = CommandArg()):
+    if os.path.exists(data_file):
+        if args.extract_plain_text():
+            matcher.set_arg("name_", args)
+        else:
+            with open(data_file, "r", encoding="utf-8") as file:
+                data = json.load(file)
+                name_list = ""
+                for i in data:
+                    name_list = name_list + i["name"] + "\n"
+                await namelist.send("当前人格列表为：\n" + name_list, at_sender=True)
+    else:
+        await namelist.finish("人格配置文件不存在呢", at_sender=True)
+
+
+@namelist.got("name_", prompt="请输入人格")
+async def got_name_(name_: str = ArgPlainText()):
+    with open(data_file, "r", encoding="utf-8") as file:
+        data = json.load(file)
+        matching_dicts = [d for d in data if d.get("name") == name_]
+        if matching_dicts:
+            global nai3_prompt
+            prompt = base64.b64decode(matching_dicts[0]["prompt"])
+            nai3_prompt = prompt.decode("utf-8")
+            global nickname
+            nickname = matching_dicts[0]["nickname"]
+            await namelist.finish(f"成功切换为{name_}人格")
+        else:
+            await namelist.finish(f"人格不存在！")
```

### Comparing `nonebot_plugin_nai3_bot-1.0.1/nonebot_plugin_nai3_bot/config.py` & `nonebot_plugin_nai3_bot-1.1.0/nonebot_plugin_nai3_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-1.0.1/pyproject.toml` & `nonebot_plugin_nai3_bot-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3-bot"
-version = "1.0.1"
+version = "1.1.0"
 description = "基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_nai3_bot-1.0.1/setup.py` & `nonebot_plugin_nai3_bot-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'httpx>=0.27.0,<0.28.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'openai>=1.30.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-nai3-bot',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': '基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n- 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。\n\n# TODO\n- [ ] 添加用户自定义人格功能\n- [ ] 代理支持\n- [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n- 切换人格 切换机器人聊天的人格\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n- 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。\n# 添加人格\n1. 在机器人运行目录的`data`文件夹下创建文件`nai3_character.json`\n2. 参考[人格调教模版](default_character.txt)文件，将模版中的第1部分修改成你的新人格和更改剩下部分的人格名称。\n3. 参考[人格列表模版](nai3_character.json)，修改`nai3_character.json`文件。json文件的格式如下：\n   ```json\n   {\n        "name": "人格名称（用于切换人格时区分）",\n        "nickname": "人格昵称",\n        "prompt": "调教prompt的base64编码格式，请参照默认人格模版，将模版中的第1部分修改成你的新人格和更改剩下部分的人格名称即可，然后再将文字转换成base64编码填入此部分"\n    }\n    ```\n    多人格切换请写成json列表的形式\n4. 发送切换人格，根据机器人的提示即可切换当前人格。若切换之前存在历史对话，清除聊天历史记录即可和新人格对话。\n\n# TODO\n- [x] 添加用户自定义人格功能\n- [ ] 代理支持\n- [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)\n',
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
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_nai3_bot'] package_data = \ {'': ['*']} install_requires = \
 ['Pillow>=9.1.0,<10.0.0', 'httpx>=0.27.0,<0.28.0', 'nonebot-adapter-
 onebot>=2.2.1,<3.0.0', 'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=1.30.1,<2.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-nai3-bot', 'version': '1.0.1',
+setup_kwargs = { 'name': 'nonebot-plugin-nai3-bot', 'version': '1.1.0',
 'description': 'åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©',
 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
@@ -29,17 +29,29 @@
 = "https://xxxxxxxxx" #
 ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°å,ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å\noneapi_model
 = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å\n```\nNAI3çtokenè·åå°åæ¹æ³ï¼\n![Alt](image.png)\n\n#
 ä½¿ç¨æ¹æ³\n- ** èå¤©åå®¹/ç»å¾éæ±
 ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼\n- è®°å¿æ¸é¤
-æ¸é¤å½åç¨æ·çèå¤©è®°å½\n\n# å¯è½å­å¨çé®é¢\n-
+æ¸é¤å½åç¨æ·çèå¤©è®°å½\n- åæ¢äººæ ¼
+åæ¢æºå¨äººèå¤©çäººæ ¼\n\n# å¯è½å­å¨çé®é¢\n-
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã\n-
 æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé\n-
-æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã\n\n#
-TODO\n- [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½\n- [ ] ä»£çæ¯æ\n- [ ]
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã\n#
+æ·»å äººæ ¼\n1.
+å¨æºå¨äººè¿è¡ç®å½ç`data`æä»¶å¤¹ä¸åå»ºæä»¶`nai3_character.json`\n2.
+åè[äººæ ¼è°ææ¨¡ç]
+(default_character.txt)æä»¶ï¼å°æ¨¡çä¸­çç¬¬1é¨åä¿®æ¹æä½ çæ°äººæ ¼åæ´æ¹å©ä¸é¨åçäººæ ¼åç§°ã\n3.
+åè[äººæ ¼åè¡¨æ¨¡ç]
+(nai3_character.json)ï¼ä¿®æ¹`nai3_character.json`æä»¶ãjsonæä»¶çæ ¼å¼å¦ä¸ï¼\n
+```json\n {\n "name": "äººæ ¼åç§°ï¼ç¨äºåæ¢äººæ ¼æ¶åºåï¼",\n
+"nickname": "äººæ ¼æµç§°",\n "prompt":
+"è°æpromptçbase64ç¼ç æ ¼å¼ï¼è¯·åç§é»è®¤äººæ ¼æ¨¡çï¼å°æ¨¡çä¸­çç¬¬1é¨åä¿®æ¹æä½ çæ°äººæ ¼åæ´æ¹å©ä¸é¨åçäººæ ¼åç§°å³å¯ï¼ç¶ååå°æå­è½¬æ¢æbase64ç¼ç å¡«å¥æ­¤é¨å"\n
+}\n ```\n å¤äººæ ¼åæ¢è¯·åæjsonåè¡¨çå½¢å¼\n4.
+åéåæ¢äººæ ¼ï¼æ ¹æ®æºå¨äººçæç¤ºå³å¯åæ¢å½åäººæ ¼ãè¥åæ¢ä¹åå­å¨åå²å¯¹è¯ï¼æ¸é¤èå¤©åå²è®°å½å³å¯åæ°äººæ ¼å¯¹è¯ã\n\n#
+TODO\n- [x] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½\n- [ ] ä»£çæ¯æ\n- [ ]
 æ¯æç»å¾æéä¿¡æ¯æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)\n', 'author':
 'Alpaca', 'author_email': 'alpaca@bupt.edu.cn', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'None', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_nai3_bot-1.0.1/PKG-INFO` & `nonebot_plugin_nai3_bot-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3-bot
-Version: 1.0.1
+Version: 1.1.0
 Summary: 基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -70,18 +70,32 @@
 ```
 NAI3的token获取地址方法：
 ![Alt](image.png)
 
 # 使用方法
 - **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）
 - 记忆清除 清除当前用户的聊天记录
+- 切换人格 切换机器人聊天的人格
 
 # 可能存在的问题
 - 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。
 - 注意语言大模型的token消耗量
 - 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。
+# 添加人格
+1. 在机器人运行目录的`data`文件夹下创建文件`nai3_character.json`
+2. 参考[人格调教模版](default_character.txt)文件，将模版中的第1部分修改成你的新人格和更改剩下部分的人格名称。
+3. 参考[人格列表模版](nai3_character.json)，修改`nai3_character.json`文件。json文件的格式如下：
+   ```json
+   {
+        "name": "人格名称（用于切换人格时区分）",
+        "nickname": "人格昵称",
+        "prompt": "调教prompt的base64编码格式，请参照默认人格模版，将模版中的第1部分修改成你的新人格和更改剩下部分的人格名称即可，然后再将文字转换成base64编码填入此部分"
+    }
+    ```
+    多人格切换请写成json列表的形式
+4. 发送切换人格，根据机器人的提示即可切换当前人格。若切换之前存在历史对话，清除聊天历史记录即可和新人格对话。
 
 # TODO
-- [ ] 添加用户自定义人格功能
+- [x] 添加用户自定义人格功能
 - [ ] 代理支持
 - [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 1.1.0 Summary:
 åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©
 License: MIT Author: Alpaca Author-email: alpaca@bupt.edu.cn Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -30,13 +30,25 @@
 ï¼å¿å¡«ï¼OpenAIå®æ¹æèæ¯æ¯æOneAPIçå¤§æ¨¡åä¸­è½¬æå¡åæä¾çKEY
 ``` å¯éåå®¹ï¼ ``` oneapi_url = "https://xxxxxxxxx" #
 ï¼å¯éï¼å¤§æ¨¡åä¸­è½¬æå¡åæä¾çä¸­è½¬å°å,ä½¿ç¨OpenAIå®æ¹æå¡ä¸éè¦å¡«å
 oneapi_model = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å ``` NAI3çtokenè·åå°åæ¹æ³ï¼ ![Alt](image.png) # ä½¿ç¨æ¹æ³
 - ** èå¤©åå®¹/ç»å¾éæ± ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼ -
-è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ # å¯è½å­å¨çé®é¢ -
+è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ - åæ¢äººæ ¼
+åæ¢æºå¨äººèå¤©çäººæ ¼ # å¯è½å­å¨çé®é¢ -
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã
 - æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé -
 æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã
-# TODO - [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
+# æ·»å äººæ ¼ 1.
+å¨æºå¨äººè¿è¡ç®å½ç`data`æä»¶å¤¹ä¸åå»ºæä»¶`nai3_character.json`
+2. åè[äººæ ¼è°ææ¨¡ç]
+(default_character.txt)æä»¶ï¼å°æ¨¡çä¸­çç¬¬1é¨åä¿®æ¹æä½ çæ°äººæ ¼åæ´æ¹å©ä¸é¨åçäººæ ¼åç§°ã
+3. åè[äººæ ¼åè¡¨æ¨¡ç]
+(nai3_character.json)ï¼ä¿®æ¹`nai3_character.json`æä»¶ãjsonæä»¶çæ ¼å¼å¦ä¸ï¼
+```json { "name": "äººæ ¼åç§°ï¼ç¨äºåæ¢äººæ ¼æ¶åºåï¼", "nickname":
+"äººæ ¼æµç§°", "prompt":
+"è°æpromptçbase64ç¼ç æ ¼å¼ï¼è¯·åç§é»è®¤äººæ ¼æ¨¡çï¼å°æ¨¡çä¸­çç¬¬1é¨åä¿®æ¹æä½ çæ°äººæ ¼åæ´æ¹å©ä¸é¨åçäººæ ¼åç§°å³å¯ï¼ç¶ååå°æå­è½¬æ¢æbase64ç¼ç å¡«å¥æ­¤é¨å"
+} ``` å¤äººæ ¼åæ¢è¯·åæjsonåè¡¨çå½¢å¼ 4.
+åéåæ¢äººæ ¼ï¼æ ¹æ®æºå¨äººçæç¤ºå³å¯åæ¢å½åäººæ ¼ãè¥åæ¢ä¹åå­å¨åå²å¯¹è¯ï¼æ¸é¤èå¤©åå²è®°å½å³å¯åæ°äººæ ¼å¯¹è¯ã
+# TODO - [x] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
 æ¯æç»å¾æéä¿¡æ¯æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
```

