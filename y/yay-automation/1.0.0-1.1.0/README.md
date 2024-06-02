# Comparing `tmp/yay-automation-1.0.0.tar.gz` & `tmp/yay-automation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yay-automation-1.0.0.tar", last modified: Sat Jun  1 20:58:10 2024, max compression
+gzip compressed data, was "yay-automation-1.1.0.tar", last modified: Sun Jun  2 15:34:46 2024, max compression
```

## Comparing `yay-automation-1.0.0.tar` & `yay-automation-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:58:10.890422 yay-automation-1.0.0/
--rw-rw-rw-   0        0        0     5794 2024-06-01 20:58:10.890422 yay-automation-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5254 2024-06-01 20:57:33.000000 yay-automation-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 20:58:10.890422 yay-automation-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      745 2024-06-01 20:56:57.000000 yay-automation-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:58:10.868498 yay-automation-1.0.0/yay_automation/
--rw-rw-rw-   0        0        0      115 2024-06-01 20:55:58.000000 yay-automation-1.0.0/yay_automation/__init__.py
--rw-rw-rw-   0        0        0    11198 2024-06-01 19:46:30.000000 yay-automation-1.0.0/yay_automation/main.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:58:10.889130 yay-automation-1.0.0/yay_automation.egg-info/
--rw-rw-rw-   0        0        0     5794 2024-06-01 20:58:10.000000 yay-automation-1.0.0/yay_automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-06-01 20:58:10.000000 yay-automation-1.0.0/yay_automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:58:10.000000 yay-automation-1.0.0/yay_automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-06-01 20:58:10.000000 yay-automation-1.0.0/yay_automation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 15:34:46.032782 yay-automation-1.1.0/
+-rw-rw-rw-   0        0        0     5794 2024-06-02 15:34:46.032782 yay-automation-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5254 2024-06-01 20:57:33.000000 yay-automation-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:34:46.032782 yay-automation-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      745 2024-06-02 15:29:32.000000 yay-automation-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:34:46.010562 yay-automation-1.1.0/yay_automation/
+-rw-rw-rw-   0        0        0      115 2024-06-02 15:29:23.000000 yay-automation-1.1.0/yay_automation/__init__.py
+-rw-rw-rw-   0        0        0    10780 2024-06-02 15:24:44.000000 yay-automation-1.1.0/yay_automation/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:34:46.030132 yay-automation-1.1.0/yay_automation.egg-info/
+-rw-rw-rw-   0        0        0     5794 2024-06-02 15:34:45.000000 yay-automation-1.1.0/yay_automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-06-02 15:34:45.000000 yay-automation-1.1.0/yay_automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:34:45.000000 yay-automation-1.1.0/yay_automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-02 15:34:45.000000 yay-automation-1.1.0/yay_automation.egg-info/top_level.txt
```

### Comparing `yay-automation-1.0.0/PKG-INFO` & `yay-automation-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yay-automation
-Version: 1.0.0
+Version: 1.1.0
 Summary: yay!というSNSに使えるAPIラッパー
 Home-page: https://github.com/taka-4602/yay-automation
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: yay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yay-automation-1.0.0/README.md` & `yay-automation-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `yay-automation-1.0.0/setup.py` & `yay-automation-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='yay-automation',
-    version='1.0.0',
+    version='1.1.0',
     keywords = "yay",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/yay-automation',
     description='yay!というSNSに使えるAPIラッパー',
```

### Comparing `yay-automation-1.0.0/yay_automation/main.py` & `yay-automation-1.1.0/yay_automation/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,30 +11,30 @@
             if email:
                 payload={
                 "password":password,
                 "uuid":uuid,
                 "email":email,
                 "api_key":"92816834ea82099597f7285db999b4b74496eaf9b7e17007ebaaa8be4eb19ad5"
                 }
-                login=requests.post("https://api-203.yay.space/v3/users/login_with_email",data=payload,proxies=self.proxy).json()
-                if login["result"]!="success":
+                login=requests.post("https://api.yay.space/v3/users/login_with_email",data=payload,proxies=self.proxy).json()
+                if "error_code" in login:
                     raise YayError(login)
                 self.access_token=login["access_token"]
         else:
             self.access_token=access_token
     
     def register(self,email:str):
         payload={
             "device_uuid":self.uuid,
             "locale":"ja",
             "intent":"sign_up",
             "email":email
             }
