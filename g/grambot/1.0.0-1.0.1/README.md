# Comparing `tmp/grambot-1.0.0.tar.gz` & `tmp/grambot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grambot-1.0.0.tar", last modified: Sun Jun  2 16:51:13 2024, max compression
+gzip compressed data, was "grambot-1.0.1.tar", last modified: Sun Jun  2 17:08:28 2024, max compression
```

## Comparing `grambot-1.0.0.tar` & `grambot-1.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.987285 grambot-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    35551 2024-06-01 16:53:32.000000 grambot-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2345 2024-06-02 16:51:12.987285 grambot-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1442 2024-06-02 16:37:37.000000 grambot-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.937285 grambot-1.0.0/grambot/
--rw-r--r--   0 root         (0) root         (0)     1092 2024-06-02 16:40:40.000000 grambot-1.0.0/grambot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1753 2024-06-02 12:42:13.000000 grambot-1.0.0/grambot/apiClient.py
--rw-r--r--   0 root         (0) root         (0)     1288 2024-06-01 19:20:38.000000 grambot-1.0.0/grambot/cache.py
--rw-r--r--   0 root         (0) root         (0)     1675 2024-06-02 12:42:36.000000 grambot-1.0.0/grambot/exception.py
--rw-r--r--   0 root         (0) root         (0)     3882 2024-06-02 16:37:37.000000 grambot-1.0.0/grambot/gramClient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.937285 grambot-1.0.0/grambot/method/
--rw-r--r--   0 root         (0) root         (0)     1030 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.937285 grambot-1.0.0/grambot/method/chats/
--rw-r--r--   0 root         (0) root         (0)     1007 2024-06-02 15:37:39.000000 grambot-1.0.0/grambot/method/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2024-06-02 10:38:26.000000 grambot-1.0.0/grambot/method/chats/getChat.py
--rw-r--r--   0 root         (0) root         (0)     1387 2024-06-02 16:19:40.000000 grambot-1.0.0/grambot/method/chats/getChatAdministrators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.947285 grambot-1.0.0/grambot/method/messages/
--rw-r--r--   0 root         (0) root         (0)      937 2024-06-01 19:20:38.000000 grambot-1.0.0/grambot/method/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2205 2024-06-02 11:30:24.000000 grambot-1.0.0/grambot/method/messages/forwardMessage.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/messages/sendMessage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.957285 grambot-1.0.0/grambot/method/user/
--rw-r--r--   0 root         (0) root         (0)      131 2024-06-02 15:36:47.000000 grambot-1.0.0/grambot/method/user/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/user/getMe.py
--rw-r--r--   0 root         (0) root         (0)     1307 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/user/getUser.py
--rw-r--r--   0 root         (0) root         (0)     1482 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/user/getUserProfilePhotos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.957285 grambot-1.0.0/grambot/method/utils/
--rw-r--r--   0 root         (0) root         (0)      105 2024-06-02 12:02:54.000000 grambot-1.0.0/grambot/method/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/utils/start.py
--rw-r--r--   0 root         (0) root         (0)     2388 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/method/utils/webhook.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-06-02 16:36:27.000000 grambot-1.0.0/grambot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.967285 grambot-1.0.0/grambot/types/
--rw-r--r--   0 root         (0) root         (0)      972 2024-06-02 11:30:24.000000 grambot-1.0.0/grambot/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.967285 grambot-1.0.0/grambot/types/business/
--rw-r--r--   0 root         (0) root         (0)      178 2024-06-02 12:01:50.000000 grambot-1.0.0/grambot/types/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2024-06-02 11:30:24.000000 grambot-1.0.0/grambot/types/business/businessConnection.py
--rw-r--r--   0 root         (0) root         (0)     1382 2024-06-02 13:42:57.000000 grambot-1.0.0/grambot/types/business/businessDeleteMessage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.967285 grambot-1.0.0/grambot/types/chats/
--rw-r--r--   0 root         (0) root         (0)      100 2024-06-02 16:16:16.000000 grambot-1.0.0/grambot/types/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1725 2024-06-02 13:42:57.000000 grambot-1.0.0/grambot/types/chats/chatFullInfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.977285 grambot-1.0.0/grambot/types/chats/chatMember/
--rw-r--r--   0 root         (0) root         (0)     1388 2024-06-02 16:17:34.000000 grambot-1.0.0/grambot/types/chats/chatMember/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2383 2024-06-02 16:20:57.000000 grambot-1.0.0/grambot/types/chats/chatMember/chatMemberAdministrator.py
--rw-r--r--   0 root         (0) root         (0)     1105 2024-06-02 16:37:37.000000 grambot-1.0.0/grambot/types/chats/chatMember/chatMemberBanned.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-06-02 16:37:37.000000 grambot-1.0.0/grambot/types/chats/chatMember/chatMemberLeft.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-06-02 16:16:16.000000 grambot-1.0.0/grambot/types/chats/chatMember/chatMemberOwner.py
--rw-r--r--   0 root         (0) root         (0)     2407 2024-06-02 16:16:16.000000 grambot-1.0.0/grambot/types/chats/chatMember/chatMemberRestricted.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-06-02 16:16:16.000000 grambot-1.0.0/grambot/types/chats/chatMember/chatMembersMember.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.987285 grambot-1.0.0/grambot/types/keyboard/
--rw-r--r--   0 root         (0) root         (0)       93 2024-06-02 10:38:26.000000 grambot-1.0.0/grambot/types/keyboard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1483 2024-06-02 10:38:26.000000 grambot-1.0.0/grambot/types/keyboard/replyKeyboardMarkup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.987285 grambot-1.0.0/grambot/types/messages/
--rw-r--r--   0 root         (0) root         (0)       59 2024-06-02 10:38:26.000000 grambot-1.0.0/grambot/types/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6447 2024-06-02 13:42:57.000000 grambot-1.0.0/grambot/types/messages/message.py
--rw-r--r--   0 root         (0) root         (0)     4118 2024-06-02 13:44:03.000000 grambot-1.0.0/grambot/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.987285 grambot-1.0.0/grambot/types/users/
--rw-r--r--   0 root         (0) root         (0)      125 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/types/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-06-02 10:38:26.000000 grambot-1.0.0/grambot/types/users/user.py
--rw-r--r--   0 root         (0) root         (0)     1277 2024-06-02 15:35:40.000000 grambot-1.0.0/grambot/types/users/userProfilePhotos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 16:51:12.937285 grambot-1.0.0/grambot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2345 2024-06-02 16:51:12.000000 grambot-1.0.0/grambot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1669 2024-06-02 16:51:12.000000 grambot-1.0.0/grambot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 16:51:12.000000 grambot-1.0.0/grambot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 16:51:12.000000 grambot-1.0.0/grambot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2024-06-02 16:51:12.000000 grambot-1.0.0/grambot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-06-02 16:51:12.000000 grambot-1.0.0/grambot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-02 16:51:12.987285 grambot-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1710 2024-06-02 16:37:37.000000 grambot-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.999047 grambot-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35551 2024-06-02 17:08:23.000000 grambot-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-06-02 17:08:27.999047 grambot-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-06-02 17:08:23.000000 grambot-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.991047 grambot-1.0.1/grambot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/apiClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/gramClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.991047 grambot-1.0.1/grambot/method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/method/chats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/chats/getChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/chats/getChatAdministrators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/method/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/messages/forwardMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/messages/sendMessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/method/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/user/getMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/user/getUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/user/getUserProfilePhotos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/method/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/utils/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/method/utils/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/types/business/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/business/businessConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/business/businessDeleteMessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.995046 grambot-1.0.1/grambot/types/chats/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatFullInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.999047 grambot-1.0.1/grambot/types/chats/chatMember/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/chatMemberAdministrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/chatMemberBanned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/chatMemberLeft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/chatMemberOwner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/chatMemberRestricted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/chats/chatMember/chatMembersMember.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.999047 grambot-1.0.1/grambot/types/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/keyboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/keyboard/replyKeyboardMarkup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.999047 grambot-1.0.1/grambot/types/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/messages/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.999047 grambot-1.0.1/grambot/types/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/users/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-06-02 17:08:23.000000 grambot-1.0.1/grambot/types/users/userProfilePhotos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:08:27.999047 grambot-1.0.1/grambot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-06-02 17:08:27.000000 grambot-1.0.1/grambot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-06-02 17:08:27.000000 grambot-1.0.1/grambot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:08:27.000000 grambot-1.0.1/grambot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:08:27.000000 grambot-1.0.1/grambot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 17:08:27.000000 grambot-1.0.1/grambot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 17:08:27.000000 grambot-1.0.1/grambot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:08:27.999047 grambot-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-02 17:08:23.000000 grambot-1.0.1/setup.py
```

### Comparing `grambot-1.0.0/LICENSE` & `grambot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/PKG-INFO` & `grambot-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grambot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Grambot Based Library For Your Telegram Bot.
 Home-page: https://github.com/AyiinXd/grambot
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/grambot/issues
 Project-URL: Source Code, https://github.com/AyiinXd/grambot
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: asyncio
+Requires-Dist: requests
 
 # Grambot Package
 
 <p align="center">
   <img src="https://telegra.ph//file/897863d5713e6b0b5ec58.jpg">
 </p>
