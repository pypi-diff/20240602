# Comparing `tmp/GraphSpy-1.2.0.tar.gz` & `tmp/GraphSpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSpy-1.2.0.tar", last modified: Mon May  6 19:51:14 2024, max compression
+gzip compressed data, was "GraphSpy-1.2.1.tar", last modified: Sun Jun  2 13:26:59 2024, max compression
```

## Comparing `GraphSpy-1.2.0.tar` & `GraphSpy-1.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    52022 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/GraphSpy.py
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/__init__.py
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/static/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/static/css/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      821 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/css/style.css
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/static/js/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    14019 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/js/functions.js
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    21835 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/js/purify.min.js
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/js/theme.js
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/templates/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7747 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/OneDrive.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8554 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/SharePoint.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5757 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/SharePointDrives.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6379 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/SharePointSites.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6336 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/access_token_modal.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9996 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/access_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17378 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/custom_requests.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6512 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/device_codes.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7933 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/generic_search.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/index.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    18474 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/layout.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/outlook.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5094 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/recent_files.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5679 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/refresh_token_modal.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/refresh_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7886 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/settings.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5108 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/shared_with_me.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    22318 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/teams.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/version.txt
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy.egg-info/
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7401 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/PKG-INFO
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1100 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/SOURCES.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/dependency_links.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/entry_points.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/requires.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/top_level.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/LICENSE.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/MANIFEST.in
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7401 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/PKG-INFO
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7303 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/README.md
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/requirements.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/setup.cfg
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/setup.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.196910 GraphSpy-1.2.1/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.192911 GraphSpy-1.2.1/GraphSpy/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    61282 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/GraphSpy.py
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/__init__.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.192911 GraphSpy-1.2.1/GraphSpy/static/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.192911 GraphSpy-1.2.1/GraphSpy/static/css/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      875 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/static/css/style.css
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.192911 GraphSpy-1.2.1/GraphSpy/static/js/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    15442 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/static/js/functions.js
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    21835 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/static/js/purify.min.js
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/static/js/theme.js
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.196910 GraphSpy-1.2.1/GraphSpy/templates/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7723 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/OneDrive.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8530 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/SharePoint.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5733 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/SharePointDrives.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6355 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/SharePointSites.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6356 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/access_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    10016 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/access_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    19710 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/custom_requests.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6452 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/device_codes.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7908 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/generic_search.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/index.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    19274 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/layout.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/outlook.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5070 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/recent_files.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5691 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/refresh_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6741 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/refresh_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7900 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/settings.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5084 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/shared_with_me.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    39307 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/templates/teams.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/GraphSpy/version.txt
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-06-02 13:26:59.192911 GraphSpy-1.2.1/GraphSpy.egg-info/
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7401 2024-06-02 13:26:59.000000 GraphSpy-1.2.1/GraphSpy.egg-info/PKG-INFO
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1100 2024-06-02 13:26:59.000000 GraphSpy-1.2.1/GraphSpy.egg-info/SOURCES.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-06-02 13:26:59.000000 GraphSpy-1.2.1/GraphSpy.egg-info/dependency_links.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-06-02 13:26:59.000000 GraphSpy-1.2.1/GraphSpy.egg-info/entry_points.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-06-02 13:26:59.000000 GraphSpy-1.2.1/GraphSpy.egg-info/requires.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-06-02 13:26:59.000000 GraphSpy-1.2.1/GraphSpy.egg-info/top_level.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/LICENSE.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/MANIFEST.in
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7401 2024-06-02 13:26:59.196910 GraphSpy-1.2.1/PKG-INFO
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7303 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/README.md
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/requirements.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-06-02 13:26:59.196910 GraphSpy-1.2.1/setup.cfg
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-06-02 13:26:54.000000 GraphSpy-1.2.1/setup.py
```

### Comparing `GraphSpy-1.2.0/GraphSpy/GraphSpy.py` & `GraphSpy-1.2.1/GraphSpy/GraphSpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sqlite3
 from datetime import datetime, timezone
 import time
 import os,sys,shutil,traceback,logging
 from threading import Thread
 import json
 import uuid
+import re
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)),"version.txt")) as f:
     __version__ = f.read()
 
 # ========== Database ==========
 
 def init_db():
@@ -143,15 +144,15 @@
 
     # Format json if the Content-Type contains json
     response_type = "json" if ("Content-Type" in response.headers and "json" in response.headers["Content-Type"]) else "xml" if ("Content-Type" in response.headers and "xml" in response.headers["Content-Type"]) else "text"
     try:
         response_text = json.dumps(response.json()) if response_type == "json" else response.text
     except ValueError as e:
         response_text = response.text
-    return {"response_status_code": response.status_code ,"response_type": response_type ,"response_text": response_text}
+    return {"response_status_code": response.status_code ,"response_type": response_type ,"response_text": response_text, "response_headers": dict(response.headers)}
 
 def save_access_token(accesstoken, description):
     decoded_accesstoken = jwt.decode(accesstoken, options={"verify_signature": False})
     user = "unknown"
     # If the idtype is user, use the unique_name or upn
     # If the idtype is app, use the app_displayname or appid
     # Otherwise, use whatever we can get
@@ -757,26 +758,25 @@
         conversation_link = request.form['conversation_link']
         if not "message_content" in request.form:
             return f"[Error] No message_content specified.", 400
         message_content = request.form['message_content']
         teams_settings = getTeamsSettings(access_token_id)
         if not teams_settings:
             return f"[Error] Unable to obtain teams settings with access token {access_token_id}.", 400
-        headers = {"Authentication":f"skypetoken={teams_settings['skypeToken']}"}
+        headers = {"Authentication":f"skypetoken={teams_settings['skypeToken']}", "User-Agent":get_user_agent()}
         body = {
             "messagetype": "RichText/Html",
             "content": message_content
         }
         response = requests.post(conversation_link, headers=headers, json=body)
         if response.status_code >= 200 and response.status_code < 300:
             message_id = response.json()["OriginalArrivalTime"] if "OriginalArrivalTime" in response.json() else "Unknown"
             return f"{message_id}"
         return f"[Error] Something went wrong trying to send Teams message. Received response status {response.status_code}", 400
-        gspy_log.error("Failed sending teams message. Received response status {response.status_code}. Response body:")
-        gspy_log.error(response.json())
+        gspy_log.error(f"Failed sending teams message. Received response status {response.status_code}. Response body:\n {response.content}")
 
     @app.post("/api/get_teams_conversation_members")
     def api_get_teams_conversation_members():
         if not "access_token_id" in request.form:
             return f"[Error] No access_token_id specified.", 400
         access_token_id = request.form['access_token_id']
         if not "conversation_id" in request.form:
@@ -788,34 +788,180 @@
         teams_and_channel_service_uri = json.loads(teams_settings['teams_settings_raw'])['regionGtms']['teamsAndChannelsService']
         uri = f"{teams_and_channel_service_uri}/beta/teams/{conversation_id}/members"
         response = generic_request(uri, access_token_id, "GET", "text", "", {})
         if response['response_status_code'] == 200 and response['response_type'] == "json":
             conversation_members = json.loads(response['response_text'])
             # Add `isCurrentUser: True` to the member if the member is the current user.
             conversation_members = [{**member, "isCurrentUser": member["mri"].endswith(teams_settings["skype_id"])} for member in conversation_members]
+            gspy_log.debug(f"Found {len(conversation_members)} members in conversation '{conversation_id}'")
             return conversation_members
+        gspy_log.error(f"Failed listing members in conversation '{conversation_id}'. Received response status {response['response_status_code']}. Response body: \n{response['response_text']}")
         return f"[Error] Something went wrong trying to obtain Teams Members. Received response status {response['response_status_code']} and response type {response['response_type']}", 400
 
     @app.get("/api/get_teams_image")
     def api_get_teams_image():
         if not "access_token_id" in request.args:
             return f"[Error] No access_token_id specified.", 400
         access_token_id = request.args['access_token_id']
         if not "image_uri" in request.args:
             return f"[Error] No image_uri specified.", 400
         image_uri = request.args['image_uri']
         teams_settings = getTeamsSettings(access_token_id)
         if not teams_settings:
             return f"[Error] Unable to obtain teams settings with access token {access_token_id}.", 400
         cookies = {"skypetoken_asm":teams_settings['skypeToken']}
-        response = requests.get(image_uri, cookies=cookies)
+        headers = {"User-Agent":get_user_agent()}
+        response = requests.get(image_uri, cookies=cookies, headers=headers)
         if response.status_code == 200:
             return Response(response.content, mimetype=response.headers['Content-Type'])
         return f"[Error] Something went wrong trying to obtain teams image. Received response status {response.status_code} and response type {response.headers['Content-Type'] if 'Content-Type' in response.headers else 'empty'}", 400
+        
+    @app.post("/api/list_teams_users")
+    def api_list_teams_users():
+        if not "access_token_id" in request.form:
+            return f"[Error] No access_token_id specified.", 400
+        access_token_id = request.form['access_token_id']
+        teams_settings = getTeamsSettings(access_token_id)
+        if not teams_settings:
+            return f"[Error] Unable to obtain teams settings with access token {access_token_id}.", 400
+        teams_and_channel_service_uri = json.loads(teams_settings['teams_settings_raw'])['regionGtms']['teamsAndChannelsService']
+        base_uri = f"{teams_and_channel_service_uri}/beta/users?top=999"
+        teams_users = []
+        next_skiptoken = ""
+        while True:
+            uri = f"{base_uri}&skipToken={next_skiptoken}" if next_skiptoken else base_uri
+            response = generic_request(uri, access_token_id, "GET", "text", "")
+            if not (response['response_status_code'] == 200 and response['response_type'] == "json"):
+                break
+            responseJson = json.loads(response['response_text'])
+            if not "users" in responseJson:
+                break
+            teams_users += responseJson["users"]
+            if not "skipToken" in responseJson:
+                return teams_users
+            next_skiptoken = responseJson["skipToken"]
+        return f"[Error] Something went wrong trying to list Teams Users. Received response status {response['response_status_code']} and response type {response['response_type']}", 400
+
+    @app.get("/api/get_teams_user_details")
+    def api_get_teams_user_details():
+        if not "access_token_id" in request.args:
+            return f"[Error] No access_token_id specified.", 400
+        access_token_id = request.args['access_token_id']
+        teams_settings = getTeamsSettings(access_token_id)
+        if not teams_settings:
+            return f"[Error] Unable to obtain teams settings with access token {access_token_id}.", 400
+        teams_and_channel_service_uri = json.loads(teams_settings['teams_settings_raw'])['regionGtms']['teamsAndChannelsService']
+        if not "user_id" in request.args:
+            return f"[Error] No user_id specified. Specify a valid UPN, ObjectID or MRI of the user", 400
+        user_id = request.args['user_id']
+        uri = f"{teams_and_channel_service_uri}/beta/users/{user_id}"
+        headers = {"x-ms-client-version":"27/1.0.0.2020101241"}
+        if "external" in request.args and request.args["external"].lower() == "true":
+            uri += "/externalsearchv3"
+        response = generic_request(uri, access_token_id, "GET", "text", "", headers)
+        if response['response_status_code'] == 200 and response['response_type'] == "json":
+            return json.loads(response['response_text'])
+        elif response['response_status_code'] == 404:
+            return f"[Error] User '{user_id} not found'", 404
+        return f"[Error] Something went wrong trying to list Teams Users. Received response status {response['response_status_code']} and response type {response['response_type']}", 400
 
