# Comparing `tmp/pybalebot-0.0.2.tar.gz` & `tmp/pybalebot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybalebot-0.0.2.tar", last modified: Wed May 29 12:43:58 2024, max compression
+gzip compressed data, was "pybalebot-0.0.3.tar", last modified: Sun Jun  2 14:04:27 2024, max compression
```

## Comparing `pybalebot-0.0.2.tar` & `pybalebot-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.838329 pybalebot-0.0.2/
--rw-rw-rw-   0        0        0     3048 2024-05-29 12:43:58.837354 pybalebot-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1888 2024-05-29 12:43:10.000000 pybalebot-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.781659 pybalebot-0.0.2/pybalebot/
--rw-rw-rw-   0        0        0      112 2024-05-29 12:43:40.000000 pybalebot-0.0.2/pybalebot/__init__.py
--rw-rw-rw-   0        0        0     4136 2024-05-29 12:38:23.000000 pybalebot-0.0.2/pybalebot/api.py
--rw-rw-rw-   0        0        0     2004 2024-05-29 12:36:03.000000 pybalebot-0.0.2/pybalebot/client.py
--rw-rw-rw-   0        0        0      357 2024-05-28 18:40:53.000000 pybalebot-0.0.2/pybalebot/errors.py
--rw-rw-rw-   0        0        0    12012 2024-05-29 12:36:09.000000 pybalebot-0.0.2/pybalebot/filters.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.810965 pybalebot-0.0.2/pybalebot/methods/
--rw-rw-rw-   0        0        0      198 2024-05-29 12:33:52.000000 pybalebot-0.0.2/pybalebot/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.818773 pybalebot-0.0.2/pybalebot/methods/chats/
--rw-rw-rw-   0        0        0      564 2024-05-29 10:35:30.000000 pybalebot-0.0.2/pybalebot/methods/chats/__init__.py
--rw-rw-rw-   0        0        0      332 2024-05-29 09:26:07.000000 pybalebot-0.0.2/pybalebot/methods/chats/ban_chat_member.py
--rw-rw-rw-   0        0        0      236 2024-05-29 09:50:52.000000 pybalebot-0.0.2/pybalebot/methods/chats/get_chat.py
--rw-rw-rw-   0        0        0      291 2024-05-29 10:35:12.000000 pybalebot-0.0.2/pybalebot/methods/chats/get_chat_administrators.py
--rw-rw-rw-   0        0        0      283 2024-05-29 09:54:53.000000 pybalebot-0.0.2/pybalebot/methods/chats/get_chat_member_count.py
--rw-rw-rw-   0        0        0      275 2024-05-29 09:47:43.000000 pybalebot-0.0.2/pybalebot/methods/chats/leave_chat.py
--rw-rw-rw-   0        0        0      344 2024-05-29 09:37:50.000000 pybalebot-0.0.2/pybalebot/methods/chats/promote_chat_member.py
--rw-rw-rw-   0        0        0      326 2024-05-29 09:43:41.000000 pybalebot-0.0.2/pybalebot/methods/chats/set_chat_photo.py
--rw-rw-rw-   0        0        0      473 2024-05-29 09:29:10.000000 pybalebot-0.0.2/pybalebot/methods/chats/unban_chat_member.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.822714 pybalebot-0.0.2/pybalebot/methods/messages/
--rw-rw-rw-   0        0        0      394 2024-05-29 09:34:58.000000 pybalebot-0.0.2/pybalebot/methods/messages/__init__.py
--rw-rw-rw-   0        0        0      455 2024-05-29 07:46:15.000000 pybalebot-0.0.2/pybalebot/methods/messages/copy_message.py
--rw-rw-rw-   0        0        0      340 2024-05-29 09:34:04.000000 pybalebot-0.0.2/pybalebot/methods/messages/delete_message.py
--rw-rw-rw-   0        0        0      416 2024-05-28 21:39:07.000000 pybalebot-0.0.2/pybalebot/methods/messages/edit_message_text.py
--rw-rw-rw-   0        0        0      464 2024-05-29 07:43:58.000000 pybalebot-0.0.2/pybalebot/methods/messages/forward_message.py
--rw-rw-rw-   0        0        0      768 2024-05-29 12:32:00.000000 pybalebot-0.0.2/pybalebot/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     2032 2024-05-29 08:44:35.000000 pybalebot-0.0.2/pybalebot/methods/messages/send_photo.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.827594 pybalebot-0.0.2/pybalebot/methods/updates/
--rw-rw-rw-   0        0        0      261 2024-05-29 12:38:10.000000 pybalebot-0.0.2/pybalebot/methods/updates/__init__.py
--rw-rw-rw-   0        0        0      296 2024-05-28 20:42:52.000000 pybalebot-0.0.2/pybalebot/methods/updates/get_updates.py
--rw-rw-rw-   0        0        0      157 2024-05-29 07:34:51.000000 pybalebot-0.0.2/pybalebot/methods/updates/get_webhook_info.py
--rw-rw-rw-   0        0        0      181 2024-05-29 07:32:36.000000 pybalebot-0.0.2/pybalebot/methods/updates/set_webhook.py
--rw-rw-rw-   0        0        0      184 2024-05-29 07:36:34.000000 pybalebot-0.0.2/pybalebot/methods/updates/webhook_info.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.828570 pybalebot-0.0.2/pybalebot/methods/users/
--rw-rw-rw-   0        0        0       69 2024-05-28 21:06:54.000000 pybalebot-0.0.2/pybalebot/methods/users/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-28 21:18:48.000000 pybalebot-0.0.2/pybalebot/methods/users/get_me.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.835401 pybalebot-0.0.2/pybalebot/types/
--rw-rw-rw-   0        0        0      331 2024-05-29 08:32:11.000000 pybalebot-0.0.2/pybalebot/types/__init__.py
--rw-rw-rw-   0        0        0      481 2024-05-29 08:13:01.000000 pybalebot-0.0.2/pybalebot/types/inline_keyboard_button.py
--rw-rw-rw-   0        0        0      374 2024-05-29 08:14:00.000000 pybalebot-0.0.2/pybalebot/types/inline_keyboard_markup.py
--rw-rw-rw-   0        0        0        0 2024-05-29 12:33:17.000000 pybalebot-0.0.2/pybalebot/types/input_file.py
--rw-rw-rw-   0        0        0      440 2024-05-29 08:14:30.000000 pybalebot-0.0.2/pybalebot/types/keyboard_button.py
--rw-rw-rw-   0        0        0     4278 2024-05-29 12:42:00.000000 pybalebot-0.0.2/pybalebot/types/message.py
--rw-rw-rw-   0        0        0      718 2024-05-29 08:23:19.000000 pybalebot-0.0.2/pybalebot/types/reply_keyboard_markup.py
--rw-rw-rw-   0        0        0      340 2024-05-29 08:23:53.000000 pybalebot-0.0.2/pybalebot/types/reply_keyboard_remove.py
--rw-rw-rw-   0        0        0     5914 2024-05-28 19:42:55.000000 pybalebot-0.0.2/pybalebot/types/results.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:43:58.836378 pybalebot-0.0.2/pybalebot.egg-info/
--rw-rw-rw-   0        0        0     3048 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 12:43:58.000000 pybalebot-0.0.2/pybalebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 12:43:58.838329 pybalebot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1533 2024-05-29 12:43:19.000000 pybalebot-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.660852 pybalebot-0.0.3/
+-rw-rw-rw-   0        0        0     3048 2024-06-02 14:04:27.659879 pybalebot-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1888 2024-05-29 12:43:10.000000 pybalebot-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.544880 pybalebot-0.0.3/pybalebot/
+-rw-rw-rw-   0        0        0      112 2024-05-29 12:43:40.000000 pybalebot-0.0.3/pybalebot/__init__.py
+-rw-rw-rw-   0        0        0     8681 2024-06-02 01:40:18.000000 pybalebot-0.0.3/pybalebot/api.py
+-rw-rw-rw-   0        0        0     4609 2024-05-30 09:50:09.000000 pybalebot-0.0.3/pybalebot/client.py
+-rw-rw-rw-   0        0        0      357 2024-05-28 18:40:53.000000 pybalebot-0.0.3/pybalebot/errors.py
+-rw-rw-rw-   0        0        0    12012 2024-05-29 12:36:09.000000 pybalebot-0.0.3/pybalebot/filters.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.581786 pybalebot-0.0.3/pybalebot/methods/
+-rw-rw-rw-   0        0        0      286 2024-05-29 17:12:09.000000 pybalebot-0.0.3/pybalebot/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.595217 pybalebot-0.0.3/pybalebot/methods/chats/
+-rw-rw-rw-   0        0        0      783 2024-05-29 22:26:28.000000 pybalebot-0.0.3/pybalebot/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0      332 2024-05-29 09:26:07.000000 pybalebot-0.0.3/pybalebot/methods/chats/ban_chat_member.py
+-rw-rw-rw-   0        0        0      310 2024-05-29 16:24:25.000000 pybalebot-0.0.3/pybalebot/methods/chats/export_chat_invite_link.py
+-rw-rw-rw-   0        0        0      236 2024-05-29 09:50:52.000000 pybalebot-0.0.3/pybalebot/methods/chats/get_chat.py
+-rw-rw-rw-   0        0        0      291 2024-05-29 10:35:12.000000 pybalebot-0.0.3/pybalebot/methods/chats/get_chat_administrators.py
+-rw-rw-rw-   0        0        0      332 2024-05-29 16:33:16.000000 pybalebot-0.0.3/pybalebot/methods/chats/get_chat_member.py
+-rw-rw-rw-   0        0        0      286 2024-05-29 17:42:17.000000 pybalebot-0.0.3/pybalebot/methods/chats/get_chat_member_count.py
+-rw-rw-rw-   0        0        0      275 2024-05-29 09:47:43.000000 pybalebot-0.0.3/pybalebot/methods/chats/leave_chat.py
+-rw-rw-rw-   0        0        0      344 2024-05-29 09:37:50.000000 pybalebot-0.0.3/pybalebot/methods/chats/promote_chat_member.py
+-rw-rw-rw-   0        0        0      345 2024-05-29 22:25:59.000000 pybalebot-0.0.3/pybalebot/methods/chats/send_chat_action.py
+-rw-rw-rw-   0        0        0      802 2024-05-29 21:14:30.000000 pybalebot-0.0.3/pybalebot/methods/chats/set_chat_photo.py
+-rw-rw-rw-   0        0        0      473 2024-05-29 09:29:10.000000 pybalebot-0.0.3/pybalebot/methods/chats/unban_chat_member.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.597290 pybalebot-0.0.3/pybalebot/methods/invoices/
+-rw-rw-rw-   0        0        0       87 2024-05-29 16:46:02.000000 pybalebot-0.0.3/pybalebot/methods/invoices/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-05-29 16:44:41.000000 pybalebot-0.0.3/pybalebot/methods/invoices/send_nvoice.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.621096 pybalebot-0.0.3/pybalebot/methods/messages/
+-rw-rw-rw-   0        0        0     1048 2024-05-29 22:51:02.000000 pybalebot-0.0.3/pybalebot/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0      455 2024-05-29 07:46:15.000000 pybalebot-0.0.3/pybalebot/methods/messages/copy_message.py
+-rw-rw-rw-   0        0        0      340 2024-05-29 09:34:04.000000 pybalebot-0.0.3/pybalebot/methods/messages/delete_message.py
+-rw-rw-rw-   0        0        0      772 2024-05-29 22:49:32.000000 pybalebot-0.0.3/pybalebot/methods/messages/edit_message_caption.py
+-rw-rw-rw-   0        0        0      416 2024-05-28 21:39:07.000000 pybalebot-0.0.3/pybalebot/methods/messages/edit_message_text.py
+-rw-rw-rw-   0        0        0      464 2024-05-29 07:43:58.000000 pybalebot-0.0.3/pybalebot/methods/messages/forward_message.py
+-rw-rw-rw-   0        0        0      437 2024-05-29 21:37:54.000000 pybalebot-0.0.3/pybalebot/methods/messages/pin_chat_message.py
+-rw-rw-rw-   0        0        0     2297 2024-05-29 21:00:15.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_animation.py
+-rw-rw-rw-   0        0        0     2249 2024-05-29 20:55:34.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_audio.py
+-rw-rw-rw-   0        0        0     1796 2024-05-29 21:12:09.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_contact.py
+-rw-rw-rw-   0        0        0     2285 2024-05-29 20:27:06.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     1890 2024-05-29 21:09:34.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_location.py
+-rw-rw-rw-   0        0        0     1345 2024-05-29 21:34:16.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_media_group.py
+-rw-rw-rw-   0        0        0      818 2024-05-31 01:20:20.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     2252 2024-05-29 20:53:47.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     2342 2024-05-29 22:36:25.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_poll.py
+-rw-rw-rw-   0        0        0     2249 2024-05-29 21:09:03.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     2249 2024-05-29 21:01:46.000000 pybalebot-0.0.3/pybalebot/methods/messages/send_voice.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.627989 pybalebot-0.0.3/pybalebot/methods/others/
+-rw-rw-rw-   0        0        0      357 2024-06-02 00:56:56.000000 pybalebot-0.0.3/pybalebot/methods/others/__init__.py
+-rw-rw-rw-   0        0        0     1416 2024-06-02 01:32:35.000000 pybalebot-0.0.3/pybalebot/methods/others/answer_callback_query.py
+-rw-rw-rw-   0        0        0     2165 2024-05-30 10:24:30.000000 pybalebot-0.0.3/pybalebot/methods/others/answer_inline_query.py
+-rw-rw-rw-   0        0        0      128 2024-05-29 17:01:06.000000 pybalebot-0.0.3/pybalebot/methods/others/close.py
+-rw-rw-rw-   0        0        0      555 2024-06-02 00:56:29.000000 pybalebot-0.0.3/pybalebot/methods/others/download.py
+-rw-rw-rw-   0        0        0      177 2024-05-29 17:05:15.000000 pybalebot-0.0.3/pybalebot/methods/others/get_file.py
+-rw-rw-rw-   0        0        0      131 2024-05-29 16:58:53.000000 pybalebot-0.0.3/pybalebot/methods/others/logout.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.632110 pybalebot-0.0.3/pybalebot/methods/stickers/
+-rw-rw-rw-   0        0        0      260 2024-05-30 11:28:49.000000 pybalebot-0.0.3/pybalebot/methods/stickers/__init__.py
+-rw-rw-rw-   0        0        0      959 2024-05-30 11:28:05.000000 pybalebot-0.0.3/pybalebot/methods/stickers/add_sticker_to_set.py
+-rw-rw-rw-   0        0        0      975 2024-05-30 11:24:01.000000 pybalebot-0.0.3/pybalebot/methods/stickers/create_new_sticker_set.py
+-rw-rw-rw-   0        0        0     1688 2024-05-30 11:22:24.000000 pybalebot-0.0.3/pybalebot/methods/stickers/upload_sticker_file.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.638004 pybalebot-0.0.3/pybalebot/methods/updates/
+-rw-rw-rw-   0        0        0      324 2024-05-29 17:14:09.000000 pybalebot-0.0.3/pybalebot/methods/updates/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-05-29 17:13:44.000000 pybalebot-0.0.3/pybalebot/methods/updates/delete_webhook.py
+-rw-rw-rw-   0        0        0      283 2024-05-29 19:25:40.000000 pybalebot-0.0.3/pybalebot/methods/updates/get_updates.py
+-rw-rw-rw-   0        0        0      157 2024-05-29 07:34:51.000000 pybalebot-0.0.3/pybalebot/methods/updates/get_webhook_info.py
+-rw-rw-rw-   0        0        0      181 2024-05-29 07:32:36.000000 pybalebot-0.0.3/pybalebot/methods/updates/set_webhook.py
+-rw-rw-rw-   0        0        0      184 2024-05-29 07:36:34.000000 pybalebot-0.0.3/pybalebot/methods/updates/webhook_info.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.642066 pybalebot-0.0.3/pybalebot/methods/users/
+-rw-rw-rw-   0        0        0      152 2024-05-29 22:56:27.000000 pybalebot-0.0.3/pybalebot/methods/users/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-28 21:18:48.000000 pybalebot-0.0.3/pybalebot/methods/users/get_me.py
+-rw-rw-rw-   0        0        0     1010 2024-05-29 22:56:08.000000 pybalebot-0.0.3/pybalebot/methods/users/get_user_profile_photos.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.656977 pybalebot-0.0.3/pybalebot/types/
+-rw-rw-rw-   0        0        0     2934 2024-05-30 10:58:09.000000 pybalebot-0.0.3/pybalebot/types/__init__.py
+-rw-rw-rw-   0        0        0     3775 2024-06-02 01:27:47.000000 pybalebot-0.0.3/pybalebot/types/callback_query.py
+-rw-rw-rw-   0        0        0      481 2024-05-29 08:13:01.000000 pybalebot-0.0.3/pybalebot/types/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0      374 2024-05-29 08:14:00.000000 pybalebot-0.0.3/pybalebot/types/inline_keyboard_markup.py
+-rw-rw-rw-   0        0        0     2670 2024-05-30 10:25:25.000000 pybalebot-0.0.3/pybalebot/types/inline_query_result.py
+-rw-rw-rw-   0        0        0     2033 2024-05-29 21:32:47.000000 pybalebot-0.0.3/pybalebot/types/input_file.py
+-rw-rw-rw-   0        0        0      298 2024-05-29 18:26:16.000000 pybalebot-0.0.3/pybalebot/types/input_media_animation.py
+-rw-rw-rw-   0        0        0      286 2024-05-29 18:28:32.000000 pybalebot-0.0.3/pybalebot/types/input_media_audio.py
+-rw-rw-rw-   0        0        0      231 2024-05-29 18:27:03.000000 pybalebot-0.0.3/pybalebot/types/input_media_document.py
+-rw-rw-rw-   0        0        0      198 2024-05-29 18:29:16.000000 pybalebot-0.0.3/pybalebot/types/input_media_photo.py
+-rw-rw-rw-   0        0        0      290 2024-05-29 18:29:55.000000 pybalebot-0.0.3/pybalebot/types/input_media_video.py
+-rw-rw-rw-   0        0        0      440 2024-05-29 08:14:30.000000 pybalebot-0.0.3/pybalebot/types/keyboard_button.py
+-rw-rw-rw-   0        0        0    13317 2024-06-02 01:34:21.000000 pybalebot-0.0.3/pybalebot/types/message.py
+-rw-rw-rw-   0        0        0      718 2024-05-29 08:23:19.000000 pybalebot-0.0.3/pybalebot/types/reply_keyboard_markup.py
+-rw-rw-rw-   0        0        0      340 2024-05-29 08:23:53.000000 pybalebot-0.0.3/pybalebot/types/reply_keyboard_remove.py
+-rw-rw-rw-   0        0        0     5914 2024-05-28 19:42:55.000000 pybalebot-0.0.3/pybalebot/types/results.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:04:27.657920 pybalebot-0.0.3/pybalebot.egg-info/
+-rw-rw-rw-   0        0        0     3048 2024-06-02 14:04:27.000000 pybalebot-0.0.3/pybalebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3127 2024-06-02 14:04:27.000000 pybalebot-0.0.3/pybalebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:04:27.000000 pybalebot-0.0.3/pybalebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 14:04:27.000000 pybalebot-0.0.3/pybalebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 14:04:27.000000 pybalebot-0.0.3/pybalebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 14:04:27.660852 pybalebot-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1533 2024-06-02 14:04:10.000000 pybalebot-0.0.3/setup.py
```

### Comparing `pybalebot-0.0.2/PKG-INFO` & `pybalebot-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybalebot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Modern and fully asynchronous framework for Bale Bot API
 Home-page: https://github.com/shayanheidari01/pybalebot
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybalebot Version: 0.0.2 Summary: Modern and fully
+Metadata-Version: 2.1 Name: pybalebot Version: 0.0.3 Summary: Modern and fully
 asynchronous framework for Bale Bot API Home-page: https://github.com/
 shayanheidari01/pybalebot Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pybalebot-0.0.2/README.md` & `pybalebot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pybalebot-0.0.2/pybalebot/filters.py` & `pybalebot-0.0.3/pybalebot/filters.py`

 * *Files identical despite different names*

### Comparing `pybalebot-0.0.2/pybalebot/methods/chats/__init__.py` & `pybalebot-0.0.3/pybalebot/methods/chats/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from .unban_chat_member import UnbanChatMember
 from .ban_chat_member import BanChatMember
 from .promote_chat_member import PromoteChatMember
 from .set_chat_photo import SetChatPhoto
 from .leave_chat import LeaveChat
 from .get_chat import GetChat