-        verification_urls=requests.post("https://api-203.yay.space/v1/email_verification_urls",data=payload,proxies=self.proxy).json()
-        if verification_urls["result"]!="success":
+        verification_urls=requests.post("https://api.yay.space/v1/email_verification_urls",data=payload,proxies=self.proxy).json()
+        if "error_code" in verification_urls:
             raise YayError(verification_urls)
         signatures=verification_urls["url"].replace("https://idcardcheck.com/apis/v1/apps/yay/","")
         payload={
             "locale":"ja",
             "email":email
             }
         verification_signature=requests.post(f"https://idcardcheck.com/apis/v1/apps/yay/{signatures}",data=payload,proxies=self.proxy).json()
@@ -48,18 +48,18 @@
         grant_tokens=requests.post("https://idcardcheck.com/apis/v1/apps/yay/email_grant_tokens",data=payload,proxies=self.proxy).json()
         payload={
             "uuid":self.uuid,
             "api_key":"92816834ea82099597f7285db999b4b74496eaf9b7e17007ebaaa8be4eb19ad5",
             "password":password,
             "email":self.email
             }
-        login_with_email=requests.post("https://api-203.yay.space/v3/users/login_with_email",data=payload,proxies=self.proxy).json()
-        if login_with_email["result"]!="success":
+        login_with_email=requests.post("https://api.yay.space/v3/users/login_with_email",data=payload,proxies=self.proxy).json()
+        if "error_code" in login_with_email:
             raise YayError(login_with_email)
-        timestamp=requests.get("https://api-203.yay.space/v2/users/timestamp",proxies=self.proxy).json()
+        timestamp=requests.get("https://api.yay.space/v2/users/timestamp",proxies=self.proxy).json()
         payload={
             "prefecture":prefecture,
             "email_grant_token":grant_tokens["email_grant_token"],
             "timestamp":timestamp["time"],
             "uuid":self.uuid,
             #"signed_info":"4d59606254c5881c292308aa7f5d11be",
             "email":self.email,
@@ -71,70 +71,73 @@
             "gender":gender,#未設定-1,男0,女1
             "birth_date":birth_date,
             "password":password,
             "biography":biography,
             "country_code":timestamp["country"],
             "nickname":nickname
             }#コメントは必要なかった部分、なんでだろう
-        register=requests.post("https://api-203.yay.space/v3/users/register",data=payload,proxies=self.proxy).json()
-        if register["result"]!="success":
+        register=requests.post("https://api.yay.space/v3/users/register",data=payload,proxies=self.proxy).json()
+        if "error_code" in register:
             raise YayError(register)
         self.access_token=register["access_token"]
         return register["access_token"]
     
     def report(self,post_id:str,reason:str,category_id:int,opponent_id:str):
-        token={"Authorization":f"Bearer {self.access_token}"}
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
         payload={
             "reason":reason,
             "category_id":category_id,
             "opponent_id":opponent_id
             }
-        report=requests.post(f"https://api-203.yay.space/v3/posts/{post_id}/report",headers=token,data=payload,proxies=self.proxy).json()
-        if report["result"]!="success":
+        report=requests.post(f"https://api.yay.space/v3/posts/{post_id}/report",headers=token,data=payload,proxies=self.proxy).json()
+        try:
+            if report["result"]!="success":
+                raise YayError(report)
+        except:
             raise YayError(report)
         return report
     
     def like(self,post_id:str):
-        token={"Authorization":f"Bearer {self.access_token}"}
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
         payload={
             "post_ids":[
                 post_id
                 ]
             }
-        like=requests.post("https://api-203.yay.space/v2/posts/like",headers=token,data=payload,proxies=self.proxy).json()
-        if like["result"]!="success":
+        like=requests.post("https://api.yay.space/v2/posts/like",headers=token,data=payload,proxies=self.proxy).json()
+        try:
+            if like["result"]!="success":
+                raise YayError(like)
+        except:
             raise YayError(like)
         return like
     
     def unlike(self,post_id:str):