+    @app.post("/api/create_teams_conversation")
+    def api_create_teams_conversation(): # access_token_id, members, type, topic, message_content
+        if not request.is_json:
+            return f"[Error] Expecting JSON input.", 400
+        request_json = request.get_json()
+        if not "access_token_id" in request_json:
+            return f"[Error] No access_token_id specified.", 400
+        access_token_id = request_json['access_token_id']
+        if not "members" in request_json:
+            return f"[Error] No members specified.", 400
+        members = request_json['members']
+        if not "type" in request_json:
+            return f"[Error] No conversation type specified.", 400
+        conversation_type = request_json['type']
+        if not conversation_type in ["direct_message", "group_chat"]:
+            return f"[Error] Type needs to be either 'direct_message' or 'group_chat'.", 400
+        teams_settings = getTeamsSettings(access_token_id)
+        if not teams_settings:
+            return f"[Error] Unable to obtain teams settings with access token {access_token_id}.", 400
+        chat_service_uri = json.loads(teams_settings['teams_settings_raw'])['regionGtms']['chatService']
+        uri = f"{chat_service_uri}/v1/threads"
+        headers = {"Authentication":f"skypetoken={teams_settings['skypeToken']}", "User-Agent":get_user_agent()}
+        # Adding ourself first
+        conversation_members = [{
+            "id": f"8:{teams_settings['skype_id']}",
+            "role": "Admin"
+        }]
+        conversation_properties = {
+            "threadType": "chat",
+            "chatFilesIndexId": "2",
+            "fixedRoster": "true",
+            "uniquerosterthread": "true" if conversation_type == "direct_message" else "false"
+        }
+        if "topic" in request_json:
+            conversation_properties["topic"] = request_json["topic"]
+        created_conversations = []
+        if conversation_type == "direct_message":
+            for member in members:
+                body = {
+                    "members": conversation_members[:],
+                    "properties": conversation_properties
+                }
+                body["members"].append({
+                    "id": member,
+                    "role": "Admin"
+                })
+                response = requests.post(uri, headers=headers, json=body)
+                if response.status_code >= 200 and response.status_code < 300 and "Location" in response.headers:
+                    conversation_id_regex = re.search('https:\/\/emea\.ng\.msg\.teams\.microsoft\.com\/v1\/threads\/(.*)$', response.headers["Location"])
+                    if conversation_id_regex:
+                        conversation_id = conversation_id_regex.group(1)
+                        created_conversations.append(conversation_id)
+                        gspy_log.debug(f"Created conversation with member {member}. Conversation ID: {conversation_id}")
+                        continue
+                gspy_log.error(f"Failed creating direct message conversation with user {member}. Received response status {response.status_code}.\n{response.content}")
+        elif conversation_type == "group_chat":
+            for member in members:
+                conversation_members.append({
+                    "id": member,
+                    "role": "Admin"
+                })
+            body = {
+                "members": conversation_members,
+                "properties": conversation_properties
+            }
+            response = requests.post(uri, headers=headers, json=body)
+            if response.status_code >= 200 and response.status_code < 300 and "Location" in response.headers:
+                conversation_id_regex = re.search('https:\/\/emea\.ng\.msg\.teams\.microsoft\.com\/v1\/threads\/(.*)$', response.headers["Location"])
+                if conversation_id_regex:
+                    conversation_id = conversation_id_regex.group(1)
+                    created_conversations.append(conversation_id)
+                    gspy_log.debug(f"Created conversation with {len(members)} members. Conversation ID: {conversation_id}")
+                else:
+                    gspy_log.error(f"Failed creating group chat conversation. Received response status {response.status_code}\n{response.content}.")
+            else:
+                gspy_log.error(f"Failed creating group chat conversation. Received response status {response.status_code}.\n{response.content}")
+        gspy_log.debug(f"Created {len(created_conversations)} conversations.")
+        if len(created_conversations) == 0:
+            return f"[Error] Something went wrong creating the conversation(s).", 400
+        # If a message is specified, send an initial message to every created conversation
+        if "message_content" in request_json:
+            body = {
+                "messagetype": "RichText/Html",
+                "content": request_json["message_content"]
+            }
+            for conversation_id in created_conversations:
+                conversation_link = f"{chat_service_uri}/v1/users/ME/conversations/{conversation_id}/messages"
+                response = requests.post(conversation_link, headers=headers, json=body)
+                if response.status_code >= 200 and response.status_code < 300:
+                    message_id = response.json()["OriginalArrivalTime"] if "OriginalArrivalTime" in response.json() else "Unknown"
+                    gspy_log.debug(f"Sent message to conversation {conversation_id}. Message ID: {message_id}")
+                else:
+                    gspy_log.error(f"Failed sending message to {conversation_id}. Received response status {response.status_code}.\n{response.content}")
+        return created_conversations
 
         # ========== Database ==========
     
     @app.get("/api/list_databases")
     def api_list_databases():
         return list_databases()
```

### Comparing `GraphSpy-1.2.0/GraphSpy/static/js/functions.js` & `GraphSpy-1.2.1/GraphSpy/static/js/functions.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -270,14 +270,55 @@
     if (response.status >= 400) {
         bootstrapToast("Teams Members", response.responseText, "danger");
         return;
     }
     return response.responseJSON;
 }
 