-from .get_chat_member_count import GetChatMemberCount
+from .get_chat_member_count import GetChatMembersCount
 from .get_chat_administrators import GetChatAdministrators
+from .export_chat_invite_link import ExportChatInviteLink
+from .get_chat_member import GetChatMember
+from .send_chat_action import SendChatAction
 
 
 class Chats(
     UnbanChatMember,
     BanChatMember,
     PromoteChatMember,
     SetChatPhoto,
     LeaveChat,
     GetChat,
-    GetChatMemberCount,
-    GetChatAdministrators
+    GetChatMembersCount,
+    GetChatAdministrators,
+    ExportChatInviteLink,
+    GetChatMember,
+    SendChatAction
 ):
     pass
```

### Comparing `pybalebot-0.0.2/pybalebot/methods/messages/send_message.py` & `pybalebot-0.0.3/pybalebot/methods/messages/send_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,12 +9,13 @@
     async def send_message(
             self: "pybalebot.Client",
             chat_id: Union[str, int],
             text: str,
             reply_to_message_id: int = None,
             reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove]] = None
     ):
-        data = dict(chat_id=chat_id,
-                    text=text,
-                    reply_to_message_id=reply_to_message_id,
-                    reply_markup=reply_markup)
+        data = dict(chat_id=chat_id, text=text)
+        if reply_to_message_id:
+            data['reply_to_message_id'] = reply_to_message_id
+        if reply_markup:
+            data['reply_markup'] = reply_markup.to_dict()
         return await self.api.execute('sendMessage', data=data)