-        token={"Authorization":f"Bearer {self.access_token}"}
-        unlike=requests.post(f"https://api-203.yay.space/v1/posts/{post_id}/unlike",headers=token,data={},proxies=self.proxy).json()
-        if unlike["result"]!="success":
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
+        unlike=requests.post(f"https://api.yay.space/v1/posts/{post_id}/unlike",headers=token,data={},proxies=self.proxy).json()
+        try:
+            if unlike["result"]!="success":
+                raise YayError(unlike)
+        except:
             raise YayError(unlike)
-        return unlike
-    
-    '''def post_x(self,text:str="",font_size:int=0):#1140
-        char_set = string.digits + string.ascii_lowercase
-        random_string = ''.join(random.sample(char_set, 32))
-        token={"Authorization":f"Bearer {self.access_token}"}
-        timestamp=requests.get("https://api-203.yay.space/v2/users/timestamp",proxies=self.proxy).json()
-        payload={
-            "api_key":"92816834ea82099597f7285db999b4b74496eaf9b7e17007ebaaa8be4eb19ad5",
-            "text":text,
-            "font_size":font_size,
-            "timestamp":timestamp["time"],
-            "signed_info":random_string
-            }
-        post=requests.post(f"https://api-203.yay.space/v3/posts/new",headers=token,data=payload,proxies=self.proxy).json()
-        if post["result"]!="success":
-            raise YayError(post)
-        return post'''
     
     def post(self,text:str,tags:list="[]",choices:list=None,font_size:str="0",color:str="0",post_id:str=None):