+function getTeamsUserDetails(access_token_id, user_id, external = false) {
+    let response = $.ajax({
+        type: "GET",
+        async: false,
+        url: `/api/get_teams_user_details?access_token_id=${access_token_id}&user_id=${user_id}&external=${external.toString()}`
+    });
+    if (response.status >= 400) {
+        bootstrapToast("Get Teams User Details", response.responseText, "danger");
+        return;
+    }
+    return response.responseJSON;
+}
+
+function createTeamsConversation(access_token_id, members, type = "group_chat", topic = null, message_content = null) {
+    body = {
+        "access_token_id": access_token_id,
+        "members": members,
+        "type": type
+    };
+    if (topic) {
+        body["topic"] = topic
+    };
+    if (message_content) {
+        body["message_content"] = message_content
+    };
+    let response = $.ajax({
+        type: "POST",
+        async: false,
+        url: "/api/create_teams_conversation",
+        dataType: "json",
+        contentType: "application/json; charset=utf-8",
+        data: JSON.stringify(body)
+    });
+    if (response.status >= 400) {
+        bootstrapToast("Create Teams Conversation", response.responseText, "danger");
+        return;
+    }
+    bootstrapToast("Create Teams Conversation", `Successfully created ${response.responseJSON.length} conversation(s).`, "success");
+    return response.responseJSON;
+}
+
 
 // ========== Settings ==========
 
 function setTableErorMessages(state) {
     let response = $.ajax({
         type: "POST",
         async: false,
```

### Comparing `GraphSpy-1.2.0/GraphSpy/static/js/purify.min.js` & `GraphSpy-1.2.1/GraphSpy/static/js/purify.min.js`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/GraphSpy/static/js/theme.js` & `GraphSpy-1.2.1/GraphSpy/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/OneDrive.html` & `GraphSpy-1.2.1/GraphSpy/templates/OneDrive.html`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     <script>
         getActiveAccessToken(document.getElementById("onedrive_form").access_token_id)
     </script>
 </div>
 <br>
 <div>
     <h2>Files</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created</th>
                 <th>Last Modified</th>
                 <th>File Name</th>
@@ -76,15 +76,15 @@
                 },
                 columns: [
                     {
                         className: 'dt-control',
                         orderable: false,
                         data: null,
                         defaultContent: '',
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         className: 'action-control',
                         orderable: false,
                         data: null,
                         render: function (d, t, r) {
                             if (r.folder) {
@@ -93,28 +93,28 @@
                             } else if (r.file) {
                                 // Download icon
                                 return '<i class="fi fi-br-download" style="cursor: pointer"></i>'
                             }
                             // Question mark icon
                             return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                         },
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         data: 'createdDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     {
                         data: 'lastModifiedDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     { data: 'name' },
                     {
                         data: 'size',
-                        width: '100px'
+                        width: '120px'
                     },
                     { data: 'webUrl' }
                 ]
             })
 
             myTable.on('click', 'td.dt-control', function (e) {
                 let tr = e.target.closest('tr');
@@ -150,17 +150,17 @@
         }
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 
     function openFolder(folder_name) {
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/SharePoint.html` & `GraphSpy-1.2.1/GraphSpy/templates/SharePoint.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         getActiveAccessToken(document.getElementById("sharepoint_form").access_token_id)
     </script>
 </div>
 <br>
 
 <div>
     <h2>Files Table</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created</th>
                 <th>Last Modified</th>
                 <th>File Name</th>
@@ -90,15 +90,15 @@
                 },
                 columns: [
                     {
                         className: 'dt-control',
                         orderable: false,
                         data: null,
                         defaultContent: '',
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         className: 'action-control',
                         orderable: false,
                         data: null,
                         render: function (d, t, r) {
                             if (r.folder) {
@@ -107,28 +107,28 @@
                             } else if (r.file) {
                                 // Download icon
                                 return '<i class="fi fi-br-download" style="cursor: pointer"></i>'
                             }
                             // Question mark icon
                             return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                         },
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         data: 'createdDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     {
                         data: 'lastModifiedDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     { data: 'name' },
                     {
                         data: 'size',
-                        width: '100px'
+                        width: '120px'
                     },
                     { data: 'webUrl' }
                 ]
             })
 
 
             myTable.on('click', 'td.dt-control', function (e) {
@@ -168,17 +168,17 @@
 
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 
     function openFolder(folder_name) {
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/SharePointDrives.html` & `GraphSpy-1.2.1/GraphSpy/templates/SharePointDrives.html`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         getActiveAccessToken(document.getElementById("sharepoint_form").access_token_id)
     </script>
 </div>
 <br>
 
 <div>
     <h2>Drives Table</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created</th>
                 <th>Last Modified</th>
                 <th>Drive Name</th>
@@ -78,35 +78,35 @@
                 },
                 columns: [
                     {
                         className: 'dt-control',
                         orderable: false,
                         data: null,
                         defaultContent: '',
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         className: 'action-control',
                         orderable: false,
                         data: null,
                         render: function (d, t, r) {
                             // Link icon
                             return '<i class="fi fi-br-link-alt" style="cursor: pointer"></i>'
                             // Question mark icon
                             // return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                         },
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         data: 'createdDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     {
                         data: 'lastModifiedDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     { data: 'name' },
                     { data: 'webUrl' }
                 ]
             })
 
             myTable.on('click', 'td.dt-control', function (e) {
@@ -133,17 +133,17 @@
 
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 </script>
 {%endblock content%}
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/SharePointSites.html` & `GraphSpy-1.2.1/GraphSpy/templates/SharePointSites.html`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         getActiveAccessToken(document.getElementById("sharepoint_form").access_token_id)
     </script>
 </div>
 <br>
 
 <div>
     <h2>Sites Table</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created</th>
                 <th>Last Modified</th>
                 <th>Site Name</th>
@@ -75,37 +75,37 @@
                 },
                 columns: [
                     {
                         className: 'dt-control',
                         orderable: false,
                         data: null,
                         defaultContent: '',
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         className: 'action-control',
                         orderable: false,
                         data: null,
                         render: function (d, t, r) {
                             if (r.resource["@odata.type"] == "#microsoft.graph.site") {
                                 // Link icon
                                 return '<i class="fi fi-br-link-alt" style="cursor: pointer"></i>'
                             }
                             // Question mark icon
                             return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                         },
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         data: 'resource.createdDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     {
                         data: 'resource.lastModifiedDateTime',
-                        width: '150px'
+                        width: '175px'
                     },
                     { data: 'resource.name' },
                     { data: 'resource.displayName' },
                     { data: 'resource.webUrl' }
                 ]
             })
 
@@ -137,17 +137,17 @@
         }
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 </script>
 {%endblock content%}
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/access_token_modal.html` & `GraphSpy-1.2.1/GraphSpy/templates/access_token_modal.html`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
                 <h1 class="modal-title fs-5" id="access_token_modal_label">Access Tokens</h1>
                 <div style="float: right">
                     <i class="fi fi-br-expand px-3" id="expand-icon" style="cursor: pointer; float: left; opacity: 0.5"></i>
                     <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                 </div>
             </div>
             <div class="modal-body">
-                <div id="dTable" class="box-body table-responsive" style="padding:20px;">
-                    <table id="access_token_modal_table" class="display" style="width:100%">
+                <div id="dTable" class="box-body table-responsive" style="padding:10px;">
+                    <table id="access_token_modal_table" class="table" style="width:100%">
                         <thead>
                             <tr>
                                 <th></th>
                                 <th></th>
                                 <th></th>
                                 <th></th>
                                 <th>ID</th>
@@ -43,52 +43,52 @@
         },
         columns: [
             {
                 className: 'dt-control',
                 orderable: false,
                 data: null,
                 defaultContent: '',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'active-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'copy-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-copy-alt" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'id', 'width': '30px' },
-            { data: 'issued_at', 'width': '150px' },
-            { data: 'expires_at', 'width': '150px' },
-            { data: 'user', 'width': '350px' },
-            { data: 'resource', 'width': '350px' },
+            { data: 'id', 'width': '60px' },
+            { data: 'issued_at', 'width': '170px' },
+            { data: 'expires_at', 'width': '170px' },
+            { data: 'user', 'width': '370px' },
+            { data: 'resource', 'width': '370px' },
             { data: 'description' }
         ],
         order: [[4, 'desc']],
         autoWidth: false,
         order: [[4, 'desc']],
         createdRow: function (row, data, dataIndex) {
             if (new Date(data.expires_at) > new Date()) {
-                $(row).addClass('bg-success-subtle').addClass('text-success-emphasis');
+                $(row).children().addClass('bg-success-subtle').addClass('text-success-emphasis');
             } else {
-                $(row).addClass('bg-danger-subtle').addClass('text-danger-emphasis');
+                $(row).children().addClass('bg-danger-subtle').addClass('text-danger-emphasis');
             }
         }
     })
 
     accessTokenModalTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
         let row = accessTokenModalTable.row(tr);
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/access_tokens.html` & `GraphSpy-1.2.1/GraphSpy/templates/access_tokens.html`

 * *Files 7% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 <script>
     getActiveAccessToken(document.getElementById("access_token_form").access_token_id);
     getActiveRefreshToken(document.getElementById("refresh_to_access_token_form").refresh_token_id);
 </script>
 <div>
     <br>
     <h1>Access Tokens</h1>
-    <table id="access_tokens" class="display" style="table-layout:fixed; width:100%">
+    <table id="access_tokens" class="table" style="table-layout:fixed; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th></th>
                 <th></th>
                 <th>ID</th>