```

### Comparing `pybalebot-0.0.2/pybalebot/methods/messages/send_photo.py` & `pybalebot-0.0.3/pybalebot/methods/messages/send_photo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-import pybalebot
-
 from pybalebot.types import InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove
 from typing import Optional, Union
+import pybalebot
+import aiohttp
+import aiofiles
+import os
+
 
 class SendPhoto:
     async def send_photo(
-        self: "pybalebot.Client",
-        chat_id: Union[int, str],
-        photo: Union[str, bytes],
-        caption: Optional[str] = None,
-        from_chat_id: Union[int, str] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove]] = None
-    ):
-        """
-        Send a photo to a chat.
+            self: "pybalebot.Client",
+            chat_id: Union[str, int],
+            photo: str,
+            caption: Optional[str] = None,
+            reply_to_message_id: Optional[int] = None,
+            reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove]] = None
+    ) -> dict:
+        """Send a document.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel (in the format @channelusername).
-        :param from_chat_id: Unique identifier for the chat where the original message was sent (or username of the channel in the format @channelusername).
-        :param photo: Photo to send. Pass a file_id as String to send a photo that exists on the Bale servers (recommended), an HTTP URL as a String for Bale to get a photo from the internet, or upload a new photo using multipart/form-data.
-        :param caption: Photo caption (0-1024 characters after entities parsing).
-        :param reply_to_message_id: If the message is a reply, ID of the original message.
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
-        :return: On success, the sent Message is returned.
-        """
-        data = {
-            'chat_id': chat_id,
-            'from_chat_id': from_chat_id or chat_id,
-            'photo': photo
-        }
-        if caption:
-            data['caption'] = caption
-        if reply_to_message_id:
-            data['reply_to_message_id'] = reply_to_message_id
-        if reply_markup:
-            data['reply_markup'] = reply_markup.to_dict()
+        Args:
+            chat_id (Union[str, int]): Unique identifier for the target chat or username of the target channel.
+            document (str): File path of the document to be sent.
+            caption (Optional[str], optional): Caption for the document, 0-1024 characters. Defaults to None.
+            reply_to_message_id (Optional[int], optional): If the message is a reply, ID of the original message. Defaults to None.
+            reply_markup (Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove]], optional): Additional interface options. Defaults to None.
 
-        return await self.api.execute('sendPhoto', data)
+        Returns:
+            dict: On success, the sent Message is returned.
+        """
+        if os.path.isfile(photo):
+            async with aiofiles.open(photo, 'rb') as f:
+                form = aiohttp.FormData()
+                form.add_field('chat_id', str(chat_id))
+                form.add_field('caption', caption or '')
+                form.add_field('reply_to_message_id', reply_to_message_id or '')
+                if reply_markup is not None:
+                    form.add_field('reply_markup', reply_markup.to_dict())
+                form.add_field('photo', await f.read(), filename=os.path.basename(photo))
+            return await self.api.execute('sendPhoto', form=form)
+        else:
+            data = {
+                'chat_id': str(chat_id),
+                'photo': photo,
+                'caption': caption,
+                'reply_to_message_id': reply_to_message_id,
+                'reply_markup': reply_markup,
+            }
+            return await self.api.execute('sendPhoto', data=data)
```

### Comparing `pybalebot-0.0.2/pybalebot/types/reply_keyboard_markup.py` & `pybalebot-0.0.3/pybalebot/types/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pybalebot-0.0.2/pybalebot/types/results.py` & `pybalebot-0.0.3/pybalebot/types/results.py`

 * *Files identical despite different names*

### Comparing `pybalebot-0.0.2/pybalebot.egg-info/PKG-INFO` & `pybalebot-0.0.3/pybalebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybalebot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Modern and fully asynchronous framework for Bale Bot API
 Home-page: https://github.com/shayanheidari01/pybalebot
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybalebot Version: 0.0.2 Summary: Modern and fully
+Metadata-Version: 2.1 Name: pybalebot Version: 0.0.3 Summary: Modern and fully
 asynchronous framework for Bale Bot API Home-page: https://github.com/
 shayanheidari01/pybalebot Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: pybalebot,bale,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pybalebot-0.0.2/pybalebot.egg-info/SOURCES.txt` & `pybalebot-0.0.3/pybalebot.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,37 +9,73 @@
 pybalebot.egg-info/SOURCES.txt
 pybalebot.egg-info/dependency_links.txt
 pybalebot.egg-info/requires.txt
 pybalebot.egg-info/top_level.txt
 pybalebot/methods/__init__.py
 pybalebot/methods/chats/__init__.py
 pybalebot/methods/chats/ban_chat_member.py