```

### Comparing `grambot-1.0.0/README.md` & `grambot-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/__init__.py` & `grambot-1.0.1/grambot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 # ===========================================================
 
 from .gramClient import GramClient
 
 __all__ = ["GramClient"]
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "GramBot - Copyright (C) 2024 - AyiinXd <https://github.com/AyiinXd>"
```

### Comparing `grambot-1.0.0/grambot/apiClient.py` & `grambot-1.0.1/grambot/apiClient.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/cache.py` & `grambot-1.0.1/grambot/cache.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/exception.py` & `grambot-1.0.1/grambot/exception.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/gramClient.py` & `grambot-1.0.1/grambot/gramClient.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/__init__.py` & `grambot-1.0.1/grambot/method/__init__.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/chats/__init__.py` & `grambot-1.0.1/grambot/method/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/chats/getChat.py` & `grambot-1.0.1/grambot/method/chats/getChat.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/chats/getChatAdministrators.py` & `grambot-1.0.1/grambot/method/chats/getChatAdministrators.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/messages/__init__.py` & `grambot-1.0.1/grambot/method/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/messages/forwardMessage.py` & `grambot-1.0.1/grambot/method/messages/forwardMessage.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/messages/sendMessage.py` & `grambot-1.0.1/grambot/method/messages/sendMessage.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/user/getMe.py` & `grambot-1.0.1/grambot/method/user/getMe.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/user/getUser.py` & `grambot-1.0.1/grambot/method/user/getUser.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/user/getUserProfilePhotos.py` & `grambot-1.0.1/grambot/method/user/getUserProfilePhotos.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/utils/start.py` & `grambot-1.0.1/grambot/method/utils/start.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/method/utils/webhook.py` & `grambot-1.0.1/grambot/method/utils/webhook.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/__init__.py` & `grambot-1.0.1/grambot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/business/businessConnection.py` & `grambot-1.0.1/grambot/types/business/businessConnection.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/business/businessDeleteMessage.py` & `grambot-1.0.1/grambot/types/business/businessDeleteMessage.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatFullInfo.py` & `grambot-1.0.1/grambot/types/chats/chatFullInfo.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/__init__.py` & `grambot-1.0.1/grambot/types/chats/chatMember/__init__.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/chatMemberAdministrator.py` & `grambot-1.0.1/grambot/types/chats/chatMember/chatMemberAdministrator.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/chatMemberBanned.py` & `grambot-1.0.1/grambot/types/chats/chatMember/chatMemberBanned.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/chatMemberLeft.py` & `grambot-1.0.1/grambot/types/chats/chatMember/chatMemberLeft.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/chatMemberOwner.py` & `grambot-1.0.1/grambot/types/chats/chatMember/chatMemberOwner.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/chatMemberRestricted.py` & `grambot-1.0.1/grambot/types/chats/chatMember/chatMemberRestricted.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/chats/chatMember/chatMembersMember.py` & `grambot-1.0.1/grambot/types/chats/chatMember/chatMembersMember.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/keyboard/replyKeyboardMarkup.py` & `grambot-1.0.1/grambot/types/keyboard/replyKeyboardMarkup.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/messages/message.py` & `grambot-1.0.1/grambot/types/messages/message.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/update.py` & `grambot-1.0.1/grambot/types/update.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/users/user.py` & `grambot-1.0.1/grambot/types/users/user.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot/types/users/userProfilePhotos.py` & `grambot-1.0.1/grambot/types/users/userProfilePhotos.py`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/grambot.egg-info/PKG-INFO` & `grambot-1.0.1/grambot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grambot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Grambot Based Library For Your Telegram Bot.
 Home-page: https://github.com/AyiinXd/grambot
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/grambot/issues
 Project-URL: Source Code, https://github.com/AyiinXd/grambot
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: asyncio
+Requires-Dist: requests
 
 # Grambot Package
 
 <p align="center">
   <img src="https://telegra.ph//file/897863d5713e6b0b5ec58.jpg">
 </p>
```

### Comparing `grambot-1.0.0/grambot.egg-info/SOURCES.txt` & `grambot-1.0.1/grambot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grambot-1.0.0/setup.py` & `grambot-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 
 from setuptools import find_packages, setup
 
 
-with open("requirements.txt", encoding="utf-8") as r:
-    requirements = [i.strip() for i in r]
+requirements = [
+    "asyncio",
+    "requests"
+]
 
 with open("grambot/__init__.py", "rt", encoding="utf8") as x:
     version = re.search(r'__version__ = "(.*?)"', x.read()).group(1)
 
 with open("grambot/__init__.py", "rt", encoding="utf8") as x:
     license = re.search(r'__license__ = "(.*?)"', x.read()).group(1)
```