@@ -121,50 +121,50 @@
         },
         columns: [
             {
                 className: 'dt-control',
                 orderable: false,
                 data: null,
                 defaultContent: '',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'active-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'copy-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-copy-alt" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'id', 'width': '30px' },
-            { data: 'issued_at', 'width': '150px' },
-            { data: 'expires_at', 'width': '150px' },
-            { data: 'user', 'width': '350px' },
-            { data: 'resource', 'width': '350px' },
+            { data: 'id', 'width': '60px' },
+            { data: 'issued_at', 'width': '170px' },
+            { data: 'expires_at', 'width': '170px' },
+            { data: 'user', 'width': '370px' },
+            { data: 'resource', 'width': '370px' },
             { data: 'description' }
         ],
         order: [[4, 'desc']],
         createdRow: function (row, data, dataIndex) {
             if (new Date(data.expires_at) > new Date()) {
-                $(row).addClass('bg-success-subtle').addClass('text-success-emphasis');
+                $(row).children().addClass('bg-success-subtle').addClass('text-success-emphasis');
             } else {
-                $(row).addClass('bg-danger-subtle').addClass('text-danger-emphasis');
+                $(row).children().addClass('bg-danger-subtle').addClass('text-danger-emphasis');
             }
         }
     })
 
     myTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
         let row = myTable.row(tr);
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/custom_requests.html` & `GraphSpy-1.2.1/GraphSpy/templates/custom_requests.html`

 * *Files 10% similar despite different names*

```diff
@@ -81,37 +81,62 @@
     </form>
     <script>
         getActiveAccessToken(document.getElementById("custom_request_form").access_token_id)
     </script>
 </div>
 <br>
 <div class="row" id="response-card" style="display: none">
-    <div class="col-auto">
+    <div class="col-auto" style="min-width:400px">
         <div class="card mt-3">
-            <div class="card-header" style="text-align: center">
-                <b>Response [<span id="response_status_code"></span>]</b>
-                <i class="fi fi-rr-copy-alt" id="copy-icon" style="cursor: pointer; float: right"></i>
+            <div class="card-header">
+                <div class="d-flex justify-content-between">
+                    <div class="btn-group btn-group-sm" role="group">
+                        <button type="button" id="response_card_body_button" class="btn btn-outline-primary active" onclick="toggleResponseCardContent()">Body</button>
+                        <button type="button" id="response_card_headers_button" class="btn btn-outline-primary" onclick="toggleResponseCardContent()">Headers</button>
+                    </div>
+                    <b>Response [<span id="response_status_code"></span>]</b>
+                    <i class="fi fi-rr-copy-alt" id="copy-icon" style="cursor: pointer"></i>
+                </div>
             </div>
             <div class="card-body">
                 <pre id="response_body" class="mb-0"></pre>
+                <div id="response_headers" class="mb-0" style="display: none">
+                    <table id="response_header_table" class="table table-striped table-responsive" style="word-wrap: break-word; word-break: break-all; width:100%">
+                        <thead>
+                            <tr>
+                                <th>Response Header</th>
+                                <th>Value</th>
+                            </tr>
+                        </thead>
+                    </table>
+                </div>
             </div>
         </div>
     </div>
 </div>
+
 <script>
-    function getHeaders() {
+    function toggleResponseCardContent() {
+        $("#response_card_body_button").toggleClass("active");
+        $("#response_card_headers_button").toggleClass("active");
+        $("#response_body").toggle();
+        $("#response_headers").toggle();
+        $("#response_header_table").DataTable().columns.adjust()
+    }
+
+    function getInputHeaders() {
         let headers = {};
         for (const header of $("#header_fields").children()) {
             if (header.getElementsByClassName("header_name")[0].value != "") {
                 headers[header.getElementsByClassName("header_name")[0].value] = header.getElementsByClassName("header_value")[0].value;
             };
         };
         return headers;
     }
-    function getVariables() {
+    function getInputVariables() {
         let variables = {};
         for (const variable of $("#variable_fields").children()) {
             if (variable.getElementsByClassName("variable_name")[0].value != "") {
                 variables[variable.getElementsByClassName("variable_name")[0].value] = variable.getElementsByClassName("variable_value")[0].value;
             };
         };
         return variables;
@@ -128,16 +153,16 @@
             contentType: "application/json; charset=utf-8",
             data: JSON.stringify({
                 "uri": request_form.request_uri.value,
                 "access_token_id": request_form.access_token_id.value,
                 "method": request_form.method.value,
                 "request_type": request_form.request_type.value,
                 "body": request_form.body.value,
-                "headers": getHeaders(),
-                "variables": getVariables()
+                "headers": getInputHeaders(),
+                "variables": getInputVariables()
             }),
             success: null
         });
         if (response.status >= 400) {
             bootstrapAlert(response.responseText, "danger");
             return;
         }
@@ -151,14 +176,39 @@
                 $("#response_body").text(responseJSON.response_text);
             }
         } catch (e) {
             $("#response_body").text(responseJSON.response_text);
         }
         $("#response_status_code").text(responseJSON.response_status_code);
         $("#response-card").show();