+pybalebot/methods/chats/export_chat_invite_link.py
 pybalebot/methods/chats/get_chat.py
 pybalebot/methods/chats/get_chat_administrators.py
+pybalebot/methods/chats/get_chat_member.py
 pybalebot/methods/chats/get_chat_member_count.py
 pybalebot/methods/chats/leave_chat.py
 pybalebot/methods/chats/promote_chat_member.py
+pybalebot/methods/chats/send_chat_action.py
 pybalebot/methods/chats/set_chat_photo.py
 pybalebot/methods/chats/unban_chat_member.py
+pybalebot/methods/invoices/__init__.py
+pybalebot/methods/invoices/send_nvoice.py
 pybalebot/methods/messages/__init__.py
 pybalebot/methods/messages/copy_message.py
 pybalebot/methods/messages/delete_message.py
+pybalebot/methods/messages/edit_message_caption.py
 pybalebot/methods/messages/edit_message_text.py
 pybalebot/methods/messages/forward_message.py
+pybalebot/methods/messages/pin_chat_message.py
+pybalebot/methods/messages/send_animation.py
+pybalebot/methods/messages/send_audio.py
+pybalebot/methods/messages/send_contact.py
+pybalebot/methods/messages/send_document.py
+pybalebot/methods/messages/send_location.py
+pybalebot/methods/messages/send_media_group.py
 pybalebot/methods/messages/send_message.py
 pybalebot/methods/messages/send_photo.py
