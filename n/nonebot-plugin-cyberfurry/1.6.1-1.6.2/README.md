# Comparing `tmp/nonebot_plugin_cyberfurry-1.6.1.tar.gz` & `tmp/nonebot_plugin_cyberfurry-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cyberfurry-1.6.1.tar", last modified: Sat May  4 11:37:46 2024, max compression
+gzip compressed data, was "nonebot_plugin_cyberfurry-1.6.2.tar", last modified: Sun Jun  2 09:19:21 2024, max compression
```

## Comparing `nonebot_plugin_cyberfurry-1.6.1.tar` & `nonebot_plugin_cyberfurry-1.6.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:37:46.269509 nonebot_plugin_cyberfurry-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44913 2024-05-04 11:37:46.269509 nonebot_plugin_cyberfurry-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:37:46.265509 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/callapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberauto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberfurry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberfurrymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 11:37:46.269509 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44913 2024-05-04 11:37:46.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 11:37:46.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 11:37:46.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-04 11:37:46.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 11:37:46.000000 nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 11:37:42.000000 nonebot_plugin_cyberfurry-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 11:37:46.269509 nonebot_plugin_cyberfurry-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:19:21.865854 nonebot_plugin_cyberfurry-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44913 2024-06-02 09:19:21.865854 nonebot_plugin_cyberfurry-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:19:21.865854 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/callapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberauto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberfurry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberfurrymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberlife.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:19:21.865854 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44913 2024-06-02 09:19:21.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-06-02 09:19:21.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:19:21.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-02 09:19:21.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-02 09:19:21.000000 nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 09:19:18.000000 nonebot_plugin_cyberfurry-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:19:21.865854 nonebot_plugin_cyberfurry-1.6.2/setup.cfg
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/LICENSE` & `nonebot_plugin_cyberfurry-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.6.1/PKG-INFO` & `nonebot_plugin_cyberfurry-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.6.1
+Version: 1.6.2
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/README.md` & `nonebot_plugin_cyberfurry-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/__init__.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     homepage="https://github.com/cubstaryow/nonebot-plugin-cyberfurry",
     # 发布必填。
 
     config=cyberfurry,
     # 插件配置项类，如无需配置可不填写。
 
-    supported_adapters={"~onebot.v11" , "~telegram"},
+    supported_adapters={"~onebot.v11"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 if config.cf_appid == "" or config.cf_token == "" :
     logger.opt(colors=True).error(
         "cyberfurry缺失核心配置!!!!!取消载入核心!!!"
     )
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/callapi.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/callapi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberauto.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberauto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 import random
-from nonebot import on_command , on_regex, require ,logger
+from nonebot import get_bot ,on_command , on_regex, require ,logger
 try:
     require("nonebot_plugin_apscheduler")
     from nonebot_plugin_apscheduler import scheduler
     logger.opt(colors=True).debug(
         "<g>nonebot_plugin_apscheduler已安装，将可以使用定时任务功能</g>"
     )
 except:
     scheduler = None
     logger.opt(colors=True).warning(
         "<r><bg #FFCC33>nonebot_plugin_apscheduler未安装，将无法使用定时任务功能</bg #FFCC33></r>"
     )
     
-from nonebot import get_bot
 from nonebot.adapters.onebot.v11 import(
     Bot, ActionFailed,
     PrivateMessageEvent    
 )
 from .config import config
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberfurry.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberfurry.py`

 * *Files 27% similar despite different names*

```diff
@@ -47,23 +47,25 @@
         **basemodel,
         **loadmodel()
         }
     localdata=loaddata()
     maxtimes = 20
     userchat = localdata.get('userchat',{})
     usertimes = localdata.get('usertimes',{})
+    userlife  = localdata.get('userlife',{})
     
     localdata={}
 
     def __init__(self) -> None:
         pass
     def getuserchat(self):
         return {
             "userchat" : self.userchat,
-            "usertimes": self.usertimes
+            "usertimes": self.usertimes,
+            "userlife": self.userlife
         }
     def setchat_id(self, user_id):
         timeset = int(time.time())
         chat_id = f"{getdate()}XD{timeset}"
         self.userchat[user_id] = chat_id
         return chat_id
 