+
+        generateRespHeadersTable(responseJSON.response_headers);
+    }
+
+    function generateRespHeadersTable(respHeaders) {
+        if ($.fn.dataTable.isDataTable('#response_header_table')) {
+            $('#response_header_table').DataTable().destroy();
+            $('#response_header_table').empty();
+        }
+        tableData = [];
+        for (const header in respHeaders) {
+            tableData.push({ "header": header, "value": respHeaders[header] })
+        };
+        let respHeadersTable = new DataTable('#response_header_table', {
+            data: tableData,
+            columns: [
+                { data: 'header', title: "Response Header" },
+                { data: 'value', title: "Value" }
+            ],
+            autoWidth: true,
+            info: false,
+            ordering: false,
+            paging: false,
+            searching: false
+        })
     }
 
     function saveRequestTemplate() {
         let request_form = document.getElementById("custom_request_form");
         let response;
         // request_template_name
         response = $.ajax({
@@ -169,16 +219,16 @@
             contentType: "application/json; charset=utf-8",
             data: JSON.stringify({
                 "template_name": $("#request_template_name").val(),
                 "uri": request_form.request_uri.value,
                 "method": request_form.method.value,
                 "request_type": request_form.request_type.value,
                 "body": request_form.body.value,
-                "headers": getHeaders(),
-                "variables": getVariables()
+                "headers": getInputHeaders(),
+                "variables": getInputVariables()
             }),
             success: null
         });
         if (response.status >= 400) {
             bootstrapAlert(response.responseText, "danger");
             return;
         }
@@ -245,16 +295,16 @@
                 <h1 class="modal-title fs-5" id="request_template_modal_label">Request Templates</h1>
                 <div style="float: right">
                     <i class="fi fi-br-expand px-3" id="expand-icon" style="cursor: pointer; float: left; opacity: 0.5"></i>
                     <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                 </div>
             </div>
             <div class="modal-body">
-                <div id="dTable" class="box-body table-responsive" style="padding:20px;">
-                    <table id="request_templates" class="display" style="width:100%">
+                <div id="dTable" class="box-body table-responsive" style="padding:10px;">
+                    <table id="request_templates" class="table table-striped" style="width:100%">
                         <thead>
                             <tr>
                                 <th></th>
                                 <th></th>
                                 <th></th>
                                 <th>ID</th>
                                 <th>Name</th>
@@ -280,34 +330,34 @@
         },
         columns: [
             {
                 className: 'dt-control',
                 orderable: false,
                 data: null,
                 defaultContent: '',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'active-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'id', 'width': '30px' },
-            { data: 'template_name', 'width': '150px' },
-            { data: 'request_type', 'width': '130px' },
-            { data: 'method', 'width': '80px' },
+            { data: 'id', 'width': '60px' },
+            { data: 'template_name', 'width': '170px' },
+            { data: 'request_type', 'width': '150px' },
+            { data: 'method', 'width': '100px' },
             { data: 'uri' }
         ],
         order: [[3, 'desc']],
         autoWidth: false
     })
 
     myTable.on('click', 'td.dt-control', function (e) {
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/device_codes.html` & `GraphSpy-1.2.1/GraphSpy/templates/device_codes.html`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         </div>
     </form>
 </div>
 <br>
 <div>
     <h1>Device Code List</h1>
     <button type="button" class="btn btn-primary" onclick="restartDeviceCodePolling()">Restart Polling</button>
-    <table id="device_codes" class="display" style="table-layout:fixed; width:100%">
+    <table id="device_codes" class="table" style="table-layout:fixed; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th></th>
                 <th>ID</th>
                 <th>Generated At</th>
@@ -65,49 +65,49 @@
         },
         columns: [
             {
                 className: 'dt-control',
                 orderable: false,
                 data: null,
                 defaultContent: '',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'copy-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-copy-alt" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'id', 'width': '30px' },
-            { data: 'generated_at', 'width': '150px' },
-            { data: 'expires_at', 'width': '150px' },
-            { data: 'last_poll', 'width': '150px' },
-            { data: 'user_code', 'width': '125px' },
-            { data: 'client_id', 'width': '310px' },
+            { data: 'id', 'width': '60px' },
+            { data: 'generated_at', 'width': '170px' },
+            { data: 'expires_at', 'width': '170px' },
+            { data: 'last_poll', 'width': '170px' },
+            { data: 'user_code', 'width': '145px' },
+            { data: 'client_id', 'width': '330px' },
             { data: 'status' }
         ],
         order: [[3, 'desc']],
         createdRow: function (row, data, dataIndex) {
             switch (data.status) {
                 case "SUCCESS":
-                    $(row).addClass('bg-success-subtle').addClass('text-success-emphasis');
+                    $(row).children().addClass('bg-success-subtle').addClass('text-success-emphasis');
                     break;
                 case "EXPIRED":
-                    $(row).addClass('bg-danger-subtle').addClass('text-danger-emphasis');
+                    $(row).children().addClass('bg-danger-subtle').addClass('text-danger-emphasis');
                     break;
                 default:
-                    $(row).addClass('bg-primary-subtle').addClass('text-primary-emphasis');
+                    $(row).children().addClass('bg-primary-subtle').addClass('text-primary-emphasis');
             }
         }
     })
 
     myTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
         let row = myTable.row(tr);
@@ -133,15 +133,14 @@
         let row = myTable.row(tr);
         if (!confirm("Are you sure you want to delete device code with ID " + row.data().id + "?")) { return }
         deleteDeviceCode(row.data().id);
     });
 
     function format(d) {
         return (
-            //'<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
             '<dl>' +
             '<dt>Device Code:</dt>' +
             '<dd><code>' +
             d.device_code +
             '</code></dd>' +
             '</dl>'
         );
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/generic_search.html` & `GraphSpy-1.2.1/GraphSpy/templates/generic_search.html`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 <option value="list">Lists</option>
                 <option value="listItem">List Items</option>
             </datalist>
         </div>
         <div class="col-sm-4">
             <label for="search_limit" class="form-label">Limit *</label>
             <input type="text" id="search_limit" name="search_limit" class="form-control" value="25" required>
-            <i class="form-text">Max 1000</i>
+            <i class="form-text">Max 500</i>
         </div>
         <div class="col-sm-4">
             <label for="access_token_id" class="form-label">Access token id *</label>
             <div class="input-group">
                 <input type="text" id="access_token_id" name="access_token_id" class="form-control" required>
                 <button class="btn btn-outline-primary" type="button" data-bs-toggle="modal" data-bs-target="#access_token_modal" onclick="$('#access_token_modal_table').DataTable().ajax.reload(null, false)">Select...</button>
             </div>
@@ -44,15 +44,15 @@
         getActiveAccessToken(document.getElementById("search_form").access_token_id)
     </script>
 </div>
 <br>
 
 <div>
     <h2>Response</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created User</th>
                 <th>Name</th>
                 <th>Summary</th>
@@ -89,15 +89,15 @@
                 colReorder: true,
                 columns: [
                     {
                         className: 'dt-control',
                         orderable: false,
                         data: null,
                         defaultContent: '',
-                        'width': '20px'
+                        'width': '40px'
                     },
                     {
                         className: 'action-control',
                         orderable: false,
                         data: null,
                         render: function (d, t, r) {
                             if (r.resource.hasOwnProperty("parentReference") && r.resource.parentReference.driveId) {
@@ -106,15 +106,15 @@
                             } else if (r.resource["@odata.type"] == "#microsoft.graph.drive") {
                                 // Link icon
                                 return '<i class="fi fi-br-link-alt" style="cursor: pointer"></i>'
                             }
                             // Question mark icon
                             return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                         },
-                        'width': '20px'
+                        'width': '40px'
                     },
                     { data: 'resource.createdBy.user.displayName' },
                     { data: 'resource.name' },
                     {
                         data: 'summary',
                         render: function (d, t, r) {
                             return d.replaceAll("<c0>", "<b>").replaceAll("</c0>", "</b>")
@@ -158,17 +158,17 @@
         }
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 </script>
 {%endblock content%}
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 Files, folders, pages, and news
 Email message
 Teams messages
 Calendar events
 Sharepoint Sites
 Lists
 List Items
-Limit * [25                  ]Max 1000
+Limit * [25                  ]Max 500
 Access token id *
 [access_token_id     ]Select...
 Search Query *[*                   ]
 Request
 
 ********** RReessppoonnssee **********
   CCrreeaatteedd UUsseerr NNaammee SSuummmmaarryy UURRLL
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/index.html` & `GraphSpy-1.2.1/GraphSpy/templates/index.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/layout.html` & `GraphSpy-1.2.1/GraphSpy/templates/layout.html`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,24 @@
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
     <!-- UIcons by Flaticon (https://www.flaticon.com/uicons) -->
     <link rel='stylesheet' href='https://cdn-uicons.flaticon.com/2.0.0/uicons-regular-rounded/css/uicons-regular-rounded.css'>
     <link rel='stylesheet' href='https://cdn-uicons.flaticon.com/2.0.0/uicons-solid-rounded/css/uicons-solid-rounded.css'>
     <link rel='stylesheet' href='https://cdn-uicons.flaticon.com/2.0.0/uicons-bold-rounded/css/uicons-bold-rounded.css'>
     <!-- DataTables & jQuery -->
-    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.13.5/css/jquery.dataTables.min.css">
+    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/2.0.7/css/dataTables.bootstrap5.css">
+    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/select/2.0.1/css/select.bootstrap5.min.css">
+    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/buttons/3.0.2/css/buttons.bootstrap5.min.css">
     <script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-3.5.1.js"></script>
-    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.11.1/js/jquery.dataTables.min.js"></script>
-    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.11.1/js/dataTables.bootstrap5.min.js"></script>
+    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/2.0.7/js/dataTables.js"></script>
+    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/2.0.7/js/dataTables.bootstrap5.js"></script>
+    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/select/2.0.2/js/dataTables.select.min.js"></script>
+    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/select/2.0.1/js/select.bootstrap5.min.js"></script>
+    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/3.0.2/js/dataTables.buttons.min.js"></script>
+    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/3.0.2/js/buttons.bootstrap5.min.js"></script>
     <!-- DOMPurify -->
     <script type="text/javascript" language="javascript" src="{{url_for('static', filename='js/purify.min.js')}}"></script>
     <!-- Static JS $ CSS -->
     <script type="text/javascript" language="javascript" src="{{url_for('static', filename='js/theme.js')}}"></script>
     <script type="text/javascript" language="javascript" src="{{url_for('static', filename='js/functions.js')}}"></script>
     <link rel="stylesheet" type="text/css" href="{{url_for('static', filename='css/style.css')}}">
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/outlook.html` & `GraphSpy-1.2.1/GraphSpy/templates/outlook.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/recent_files.html` & `GraphSpy-1.2.1/GraphSpy/templates/recent_files.html`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     <script>
         getActiveAccessToken(document.getElementById("recent_file_form").access_token_id)
     </script>
 </div>
 <br>
 <div>
     <h2>Files</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created</th>
                 <th>Last Modified</th>
                 <th>File Name</th>
@@ -58,15 +58,15 @@
             },
             columns: [
                 {
                     className: 'dt-control',
                     orderable: false,
                     data: null,
                     defaultContent: '',
-                    'width': '20px'
+                    'width': '40px'
                 },
                 {
                     className: 'action-control',
                     orderable: false,
                     data: null,
                     render: function (d, t, r) {
                         if (r.folder) {
@@ -75,28 +75,28 @@
                         } else if (r.file) {
                             // Download icon
                             return '<i class="fi fi-br-download" style="cursor: pointer"></i>'
                         }
                         // Question mark icon
                         return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                     },
-                    'width': '20px'
+                    'width': '40px'
                 },
                 {
                     data: 'createdDateTime',
-                    width: '150px'
+                    width: '175px'
                 },
                 {
                     data: 'lastModifiedDateTime',
-                    width: '150px'
+                    width: '175px'
                 },
                 { data: 'name' },
                 {
                     data: 'size',
-                    width: '100px'
+                    width: '120px'
                 },
                 { data: 'webUrl' }
             ],
             order: [[2, 'desc']]
         })
 
         myTable.on('click', 'td.dt-control', function (e) {
@@ -124,17 +124,17 @@
         });
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 </script>
 {%endblock content%}
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/refresh_token_modal.html` & `GraphSpy-1.2.1/GraphSpy/templates/refresh_token_modal.html`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
                 <h1 class="modal-title fs-5" id="refresh_token_modal_label">Refresh Tokens</h1>
                 <div style="float: right">
                     <i class="fi fi-br-expand px-3" id="expand-icon" style="cursor: pointer; float: left; opacity: 0.5"></i>
                     <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                 </div>
             </div>
             <div class="modal-body">
-                <div id="dTable" class="box-body table-responsive" style="padding:20px;">
-                    <table id="refresh_token_modal_table" class="display" style="width:100%">
+                <div id="dTable" class="box-body table-responsive" style="padding:10px;">
+                    <table id="refresh_token_modal_table" class="table table-striped" style="width:100%">
                         <thead>
                             <tr>
                                 <th></th>
                                 <th></th>
                                 <th></th>
                                 <th></th>
                                 <th>ID</th>
@@ -44,43 +44,43 @@
         },
         columns: [
             {
                 className: 'dt-control',
                 orderable: false,
                 data: null,
                 defaultContent: '',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'active-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'copy-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-copy-alt" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'id', 'width': '30px' },
-            { data: 'stored_at', 'width': '150px' },
-            { data: 'user', 'width': '300px' },
-            { data: 'tenant_id', 'width': '300px' },
-            { data: 'resource', 'width': '300px' },
-            { data: 'foci', 'width': '30px' },
+            { data: 'id', 'width': '60px' },
+            { data: 'stored_at', 'width': '170px' },
+            { data: 'user', 'width': '320px' },
+            { data: 'tenant_id', 'width': '320px' },
+            { data: 'resource', 'width': '320px' },
+            { data: 'foci', 'width': '50px' },
             { data: 'description' }
         ],
         order: [[4, 'desc']],
         autoWidth: false
     })
 
     refreshTokenModalTable.on('click', 'td.dt-control', function (e) {
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/refresh_tokens.html` & `GraphSpy-1.2.1/GraphSpy/templates/refresh_tokens.html`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 </div>
 <script>
     getActiveRefreshToken(document.getElementById("refresh_token_form").refresh_token_id);
 </script>
 <br>
 <div>
     <h1>Refresh Tokens</h1>
-    <table id="refresh_tokens" class="display" style="table-layout:fixed; width:100%">
+    <table id="refresh_tokens" class="table table-striped" style="table-layout:fixed; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th></th>
                 <th></th>
                 <th>ID</th>
@@ -90,43 +90,43 @@
         },
         columns: [
             {
                 className: 'dt-control',
                 orderable: false,
                 data: null,
                 defaultContent: '',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'active-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'copy-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-copy-alt" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'id', 'width': '30px' },
-            { data: 'stored_at', 'width': '150px' },
-            { data: 'user', 'width': '300px' },
-            { data: 'tenant_id', 'width': '300px' },
-            { data: 'resource', 'width': '300px' },
-            { data: 'foci', 'width': '30px' },
+            { data: 'id', 'width': '60px' },
+            { data: 'stored_at', 'width': '170px' },
+            { data: 'user', 'width': '320px' },
+            { data: 'tenant_id', 'width': '320px' },
+            { data: 'resource', 'width': '320px' },
+            { data: 'foci', 'width': '50px' },
             { data: 'description' }
         ],
         order: [[4, 'desc']]
     })
 
     myTable.on('click', 'td.dt-control', function (e) {
         let tr = e.target.closest('tr');
@@ -160,15 +160,14 @@
         if (!confirm("Are you sure you want to delete refresh token with ID " + row.data().id + "?")) { return }
         deleteRefreshToken(row.data().id);
         $('#refresh_tokens').DataTable().ajax.reload(null, false);
     });
 
     function format(d) {
         return (
-            //'<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
             '<dl>' +
             '<dt>Raw Token:</dt>' +
             '<dd><code>' +
             d.refreshtoken +
             '</code></dd>' +
             '</dl>'
         );
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/settings.html` & `GraphSpy-1.2.1/GraphSpy/templates/settings.html`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         <h1>Databases</h1>
         <div class="col-md-9">
             <div class="input-group">
                 <span class="input-group-text">Database Folder</span>
                 <input class="form-control" id="db_folder" type="text" value="{{ config['graph_spy_db_folder'] }}" readonly>
             </div>
         </div>
-        <table id="databases" class="display" style="table-layout:fixed; width:100%">
+        <table id="databases" class="table table-striped" style="table-layout:fixed; width:100%">
             <thead>
                 <tr>
                     <th></th>
                     <th></th>
                     <th></th>
                     <th>Last Modified</th>
                     <th>Size</th>
@@ -110,33 +110,33 @@
         },
         columns: [
             {
                 className: 'active-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-br-check" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'duplicate-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-duplicate" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
             {
                 className: 'delete-control',
                 orderable: false,
                 data: null,
                 defaultContent: '<i class="fi fi-rr-trash" style="cursor: pointer"></i>',
-                'width': '20px'
+                'width': '40px'
             },
-            { data: 'last_modified', 'width': '150px' },
-            { data: 'size', 'width': '75px' },
-            { data: 'state', 'width': '75px' },
+            { data: 'last_modified', 'width': '170px' },
+            { data: 'size', 'width': '100px' },
+            { data: 'state', 'width': '100px' },
             { data: 'name' }
         ],
         order: [[5, 'asc'], [3, 'desc']]
     })
 
     myTable.on('click', 'td.active-control', function (e) {
         let tr = e.target.closest('tr');
```

### Comparing `GraphSpy-1.2.0/GraphSpy/templates/shared_with_me.html` & `GraphSpy-1.2.1/GraphSpy/templates/shared_with_me.html`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     <script>
         getActiveAccessToken(document.getElementById("shared_file_form").access_token_id)
     </script>
 </div>
 <br>
 <div>
     <h2>Files</h2>
-    <table id="response_table" class="display" style="word-wrap: break-word; word-break: break-all; width:100%">
+    <table id="response_table" class="table table-striped" style="word-wrap: break-word; word-break: break-all; width:100%">
         <thead>
             <tr>
                 <th></th>
                 <th></th>
                 <th>Created</th>
                 <th>Last Modified</th>
                 <th>File Name</th>
@@ -58,15 +58,15 @@
             },
             columns: [
                 {
                     className: 'dt-control',
                     orderable: false,
                     data: null,
                     defaultContent: '',
-                    'width': '20px'
+                    'width': '40px'
                 },
                 {
                     className: 'action-control',
                     orderable: false,
                     data: null,
                     render: function (d, t, r) {
                         if (r.folder) {
@@ -75,28 +75,28 @@
                         } else if (r.file) {
                             // Download icon
                             return '<i class="fi fi-br-download" style="cursor: pointer"></i>'
                         }
                         // Question mark icon
                         return '<i class="fi fi-br-question" style="cursor: pointer"></i>'
                     },
-                    'width': '20px'
+                    'width': '40px'
                 },
                 {
                     data: 'createdDateTime',
-                    width: '150px'
+                    width: '175px'
                 },
                 {
                     data: 'lastModifiedDateTime',
-                    width: '150px'
+                    width: '175px'
                 },
                 { data: 'name' },
                 {
                     data: 'size',
-                    width: '100px'
+                    width: '120px'
                 },
                 { data: 'webUrl' }
             ],
             order: [[2, 'desc']]
         })
 
         myTable.on('click', 'td.dt-control', function (e) {
@@ -124,17 +124,17 @@
         });
         return false;
     }
 
     function format(d) {
         // `d` is the original data object for the row
         return (
-            '<dl style = "word-wrap: break-word; word-break: break-all; width:100%">' +
+            '<dl>' +
             '<dt>Raw File Info:</dt>' +
-            '<dd><pre>' +
+            '<dd><pre style="white-space: pre-wrap;">' +
             JSON.stringify(d, undefined, 4) +
             '</pre></dd>' +
             '</dl>'
         );
     }
 </script>
 {%endblock content%}
```

### Comparing `GraphSpy-1.2.0/GraphSpy.egg-info/PKG-INFO` & `GraphSpy-1.2.1/GraphSpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPi Version](https://img.shields.io/pypi/v/GraphSpy.svg)](https://pypi.org/project/GraphSpy/)
```

### Comparing `GraphSpy-1.2.0/GraphSpy.egg-info/SOURCES.txt` & `GraphSpy-1.2.1/GraphSpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/LICENSE.txt` & `GraphSpy-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/PKG-INFO` & `GraphSpy-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPi Version](https://img.shields.io/pypi/v/GraphSpy.svg)](https://pypi.org/project/GraphSpy/)
```

### Comparing `GraphSpy-1.2.0/README.md` & `GraphSpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.2.0/setup.py` & `GraphSpy-1.2.1/setup.py`

 * *Files identical despite different names*