+pybalebot/methods/messages/send_poll.py
+pybalebot/methods/messages/send_video.py
+pybalebot/methods/messages/send_voice.py
+pybalebot/methods/others/__init__.py
+pybalebot/methods/others/answer_callback_query.py
+pybalebot/methods/others/answer_inline_query.py
+pybalebot/methods/others/close.py
+pybalebot/methods/others/download.py
+pybalebot/methods/others/get_file.py
+pybalebot/methods/others/logout.py
+pybalebot/methods/stickers/__init__.py
+pybalebot/methods/stickers/add_sticker_to_set.py
+pybalebot/methods/stickers/create_new_sticker_set.py
+pybalebot/methods/stickers/upload_sticker_file.py
 pybalebot/methods/updates/__init__.py
+pybalebot/methods/updates/delete_webhook.py
 pybalebot/methods/updates/get_updates.py
 pybalebot/methods/updates/get_webhook_info.py
 pybalebot/methods/updates/set_webhook.py
 pybalebot/methods/updates/webhook_info.py
 pybalebot/methods/users/__init__.py
 pybalebot/methods/users/get_me.py
+pybalebot/methods/users/get_user_profile_photos.py
 pybalebot/types/__init__.py
+pybalebot/types/callback_query.py
 pybalebot/types/inline_keyboard_button.py
 pybalebot/types/inline_keyboard_markup.py
+pybalebot/types/inline_query_result.py
 pybalebot/types/input_file.py
+pybalebot/types/input_media_animation.py
+pybalebot/types/input_media_audio.py
+pybalebot/types/input_media_document.py
+pybalebot/types/input_media_photo.py
+pybalebot/types/input_media_video.py
 pybalebot/types/keyboard_button.py
 pybalebot/types/message.py
 pybalebot/types/reply_keyboard_markup.py
 pybalebot/types/reply_keyboard_remove.py
 pybalebot/types/results.py
```

### Comparing `pybalebot-0.0.2/setup.py` & `pybalebot-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp']
 
 with open('README.md', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(
     name = 'pybalebot',
-    version = '0.0.2',
+    version = '0.0.3',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'Modern and fully asynchronous framework for Bale Bot API',
     keywords = ['pybalebot', 'bale', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires='~=3.7',
     long_description_content_type = 'text/markdown',
```