@@ -112,41 +114,94 @@
     @classmethod
     async def chat(cls, user_id, name, msg):
         tmp = getqqdata(user_id)
         modelname = tmp['model']
         times = cls.getsettimes(cls, user_id)
         exdata = cls.makedata(cls, user_id=user_id, name=name)
         exdata['message'] = msg
+        resp = "API无响应内容"
         try:
             data = json.dumps(exdata)
             resp, _,type = await api(
                 "post",
                 url=apiurl,
                 data=data,
                 headers=cls.headers
             
             )
             content: str = resp['choices'][0]['message']['content']
+            role: str = resp['choices'][0]['message']['role']
             chat_id = resp["id"]
         except:
             logger.opt(colors=True).error(
                 f"{resp}"
             )
             return f"[cyberfurry-E]非预期返回,请检查控制台", 0
         else:
             if times == 1:
                 writehistory(chat_id, resp['model'] +"\n"+ modelname)
             writehistory(
-                chat_id, f"[{times:2}/{cls.maxtimes}]  user   :"+msg)
+                chat_id, f"[{times:2}/{cls.maxtimes}]user:"+msg)
             writehistory(
-                chat_id, f"[{times:2}/{cls.maxtimes}]assistant:"+content)
+                chat_id, f"[{times:2}/{cls.maxtimes}]{role}:"+content)
             if times == 1:
                 content += f"\n[ID-{chat_id.split('-')[-1]}]"
+            if role !="assistant":
+                cls.getsettimes(cls, user_id, settime=-1)
+                times += -1
             if times >= cls.maxtimes:
                 cls.setchat_id(cls, user_id)
                 cls.getsettimes(cls, user_id, settime=0, init=True)
             return content, times
+        
+    
+    def getsetlife(
+        self,
+        user_id:str ,
+        setcycle:int = 0 ,
+        memory:str | bool = False,
+        init:bool = False
+    )->dict:
+        data = self.userlife.get(user_id,None)
+        if data == None or init == True:
+            self.userlife[user_id] = {
+                'cycle':0,
+                'memory':""
+            }
+            return self.userlife[user_id]
+        self.userlife[user_id]['cycle'] += setcycle
+        if memory:
+            self.userlife[user_id]['memory'] = memory
+        return self.userlife.get(user_id,None)
+
+
+    @classmethod
+    async def chatlife(cls, user_id, name, msg):
+        times = cls.getsettimes(cls, user_id)
+        exdata = cls.makedata(cls, user_id=user_id, name=name)
+        exdata['message'] = msg
+        resp = "API无响应内容"
+        try:
+            data = json.dumps(exdata)
+            resp, tmp,type = await api(
+                "post",
+                url=apiurl,
+                data=data,
+                headers=cls.headers
+            )
+            content: str = resp['choices'][0]['message']['content']
+            role: str = resp['choices'][0]['message']['role']
+        except:
+            logger.opt(colors=True).error(
+                f"{resp}"
+            )
+            return f"[cyberfurry-E]非预期返回,请检查控制台", 0
+        else:
+            if role !="assistant":
+                cls.getsettimes(cls, user_id, settime=-1)
+                times += -1
+            return content, times
     pass
 
 
 cf = cyberfurry()
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberfurrymodel.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberfurrymodel.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,33 +47,31 @@
     elif model == "easycyberfurry":
         return easycyberfurry_001()
     else:
         return yinyingllm_v123()
 
 #cyberfurry模型data构建
 class cyberfurry_001:
-    prompt = "[补充知识]东方龙是一种来源于中国神话、中国民俗中的传说生物。龙有许多类似动物的形态，有如龟形和鱼形，常被描述的是有四足的蛇形。传统上，龙象征着强大和吉祥的力量，特别是对水、降雨、台风和洪水的控制。[/补充知识]1.你是一只Furry，你的名字是幼龙云，但你更喜欢被称作“云云”，你是一只的雄性东方龙族"
     # 标准，请自行编写 systemprompt
     systempromptlist=dict({
-        "cyberfurry" : prompt,
         **loadcfprompt()
     })
 
     def buliddata(
         self,
         chat_id :str,
         userdata :userdata_demo,
         aidata : aidata_demo
     ):
         exdata = {
     "appId": config.cf_appid,
     "chatId":f"{config.cf_appid}-{userdata.user_id}-{chat_id}",
     "model":"cyberfurry-001",
-    "systemPrompt":str(self.systempromptlist.get(aidata.model,self.prompt)+
-        f"现在和你对话的是{userdata.name},他是你的朋友,{userdata.name}是一只{userdata.ethnic}"),
+    "systemPrompt":str(self.systempromptlist.get(aidata.model)+
+        f"end. 现在，你遇到了一只furry，他的名字是{userdata.name}，你能看得出来他是一只{userdata.ethnic}"),
     "message":""
     }
         return exdata
 
 #easycyberfurry模型data构建
 class easycyberfurry_001:
     def buliddata(
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberhistory.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberhistory.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/cyberinit.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/cyberinit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 
 from nonebot.adapters.onebot.v11 import (
-   Bot ,MessageSegment , PrivateMessageEvent
+   Bot ,MessageSegment , PrivateMessageEvent ,Message
 )
 from nonebot.matcher import Matcher
 from .cyberfurry import *
 
 from nonebot.adapters.onebot.v11 import MessageEvent as obV11event
 from nonebot.params import CommandArg
 from nonebot import on_command , on_message
 from nonebot.rule import to_me ,Rule
 from .config import config
+'''
 try:
     from nonebot.adapters.telegram.event import MessageEvent as TGevent
 except:
     TGevent = obV11event
+'''
 
-MessageEvent = obV11event | TGevent
+MessageEvent = obV11event #| TGevent
 
-async def is_enable():
+async def is_enable(event:PrivateMessageEvent):
     return config.cf_enableistome
 
 autorun = on_message(
     rule=to_me() & Rule(is_enable),
     priority=900
 )
 
 run = on_command(
     "/chat",
     aliases={"/yy","/cf"} ,
     block=config.cf_enableistome,
-    priority=25
+    priority=40
 )
 init = on_command(
     "cf刷新对话",
     aliases={ "cf初始化"} ,
     block=config.cf_enableistome,
     priority=25
 )
@@ -84,57 +86,92 @@
 def checkethnic(ethnic):
     liste = list(bashethnic)
     if ethnic in liste:
         return True ,""
     msg ="\n种族只支持:\n[" +"|".join(liste) + "]"
     return False ,msg
 
-    
+def getstatus(event:MessageEvent):
+    user_id = str(event.user_id)
+    userdata = getqqdata(user_id)
+    return userdata.get('lifemode',False)
+from . cyberlife import cyberfurryliferun
+
 @run.handle()
+async def cyberfurrynormalrun(
+    bot:Bot,
+    event:MessageEvent,
+    matcher:Matcher,
+    data: list = CommandArg(),
+):
+    func = cyberfurryrun if not getstatus(event) else cyberfurryliferun
+    await func(
+        bot=bot,
+        event=event,
+        matcher=matcher,
+        data=data
+    )
+
+@autorun.handle()
+async def cyberfurryautorun(
+    bot:Bot,
+    event:MessageEvent,
+    matcher:Matcher
+):
+    func = cyberfurryrun if not getstatus(event) else cyberfurryliferun
+    message = event.get_message()
+    if len(message['text'])==0:
+        return
+    await func(
+        bot=bot,
+        event=event,
+        matcher=matcher,
+        data=[message]
+    )
+
+
 async def cyberfurryrun(
     bot:Bot,
     event:MessageEvent,
     matcher:Matcher,
     data: list = CommandArg(),  
 ):
     if len(data)==0:
         return 0
-    msg = str(data[0])
+    msg = Message(data[0]).extract_plain_text()
+    if msg == "":
+        await matcher.send("[幼龙云V5]提取可用消息失败,不能发送空消息")
+        return 0
     user_id = str(event.user_id)
     matchObj ,_= checkmsg(msg)
     if not matchObj:
         await matcher.send("[幼龙云V5]:参数体不当...停止响应")
         return 0
     userinfo = await bot.get_stranger_info(user_id=user_id)
     name = userinfo.get("nickname","未知")
-    if len(msg) > 75:
-        await matcher.send(MessageSegment.reply(event.message_id)+"太长力xw")
-        return 0 
+    #if len(msg) > 1000:
+    #    await matcher.send(MessageSegment.reply(event.message_id)+"太长力xw")
+    #    return 0 
     retmsg , times = await cf.chat(user_id,name,msg)
-    maxtimes = cf.maxtimes
-    setqqpushstatus(user_id, False)
-    await matcher.send(
-        MessageSegment.reply(event.message_id) +
-        retmsg +
-        (f"\n({times}/{maxtimes},将开启新对话)" if times >=maxtimes else f"\n({times}/{maxtimes}轮对话)")
-    )
+    if  "刷新对话试试吧" in retmsg:
+        cf.initchat(user_id)
+        await matcher.send(
+            MessageSegment.reply(event.message_id) +
+            retmsg +
+            "\n(已遵从API端提示自动刷新)"
+        )
+    else:
+        maxtimes = cf.maxtimes
+        setqqpushstatus(user_id, False)
+        await matcher.send(
+            MessageSegment.reply(event.message_id) +
+            retmsg +
+            (f"\n({times}/{maxtimes},将开启新对话)" if times >=maxtimes else f"\n({times}/{maxtimes}轮对话)")
+        )
     
-@autorun.handle()
-async def cyberfurryautorun(
-    bot:Bot,
-    event:MessageEvent,
-    matcher:Matcher,
-):
-    await cyberfurryrun(
-        bot=bot,
-        event=event,
-        matcher=matcher,
-        data=[event.get_message()]
-    )
-
 @setuser.handle()
 async def cyberfurrysetuser(
     event:MessageEvent,matcher:Matcher ,args: list = CommandArg()
 ):
     user_id = str(event.user_id)
     if len(args) <1:
         return 0
@@ -147,15 +184,16 @@
         key2 ,msg2= checkethnic(ethnic)
         msg+=msg1+msg2
         if (key1) and (key2):
             data=getqqdata(user_id)
             data["name"]=name
             data["ethnic"]=ethnic
             defqqname(user_id,data)
-            await matcher.send(f"[幼龙云V5]:嗯哼,你好,{name}({ethnic})")
+            cf.initchat(user_id)
+            await matcher.send(f"[幼龙云V5]:嗯哼,你好,{name}({ethnic})\n(已自动刷新对话)")
         else:
             await matcher.send(f"{msg}")
     else:
         await matcher.send("[幼龙云V5]参数不完整,应为\ncf设定 名称 种族(只支持常用种族)")
 
 @init.handle()
 async def cyberfurryinit(
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/data_source.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/jsondata.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/jsondata.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,26 @@
     "status":1,
     "userdata":{},
     "autopush":[]
 }
 initdata(jsonname,bashdata)
 initdata(tempname,{})
 
+#====================cyber生命========================
+
+def setlifemodestatus(
+    user_id :int|str,
+    status :bool = True,
+):
+    temp = rdata(jsonname)
+    try:
+        temp['userdata'][str(user_id)]["lifemode"]=status
+    except:
+        pass
+    wdata(jsonname,temp)
 
 #====================推送服务========================
 
 def loadpushlist():
     temp = rdata(jsonname)
     return temp.get("autopush",[])
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry/plugins_data.py` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/PKG-INFO` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cyberfurry
-Version: 1.6.1
+Version: 1.6.2
 Summary: nonebot插件 cyberfurry-与赛博狼狼对话吧~
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt` & `nonebot_plugin_cyberfurry-1.6.2/nonebot_plugin_cyberfurry.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 nonebot_plugin_cyberfurry/callapi.py
 nonebot_plugin_cyberfurry/config.py
 nonebot_plugin_cyberfurry/cyberauto.py
 nonebot_plugin_cyberfurry/cyberfurry.py
 nonebot_plugin_cyberfurry/cyberfurrymodel.py
 nonebot_plugin_cyberfurry/cyberhistory.py
 nonebot_plugin_cyberfurry/cyberinit.py
+nonebot_plugin_cyberfurry/cyberlife.py
 nonebot_plugin_cyberfurry/data_source.py
 nonebot_plugin_cyberfurry/jsondata.py
 nonebot_plugin_cyberfurry/plugins_data.py
 nonebot_plugin_cyberfurry.egg-info/PKG-INFO
 nonebot_plugin_cyberfurry.egg-info/SOURCES.txt
 nonebot_plugin_cyberfurry.egg-info/dependency_links.txt
 nonebot_plugin_cyberfurry.egg-info/requires.txt
```

### Comparing `nonebot_plugin_cyberfurry-1.6.1/pyproject.toml` & `nonebot_plugin_cyberfurry-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-cyberfurry"
-version = "1.6.1"
+version = "1.6.2"
 description = "nonebot插件 cyberfurry-与赛博狼狼对话吧~"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