-        token={"Authorization":f"Bearer {self.access_token}"}
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
         payload={
             "color": color,
             "font_size": font_size,
             "message_tags": tags,
             "post_type": "text",
             "text": text,
             "uuid": str(uuid4())
@@ -146,79 +149,86 @@
             payload["in_reply_to"]=post_id
         post=requests.post(f"https://yay.space/api/posts",headers=token,data=payload,proxies=self.proxy).json()
         if post["result"]!="success":
             raise YayError(post)
         return post
     
     def repost(self,text:str,post_id:str,tags:list="[]",font_size:str="0",color:str="0"):
-        token={"Authorization":f"Bearer {self.access_token}"}
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
         payload={
             "color": color,
             "font_size": font_size,
             "message_tags": str(tags),
             "post_type": "text",
             "text": text,
             "post_id": post_id
             }
         repost=requests.post(f"https://yay.space/api/posts",headers=token,data=payload,proxies=self.proxy).json()
         if repost["result"]!="success":
             raise YayError(repost)
         return repost
     
-    '''def change_profile_x(self,):
-        token={"Authorization":f"Bearer {self.access_token}"}
-        timestamp=requests.get("https://api-203.yay.space/v2/users/timestamp",proxies=self.proxy).json()
-        char_set = string.digits + string.ascii_lowercase
-        random_string = ''.join(random.sample(char_set, 32))
-        payload={
-            "country_code":"JP",
-            "nickname":"adfasdfasfgfffff",
-            "gender":-1,
-            "signed_info":random_string,
-            "timestamp":timestamp["time"],
-            "uuid":"790A36DA-43C5-485A-8E08-7D53FCF16DB5",
-            "biography":"cccccvjkf",
-            "prefecture":"",
-            "is_private":False,
-            "api_key":"92816834ea82099597f7285db999b4b74496eaf9b7e17007ebaaa8be4eb19ad5"
-            }
-        cp=requests.post("https://api-203.yay.space/v3/users/edit",headers=token,data=payload,proxies=self.proxy).json()
-        if cp["result"]!="success":
-            raise YayError(cp)
-        return cp'''
-
+    def follow(self,user_id:str):
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
+        payload={"userId":user_id}
+        follow=requests.post(f"https://api.yay.space/v2/users/{user_id}/follow",headers=token,data=payload,proxies=self.proxy).json()
+        try:
+            if follow["result"]!="success":
+                raise YayError(follow)
+        except:
+            raise YayError(follow)
+        return follow
+    
+    def unfollow(self,user_id:str):
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
+        payload={"userId":user_id}
+        unfollow=requests.post(f"https://api.yay.space/v2/users/{user_id}/unfollow",headers=token,data=payload,proxies=self.proxy).json()
+        try:
+            if unfollow["result"]!="success":
+                raise YayError(unfollow)
+        except:
+            raise YayError(unfollow)
+        return unfollow
+    
     def change_profile(self,nickname:str,biography:str="",prefecture:str=None):
-        token={"Authorization":f"Bearer {self.access_token}"}
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
         payload={
             "nickname": nickname,
             "biography": biography,
             }
         if prefecture:
             payload["prefecture"]=prefecture #都道府県
         cp=requests.post("https://api.yay.space/v3/users/edit",headers=token,data=payload,proxies=self.proxy).json()
-        if cp["result"]!="success":
+        try:
+            if cp["result"]!="success":
+                raise YayError(cp)
+        except:
             raise YayError(cp)
         return cp
 
     def add_to_bookmark(self,post_id:str):
-        token={"Authorization":f"Bearer {self.access_token}"}
-        bookmark=requests.post(f"https://api-203.yay.space/v1/users/8926797/bookmarks/{post_id}",headers=token,proxies=self.proxy).json()
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
+        bookmark=requests.post(f"https://api.yay.space/v1/users/8926797/bookmarks/{post_id}",headers=token,proxies=self.proxy).json()
         return bookmark
     
     def remove_from_bookmark(self,post_id:str,user_id:str):
-        token={"Authorization":f"Bearer {self.access_token}"}
-        bookmark=requests.delete(f"https://api-203.yay.space/v1/users/{user_id}/bookmarks/{post_id}",headers=token,proxies=self.proxy)
-        return bookmark.status_code
-
-yay=Yay()
-yay.register(email="メールアドレス")
-yay.register_code(code="メールされた6桁のコード",password="パスワード",nickname="アカウント名",biography="自己紹介",birth_date="2000-05-02",gender=-1,prefecture="都道府県",referral_code="招待コード？")
-yay=Yay(email="メールアドレス",password="パスワード")#,access_token="ベアラートークン",proxy="dict")#これがログイン、トークンをつけるとログインをスキップする
-yay.post(text="本文",tags=["リスト、タグ？使ったことない"],choices=["これもリスト","5個まで","選択肢を","設定","できる"],font_size="0",color="0",post_id="返信先のポストID")#本文しか書かなくていい
-yay.repost(text="本文",post_id="リポストするポストID",tags=["リスト"])
-yay.change_profile(nickname="アカウント名",biography="自己紹介",prefecture="都道府県")
-yay.like("いいねするポストのID")
-yay.unlike("いいねけすポストのID")
-yay.add_to_bookmark("ブックマークするポストのID")
-yay.remove_from_bookmark("ブックマークけすポストのID")
-yay.report(post_id="通報するポストのID",reason="理由、絶対いるらしい",category_id=0,opponent_id="通報するポスト主のユーザーID")
-#↑カテゴリーIDは0～6までそれぞれ、不快なコンテンツ・煽り・暴言=0、スパム=1、他サイトへ誘導・ID交換=2、仕事・勧誘などの業者=3、出会い厨=4、なりすまし・権利侵害=5、その他=6
+        token={
+            "Authorization":f"Bearer {self.access_token}",
+            "X-Device-Info":"Yay 3.39.0 Web (Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36)"
+            }
+        bookmark=requests.delete(f"https://api.yay.space/v1/users/{user_id}/bookmarks/{post_id}",headers=token,proxies=self.proxy)
+        return bookmark.status_code
```

### Comparing `yay-automation-1.0.0/yay_automation.egg-info/PKG-INFO` & `yay-automation-1.1.0/yay_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yay-automation
-Version: 1.0.0
+Version: 1.1.0
 Summary: yay!というSNSに使えるAPIラッパー
 Home-page: https://github.com/taka-4602/yay-automation
 Author: taka4602
 Author-email: shun4602@gmail.com
 Keywords: yay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

